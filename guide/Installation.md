# PocoF1 Установка Винды 11 [Без пека]
<img align="right" src="beryllium.png" width="350" alt="Windows installation on beryllium">

[![download](https://github.com/Kumar-Jy/Windows-in-PocoF1-Without-PC/assets/20044626/3abc8b52-c5c6-4495-b623-d1312195d639)]()
## Steps for Installation
- 1 шаг - Разметка
- 2 шаг - Установка
- 3 шаг - Дуалбут
#
### Необходимо
- _Мозги_(Обязательно)

- _Анлокнутый загрузчик_ 

- _Рут и кастомное рекавери_
#
### [Ахтунг]
> - _Все данные будут удалены! Сделайте бэкап _
> - _Сделать бэкап важных разделов (Boot, EFS, Modem and Persist) и скопируйте из внутренней памяти
> - _нужен [root](https://github.com/Kumar-Jy/Windows-in-PocoF1-Without-PC/blob/main/guide/root.md) почитайте этот гайд перед этим
> - _не прошивайте /не выполняйте одни и те же файлы или команды 2 раза если указано._
> - СЛЕДУЙТЕ ГАЙДУ ВНИМАТЕЛЬНО
> - _YOU CAN BREAK YOUR DEVICE WITH THE COMMANDS/FILE BELOW IF YOU DO THEM WRONG!!!_
> - _DO NOT REBOOT YOUR PHONE! If you think you made a mistake, ask for help in the [Telegram chat](https://t.me/WinInstaller)._
#

### 1st Step - Partitioning
- Flash [Modified Recovery](https://github.com/Kumar-Jy/Windows-in-PocoF1-Without-PC/releases/tag/Modified-Recovery).
- Goto mount section and unmount all partition.
- Open recovery terminal and type ` partition $ ` _[Replace $ with the size of storage in GB you want for Windows, Ex. - for 40GB type `partition 40`] (do not add GB at the end.)_
- If it asks you to run it once again, do so
- Reboot to check if Android still works. If it doesn't boot, format userdata and Reboot.
- Root it (if not already rooted), Install Magisk/KernalSU
- #### Notes :- 
> - if your phone encrypted first unmount and format userdata then type above command to create partition.
> - If you already modified or installed Windows, first type ` restore ` then type above command to create new partition. 
#

### 2nd Step - Installation
- Download [windows esd image](https://arkt-7.github.io/woawin/)
- Download [WinInstaller.zip](https://github.com/Kumar-Jy/Windows-in-PocoF1-Without-PC/releases/tag/PocoF1_WinInstaller)
- The ESD file must be in the Download folder of the phone's memory, or if you need to flash it through a MEMORY_CARD or PENDRIVE, create a folder named `WOA` and copy ESD and WinInstaller.zip into it."
- Reboot to recovery and flash wininstaller.zip
- That's all , 
 You don't need to touch you phone just sit back and watch, all installation process start automatically and phone will reboot to windows setup.
- #### Notes :- 
> - Must format windows partition by typing `format` command on recovery terminal, If you have to re-flash it by-any reasons or there is already windows installed.
> - Remove any attached usb device or charger before flashing, else it may be BSOD error.
> - Visit _[troubleshooting](troubleshooting.md)_ if any error.

#
### Last Step - Dual Boot Setup
#### _Switch to Android_
- Run `Android` Icon from windows desktop to boot into Android.
#### _Switch to Windows_
- Open WOA Helper app (Install it from Download folder and grant root access, and press ``QUICKBOOT TO WINDOWS``, it will boot in windows.

# 
### Miscellaneous:-
#### _If change to new Android_ 
- You can install any Android Rom but must copy android boot.img of newly installed android to the windows partition.
- For creating backup of android boot.img on windows partition, first root it then boot to modded recovery - open terminal and type ``dd if=/dev/block/by-name/boot of=/win/boot.img`` .

#### _If format userdata_
- Download [Device Info HW app](https://play.google.com/store/apps/details?id=ru.andr7e.deviceinfohw&pcampaignid=web_share), and check your touch panel type
- Creat a folder in the phone storage and rename it to `UEF`  - Download [new-boot.img](https://github.com/Kumar-Jy/Windows-in-PocoF1-Without-PC/releases/tag/UEFI-Boot-Image) according to your touch panel and place it in `UEFI` folder.
- Download and install the [WOA Helper app](https://github.com/n00b69/woa-helper/releases), open it and grant root access.
- Now you can boot to windows by pressing ``QUICKBOOT TO WINDOWS`` .

#### _Windows re-installation_
- Download WinInstaller.zip and Windows ESD file.
- Boot to modded recovery.
- open recovery terminal, type `format` and press enter (it will format previously installed windows)
- Now reboot to recovery again and flash Wininstaller.zip
#
# _[Troubleshooting](troubleshooting.md)_


## Support My Work

#### If you find my projects helpful, consider supporting my work! Your contributions will help me keep developing and sharing useful resources.

<p align="left">
  <a href="https://www.buymeacoffee.com/kumarjy" target="_blank">
    <img src="https://github.com/Kumar-Jy/Windows-in-PocoF1-Without-PC/blob/main/guide/buymecoffee.png" alt="Buy Me A Coffee" style="height: 60px !important; width: 217px !important;">
  </a>
</p>
