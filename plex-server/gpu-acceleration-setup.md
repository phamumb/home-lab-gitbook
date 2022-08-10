---
description: Guideline to setup Plex Hardware Acceleration function
cover: >-
  https://www.hardwaretimes.com/wp-content/uploads/2019/11/nvidia-eye-siggraph-2018.jpg
coverY: 0
---

# GPU Acceleration Setup



![Quadro M2000](https://www.pny.com/productimages/4EAB7262-FDC4-4085-A75C-31EB2D772A57/images/PNY-Quadro-M2000-front-1.png)

### Pre-setup Plex Hardware Acceleration

* Pre-req for GPU offload

```
apt install beignet-opencl-icd
apt install ocl-icd-libopencl1
```

* Install NVIDIA drivers (optional if doing GPU transcoding). Install ubuntu package to identify the drivers necessary for your particular GPU

```
apt install ubuntu-drivers-common 
```

* List the graphics devices to get the nvidia drivers needed

```
ubuntu-drivers devices
```

* Install latest drivers (replace xxx with driver package you want to use)

```
apt install nvidia-drivers-xxx 
```

* After install the driver package will also install the ubuntu GUI environment, this will turn it back off. (skip this step if you want the GUI for some reason)

```
systemctl set-default multi-user
```

* Reboot system, done !

```
shutdown -r now
```

### Setup Plex Hardware inside Container

#### Installing the NVIDIA container toolkit

```
# Update apt.
sudo apt-get update

# Install the nvidia-docker2 package.
sudo apt-get install -y nvidia-docker2

# Restart Docker.
sudo systemctl restart docker

# Test the GPU with a base CUDA container.
sudo docker run --rm --gpus all nvidia/cuda:11.0.3-base-ubuntu20.04 nvidia-smi
```

After running all command above and installed all package, the final result should display as below

```
idia-smi

# Output
+-----------------------------------------------------------------------------+
| NVIDIA-SMI 510.73.05    Driver Version: 510.73.05    CUDA Version: 11.6     |
|-------------------------------+----------------------+----------------------+
| GPU  Name        Persistence-M| Bus-Id        Disp.A | Volatile Uncorr. ECC |
| Fan  Temp  Perf  Pwr:Usage/Cap|         Memory-Usage | GPU-Util  Compute M. |
|                               |                      |               MIG M. |
|===============================+======================+======================|
|   0  Quadro P2000        Off  | 00000000:0B:00.0 Off |                  N/A |
| 44%   31C    P8     5W /  75W |      2MiB /  5120MiB |      0%      Default |
|                               |                      |                  N/A |
+-------------------------------+----------------------+----------------------+
                                                                               
+-----------------------------------------------------------------------------+
| Processes:                                                                  |
|  GPU   GI   CI        PID   Type   Process name                  GPU Memory |
|        ID   ID                                                   Usage      |
|=============================================================================|
|  No running processes found                                                 |
+-----------------------------------------------------------------------------+
```

After confirming the result, we can deploy plex server following this instruction

{% content-ref url="setup.md" %}
[setup.md](setup.md)
{% endcontent-ref %}
