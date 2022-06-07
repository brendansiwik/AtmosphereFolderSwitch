# AtmosphereFolderSwitcher

A clunky TegraScript that manages 2 Atmosphere folders and SimpleModMenu folders so you can have 2 separate Atmosphere installs for sysMMC and emuMMC.

This is something I threw together awhile ago because I wanted a way to keep my sysMMC and emuMMC separate while having different sysmodules and mods installed in each. 

## Files Needed
+ [Latest Atmosphere Release](https://github.com/Atmosphere-NX/Atmosphere/releases)
    + Download the Atmosphere zip and fusee.bin
+ [Latest TegraExplorer Release](https://github.com/suchmememanyskill/TegraExplorer/releases)
+ The Latest Release of this obviously
    + I'm sure you can find the releases page yourself.
    + It's on the right if you need a hint.

## Installation
Make sure that atmosphere is currently booting into emuMMC by default. As long as emuMMC is enabled in hekate it should be.

Extract files to the root of your SD Card.

Extract the atmosphere folder from the latest release to swap/sysmmc/ on your sd card

Copy fusee.bin and TegraExplorer.bin to bootloader/payloads

Copy emuMMC/emummc.ini to swap/sysmmc

Open the copy you just made in notepad and change enabled=1 to enabled=0 and save it

## Usage

Launch hekate and select Payloads -> TegraExplorer.bin

Run the script called Boot.te at the bottom of the menu

Pick which you want to boot

To make it work even better set Atmosphere's reboot payload to hekate and have hekate autoboot TegraExplorer so you easily reboot from emuMMC to sysMMC or the other way around.

## Things to keep in mind

When you need to update Atmosphere remember to update the one in the root of your SD Card and the one in the folder of whichever option you weren't booted in.

## Credits
+ Everyone behind the [Atmosphere](https://github.com/Atmosphere-NX/Atmosphere) Custom Firmware
+ suchmememanyskill for [TegraExplorer](https://github.com/suchmememanyskill/TegraExplorer)
