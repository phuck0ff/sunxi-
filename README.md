# tab744
Files to drive or repair TAB744 INM7102AVD M7100AVD RTL8188ETV 8188EU GC0329 sun8iw5p1 astar m7100nobt tablets.

* First try to unxz and flash the ``img.xz`` firmware image using LiveSuit.
* If unsuccessful, all other files might help you debug and cook a firmware that works for you.

Log of successful flash looks like this:
```bash
--------------Init Called------------------
workDir /home/user/sunxi-livesuit/x86-64/LiveSuit
ImgLenHigh      0
ImgLenLow       673796096
Mode    8
hWnd    0
imgFilePath     /home/user/INM7102AVD_M7100AVD_RTL8188ETV_8188EU_GC0329_sun8iw5p1_astar_m7100nobt_20140917.img
[TL_MSG]:Mode = 8, ImgLenHigh=0, ImgLenLow = 28295000, imgFilePath = /home/user/INM7102AVD_M7100AVD_RTL8188ETV_8188EU_GC0329_sun8iw5p1_astar_m7100nobt_20140917.img

IMAGEWTY
ItemTableSize = 1048576
[TL_MSG]:Tools Open Img

---fun end---
--------------entry-fel2fes Called-----------
felDevName      /dev/aw_efex0
[TL_MSG]:Hi, I'm fel, dev=/dev/aw_efex0

[TL_MSG]:To down and Run fes1-1

[TL_MSG]:fes1 down addr = 0x2000, retAddr =0x7210

[TL_MSG]:To clear fes aide log

Dev Plugin The Device Path is: /dev/aw_efex0
Too Many Devices plugin...
[TL_FEX]:fel UP addr=0x7210, len=136

[TL_MSG]:SYS_PARA_LOG read = 0x4d415244

[TL_MSG]:dram paras[0]: 0x228

[TL_MSG]:dram paras[1]: 0x3

[TL_MSG]:dram paras[2]: 0x3bbb

[TL_MSG]:dram paras[3]: 0x1

[TL_MSG]:dram paras[4]: 0x10f20600

[TL_MSG]:dram paras[5]: 0x1000

[TL_MSG]:dram paras[6]: 0x1c70

[TL_MSG]:dram paras[7]: 0x40

[TL_MSG]:dram paras[8]: 0x18

[TL_MSG]:dram paras[9]: 0x0

[TL_MSG]:dram paras[10]: 0x47214f

[TL_MSG]:dram paras[11]: 0x1c2294b

[TL_MSG]:dram paras[12]: 0x61043

[TL_MSG]:dram paras[13]: 0x0

[TL_MSG]:dram paras[14]: 0x0

[TL_MSG]:dram paras[15]: 0x0

[TL_MSG]:dram paras[16]: 0x0

[TL_MSG]:dram paras[17]: 0x0

[TL_MSG]:dram paras[18]: 0x0

[TL_MSG]:dram paras[19]: 0x0

[TL_MSG]:dram paras[20]: 0x0

[TL_MSG]:dram paras[21]: 0x0

[TL_MSG]:dram paras[22]: 0xa8

[TL_MSG]:dram paras[23]: 0x40901

[TL_MSG]:dram paras[24]: 0x0

[TL_MSG]:dram paras[25]: 0x0

[TL_MSG]:dram paras[26]: 0x0

[TL_MSG]:dram paras[27]: 0x0

[TL_MSG]:dram paras[28]: 0x0

[TL_MSG]:dram paras[29]: 0x0

[TL_MSG]:dram paras[30]: 0x0

[TL_MSG]:dram paras[31]: 0x0

[TL_MSG]:To down and Run uboot

[TL_MSG]:u-boot down addr = 0x4a000000

[TL_MSG]:workmode = 0x10

---fun end---
Fel Thread Finished!
Dev Plugout The Device Path is: /dev/aw_efex0
Dev Plugout The Device Path is: /dev/aw_efex0
Dev Plugout The Device Path is: /dev/aw_efex0
Dev Plugin The Device Path is: /dev/aw_efex0
--------------entry fes_thread Called---------
portId  0
fesDevName      /dev/aw_efex0
hubId   0
DeviceId        1
[TL_MSG]:enter FES--/dev/aw_efex0

[TL_MSG]:Verify: media crc = 0

[TL_MSG]:save item to mem :(12345678,1234567890___MBR) realLen(65536)

./buffer.cpp, pBuffer = 0x7f9bec011604, nLen = 16380, crc32 = 112357176[TL_MSG]:name = bootloader, keydata = 0

[TL_MSG]:name = env, keydata = 0

[TL_MSG]:name = boot, keydata = 0

[TL_MSG]:name = system, keydata = 0

[TL_MSG]:name = data, keydata = 0

[TL_MSG]:name = misc, keydata = 0

[TL_MSG]:name = recovery, keydata = 0

[TL_MSG]:name = cache, keydata = 0

[TL_MSG]:name = metadata, keydata = 0

[TL_MSG]:name = private, keydata = 0

[TL_MSG]:name = UDISK, keydata = 0

[TL_MSG]:name = , keydata = 0

[TL_MSG]:Verify: media crc = 0

[TL_MSG]:down mbr success!!!

[TL_MSG]:dl file :save item to mem :(12345678,1234567890DLINFO) realLen(16384)

./buffer.cpp, pBuffer = 0x7f9bec218b54, nLen = 16380, crc32 = 256739088[TL_MSG]:------------dlmap dump--------------

[TL_MSG]:crc32     = 0xf4d8710

[TL_MSG]:version   = 0x200

[TL_MSG]:magic     = softw411

[TL_MSG]:part_cnt  = 6

[TL_MSG]:flash size is : 14761984 Sectors

[TL_MSG]:name = bootloader addrhi=0x0 addrlo = 0x8000  lenhi = 0x0 lenlo = 0x10000  file = BOOTLOADER_FEX00, en=0,vf=1

[TL_MSG]:need verify:1,VBOOTLOADER_FEX0

[TL_FEX]:8000, 615c00

[TL_MSG]:Verify:start = 8000 ,size = 615c00 ,pc_crc = d6b3738b, media crc = d6b3738b

[TL_MSG]:name = env addrhi=0x0 addrlo = 0x18000  lenhi = 0x0 lenlo = 0x8000  file = ENV_FEX000000000, en=0,vf=1

[TL_MSG]:need verify:1,VENV_FEX00000000

[TL_FEX]:18000, 20000

[TL_MSG]:Verify:start = 18000 ,size = 20000 ,pc_crc = 9b444057, media crc = 9b444057

[TL_MSG]:name = boot addrhi=0x0 addrlo = 0x20000  lenhi = 0x0 lenlo = 0x8000  file = BOOT_FEX00000000, en=0,vf=1

[TL_MSG]:need verify:1,VBOOT_FEX0000000

[TL_FEX]:20000, aef000

[TL_MSG]:Verify:start = 20000 ,size = aef000 ,pc_crc = c82fb952, media crc = c82fb952

[TL_MSG]:name = system addrhi=0x0 addrlo = 0x28000  lenhi = 0x0 lenlo = 0x180000  file = SYSTEM_FEX000000, en=0,vf=1

[TL_MSG]:find a sparse format part,SYSTEM_FEX000000

[TL_MSG]:item size :610 M

[TL_MSG]:magic = ed26ff3a

[TL_MSG]:blk_size = 1000

[TL_MSG]:total_chunk = 15

[TL_MSG]:tlBufImg size = 200000

Fes Device Plugin before Timeout!
Kill Timer!
[TL_MSG]:handled chunk = 15 total_chunk = 15

[TL_MSG]:name = recovery addrhi=0x0 addrlo = 0x3b0000  lenhi = 0x0 lenlo = 0x10000  file = RECOVERY_FEX0000, en=0,vf=1

[TL_MSG]:need verify:1,VRECOVERY_FEX000

[TL_FEX]:3b0000, db9000

[TL_MSG]:Verify:start = 3b0000 ,size = db9000 ,pc_crc = e19489d0, media crc = e19489d0

[TL_MSG]:name = UDISK addrhi=0x0 addrlo = 0x4d0000  lenhi = 0x0 lenlo = 0x0  file = DISKFS_FEX000000, en=0,vf=0

[TL_MSG]:work mode update ,udisk part ignore !!!!

[TL_MSG]:save item to mem :(12345678,UBOOT_0000000000) realLen(737280)

[TL_MSG]:Verify: media crc = 0

[TL_MSG]:down uboot success!!!

[TL_MSG]:storge type is 0 (0:nand 1-2:card 3:spinor)

[TL_MSG]:save item to mem :(BOOT    ,BOOT0_0000000000) realLen(32768)

[TL_MSG]:Verify: media crc = 0

[TL_MSG]:down boot0 success!!!

QObject::startTimer: QTimer can only be used with threads started with QThread
QObject::startTimer: QTimer can only be used with threads started with QThread
Dev Plugout The Device Path is: /dev/aw_efex0
[TL_MSG]:---fun end-----

---------------Exit Called-----------------
Closing image now! 

Clos image OK! 

[TL_MSG]:Tools Close Img ...

---fun end---
L302, Finished to call Tools.entry_fes_thread.
Dev Plugout The Device Path is: /dev/aw_efex0
Dev Plugout The Device Path is: /dev/aw_efex0
```
