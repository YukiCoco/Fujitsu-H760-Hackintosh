# Fujitsu_H760_Hackintosh

## Hardware
Processor: i7-6820HQ  
IGPU: Intel HD Graphics 530  
GPU: NVIDIA® Quadro® M1000M  
Audio: ALC255  
Wlan: Intel® Dual Band Wireless-AC8260

## Software
MacOS Catalina 10.15.7 (Tested)  

## What's Working
+ Touchpad (Support gesture)  
+ Keyboard  
+ IGPU  
+ Audio  
+ WLAN (Low performence)  
+ Bluetooth
+ CD/ROM  

## What's Not Working
+ NVIDIA® Quadro® M1000M  

## How to Fix CFG Lock  
**To use the EFI, you must fix Cfg lock at first.**  
**A USB flash disk is required.**  
Create a FAT32 volume on your USB flash disk, Create `EFI/Boot` directory, download [modGRUBShell.efi](https://github.com/datasone/grub-mod-setup_var/releases) and place it at `EFI/Boot`, rename to `bootx64.efi`.  Reboot your computer, press 'F12' and select USB flash disk.  

1. enter `setup_var 0x84A`, the value must be 0x01, then go next step.
2. enter `setup_var 0x84A 0x00`.

## Screenshot
![image](https://user-images.githubusercontent.com/18544362/136685321-f2ebbe3b-8f1f-4943-b19a-a0093eae7446.png)
![image](https://user-images.githubusercontent.com/18544362/136685296-9b45f24b-8d91-4529-a6c7-def81a0857f7.png)
![image](https://user-images.githubusercontent.com/18544362/136685270-5e7ed714-08bf-49d3-8bb7-f839189ab832.png)


