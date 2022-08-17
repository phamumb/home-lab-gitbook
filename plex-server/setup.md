---
description: >-
  Instructions and guideline showing setup a Plex media server, services
  automation
cover: https://cdn.wallpapersafari.com/44/94/zZvlng.jpg
coverY: 0
---

# Plex Media Server

![plex](../.gitbook/assets/plex.png)

## Prerequisites

* [Ubuntu 20.04 OS](https://ubuntu.com/download/server)
* [Docker Engine & Docker Compose](https://github.com/phamumb/home-lab-docsify/blob/main/docs/plex-server/docker/install-docker.md)
* [Docker NVIDIA container](https://github.com/phamumb/home-lab-docsify/blob/main/docs/plex-server/docker/nvidia-container.md)
* [RAID Array Level 5](https://github.com/phamumb/home-lab-docsify/blob/main/docs/plex-server/raid-array/create-raid-array.md)
* [PURE VPN](https://purevpn.com)

### Setting up Environment

* Modify the `~/.bashrc` to add `MEDIA_SERVER_PATH` permanently

```
nano ~/.bashrc
#add lines at the bottom of the file:
    export MEDIA_SERVER_PATH=<YOUR_MOUNT_PATH> (Depends on how you mount your RAID array location)
```

## Download Clients

### SABNzbd

* **Usage**

```
version: "2.1"
services:
  sabnzbd:
    image: lscr.io/linuxserver/sabnzbd:latest
    container_name: sabnzbd
    network_mode: host
    environment:
      - PUID=1000
      - PGID=1000
      - TZ=America/Newyork
    volumes:
      - ${MEDIA_SERVER_PATH}/configs/sabnzbd:/config
      - ${MEDIA_SERVER_PATH}/downloads:/downloads #optional
      - ${MEDIA_SERVER_PATH}/downloads/incomplete:/incomplete-downloads #optional
    restart: unless-stopped
```

### Transmission

* **Configuration**

```
  OPENVPN_PROVIDER=<VPN_PROVIDER>
  OPENVPN_CONFIG=<VPN_SERVER_NAME>
  OPENVPN_USERNAME=<VPN_USERNAME>
  OPENVPN_PASSWORD=<VPN_PASSWORD>
```

* **Usage**

```
  version: '2.1'
  services:
    transmission:
        image: haugene/transmission-openvpn
        container_name: transmission
        network_mode: host
        volumes:
            - ${MEDIA_SERVER_PATH}/configs/transmission:/config
            - ${MEDIA_SERVER_PATH}/downloads/transmission:/downloads/transmission
        env_file:
            - ./config.env
        environment:
            - PUID=0
            - PGID=0
            - CREATE_TUN_DEVICE=true
            - WEBPROXY_ENABLED=false
            - TRANSMISSION_DOWNLOAD_DIR=/downloads/transmission
            - TRANSMISSION_IDLE_SEEDING_LIMIT_ENABLED=true
            - TRANSMISSION_SEED_QUEUE_ENABLED=true
            - TRANSMISSION_INCOMPLETE_DIR_ENABLED=false
            - LOCAL_NETWORK=192.168.0.0/16
        cap_add:
            - NET_ADMIN
        logging:
            driver: json-file
            options:
                max-size: 10m
        restart: unless-stopped
```

## Indexers

### Prowlarr

```
---
version: "2.1"
services:
  prowlarr:
    image: lscr.io/linuxserver/prowlarr:develop
    container_name: prowlarr
    environment:
      - PUID=0
      - PGID=0
      - TZ=America/New_York
    volumes:
      - ${MEDIA_SERVER_PATH}/configs/prowlarr:/config
    network_mode: host
    restart: always
```

### NZBGeek

* Go to this site: [nzbgeek](https://nzbgeek.info/)
* Login with your credential
* NZBGeek host: https://api.nzbgeek.info/
* Click on the corner to get api key: `<username>` --> `my account`

### NZBPlanet

* Go to this site: [nzbgeek](https://nzbplanet.net/)
* Login with your credential
* NZBPlanet host: https://api.nzbplanet.net
* Click on the corner to get api key: `<username>` --> `my account`

## Services

### Radarr, Sonarr, Bazarr

![](https://images.opencollective.com/radarr/7348012/background.png)

Replace \<IMAGE> with:

* `lscr.io/linuxserver/sonarr:latest`
* `lscr.io/linuxserver/bazarr:latest`
* `lscr.io/linuxserver/radarr:latest`

```
---
version: "2.1"
services:
  radarr:
    image: <IMAGE>
    container_name: <SERVICE_NAME>
    environment:
      - PUID=1000
      - PGID=1000
      - TZ=America/Newyork
    volumes:
      - ${MEDIA_SERVER_PATH}/configs/<SERVICE_NAME>:/config
      - ${MEDIA_SERVER_PATH}/media:/movies #optional
      - ${MEDIA_SERVER_PATH}/downloads:/downloads #optional
    network_mode: host
    restart: unless-stopped
```

## Requesting

### Overseerr

![](https://overseerr.dev/screenshots/screen\_movie\_details.jpg)

```
---
version: "2.1"
services:
  overseerr:
    image: lscr.io/linuxserver/overseerr:latest
    container_name: overseerr
    environment:
      - PUID=1000
      - PGID=1000
      - TZ=America/New_York
    volumes:
      - ${MEDIA_SERVER_PATH}/configs/overseerr:/config
    ports:
      - 5055:5055
    restart: unless-stopped

```

## Plex Media Server

Create and run docker-compose file below to bring up plex server

```
---
version: "2.3"
services:
  plex:
    image: lscr.io/linuxserver/plex
    container_name: plex
    network_mode: host
    environment:
      - PUID=0
      - PGID=0
      - VERSION=docker
      - NVIDIA_DRIVER_CAPABILITIES=all
      - NVIDIA_VISIBLE_DEVICES=all
    volumes:
      - ${MEDIA_SERVER_PATH}/config/plex:/config
      - ${MEDIA_SERVER_PATH}/media:/media
    runtime: nvidia
    restart: unless-stopped

```
