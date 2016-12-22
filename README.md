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

----

## Mac style touch pad

```
vim synaptics-settings.sh

#!/bin/bash
synclient RightButtonAreaLeft=0
synclient RightButtonAreaTop=0

chmod a+rx ~/.synaptics-custom-settings.sh
```

Open the Startup Applications program in Unity and add ~/.synaptics-custom-settings.sh to the list of startup applications. This way, the custom trackpad settings will be applied automatically every time you log in.

http://askubuntu.com/questions/602193/how-to-disable-right-click-on-the-touchpad
