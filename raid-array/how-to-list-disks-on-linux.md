---
description: >-
  In many cases, you will have to list all the disks available on your computer,
  with their sizes, in order to make sure that they don’t run out of space.
---

# How To List Disks on Linux

### Prerequisites

For some of the commands used in this tutorial, you will need administrator rights in order to have the full output of the command.

In order to check that you have sudo rights, you can execute the “**sudo**” command with the “-l” option.

### List Disks on Linux using lsblk

**The easiest way to list disks on Linux is to use the “**[**lsblk**](https://linux.die.net/man/8/lsblk)**” command with no options. The “type” column will mention the “disk” as well as optional partitions and LVM available on it.**

```
lsblk -f
```

By executing the “**lsblk**” command, you are presented with multiple different columns :

* **Name** : the name of the device. It is quite important for you to know that Linux devices have a specific prefix depending on the nature of the device. “sd” in this case refers to SCSI devices but it is also short for SATA connections as most drives use SATA nowadays;
* **Filesystem type** : if your partition contains a filesystem, it should be listed in this column (xfs, swap or [encrypted devices](https://devconnected.com/how-to-encrypt-partition-on-linux/));
* **Label** : in some cases, in order to avoid using a UUID, you can choose to have a label for your device;
* **UUID** : a universal unique identifier. This identifier should be unique worldwide and uniquely identify your device;
* **Mountpoint** : if your filesystem is mounted, you should be able to see the actual mountpoint.

**Awesome, you successfully listed your disks on Linux using “lsblk”.**

However, in some cases, you are interested in listing your disks **with the actual hardware information** linked to it.

If I want to remove a disk from my Linux machine, knowing the actual physical port or the vendor can be quite useful.

### List Disks Information using lshw

**In order to list disk information on Linux, you have to use the “lshw” with the “class” option specifying “disk”. Combining “lshw” with the “grep” command, you can retrieve specific information about a disk on your system.**

```
$ sudo lshw -class disk

$ sudo lshw -class disk | grep <disk_name> -A 5 -B
```

As you can see, by running the “lshw” with no grep filters, you are presented with all the disks available on your computer.

If you want to target a specific disk on your computer, **you can “pipe” the command with “grep”** in order to only list the disks that you want.

As you can see, using this command, you have way more information about your disks : **the description, the product and its vendor as well as the actual bus info** (where it might be plugged on your mother board).

Using this information, you can unplug it and replace it with another one very easily.

**Awesome, you know how to list your disk information using “lshw” now.**

References:

[https://devconnected.com/how-to-list-disks-on-linux/](https://devconnected.com/how-to-list-disks-on-linux/)
