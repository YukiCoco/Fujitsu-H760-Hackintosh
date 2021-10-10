# Fujitsu_H760_Hackintosh

## Hardware
Processor: i7-6820HQ  
IGPU: Intel HD Graphics 530  
GPU: NVIDIA® Quadro® M1000M  
Audio: ALC255  
Wlan: Intel® Dual Band Wireless-AC8260

## Software
MacOS Catalina 10.15.7 (Tested)  

## What's work
+ Touchpad (support Apple gesture)  
+ Keyboard  
+ IGPU  
+ Audio  
+ WLAN (Low performence)  
+ CD/ROM  

## What's not work  
+ NVIDIA® Quadro® M1000M  

## How to Fix CFG Lock  
**To use the EFI, you must fix Cfg lock at first.**  
**A USB flash disk is required.**  
Create a FAT32 volume on your USB flash disk, Create `EFI/Boot` directory, download [modGRUBShell.efi](https://github.com/datasone/grub-mod-setup_var/releases) and place it at `EFI/Boot`, rename to `bootx64.efi`.  Reboot your computer, press 'F12' and select USB flash disk.  

1. enter `setup_var 0x84A`, the value must be 0x01, then go next step.
2. enter `setup_var 0x84A 0x00`.

