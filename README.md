# Lenovo IdeaPad Y410P NoteBook for macOS Mojave & High Sierra

Hackintosh your Y410P Notebook

[English](README.md) | [中文](README-CN.md)

## Features

* Support 10.13.x and 10.14.x
* ACPI fixes use hotpatch; related files are located in `/CLOVER/ACPI/patched`.

## What Works
* Graphics with full acceleration QE/CI (using Intel GPU only) + HDMI Video
* Audio using AppleALC
* Ethernet (LAN)
* WiFi / Bluetooth (after replacing the Intel card (incompatible) with a compatible one like Broadcom BCM4352 for example
* Sleep (also sleep on Lid Close)
* Brightness,Support use FN+Arrows﻿
* Battery
* Keyboard / Touchpad
* CPU Power Management
* Web-Cam
* All USB ports
* App Store/iCloud/iMessage/Facetime
* TRIM
* SIP (0ff)


## Problem
* VGA Port:This will not work at all. A workaround when projecting to VGA display is to buy and use (male)HDMI-to-(fem﻿ale)VGA adapter. 
* Restart:There is a problem related to graphics occurs when﻿ display goes off then on, like when system sleeps ﻿and wake or when changing display r﻿esolutio﻿n for example, which results in n﻿o display on restart﻿. These ev﻿ents requires re-initialization for the graphic driver but it seems the driver re-initialize incorrectly. As a result, the graphics related memory hold wrong data for some graphic registers which indirectly affects the restart functionality. Once the system is restarted in any of these scenarios, the POST (where Lenovo logo should appear) has no display and so is Clover and beyond if an OS is selected and booted using keyboard blindly. However, this is a graphic driver issue and has nothing to do with power or reboot function itself.
* Nvidia GPU (built-in): This will have to be disabled as OS X does not support Optimus technology.
* Truddy:There is a problem of truddy when boot the notebook if your notebook's bios be set to uefi only.


## Credits

- Thanks to RehabMan、intruder16、panybbib、ahmed_ais

