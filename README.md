# linux notes

## Partition using 2 hard disks (SSD and non-SSD)

* Solid state: / (root filesystem), /usr, /usr/local, /opt
* Spinning disk: /var, /home, /tmp, swap

http://unix.stackexchange.com/questions/89213/partitioning-using-2-hard-disks-ssd-and-non-ssd-in-linux

----

## Create a bootable USB from iso

```
sudo fdisk -l
dd if=filename.iso of=/dev/usbdevice
```
