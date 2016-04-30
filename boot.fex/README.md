```bash
unmkbootimg version 1.2 - Mikael Q Kuisma <kuisma@ping.se>
Kernel size 10154396
Kernel address 0x40008000
Ramdisk size 1304671
Ramdisk address 0x41300000
Secondary size 0
Secondary address 0x40f00000
Kernel tags address 0x40000100
Flash page size 2048
Board name is ""
Command line ""

*** WARNING ****
This image is built using NON-standard mkbootimg!
OFF_RAMDISK_ADDR is 0x01300000
Please modify mkbootimg.c using the above values to build your image.
****************

Extracting kernel to file zImage ...
Extracting root filesystem to file initramfs.cpio.gz ...
All done.
---------------
To recompile this image, use:
  mkbootimg --kernel zImage --ramdisk initramfs.cpio.gz --base 0x40000000 -o new_boot.img
---------------
```
