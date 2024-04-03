# MOD firmwares

Each firmware builds upon the previous firmware (usually), so you get all the benefits of the past versions.

## BCD436HP_V1_99_09.bin (based on v1.99.05)

* Add Hytera BP (Basic Privacy) and Motorola BP (Basic Privacy) decryption with known key
* Now "Set Debug Log Mode" submenu always enabled in the "Settings" menu

 https://github.com/x27/openscanner/releases/tag/BCD436HP_1.99.09

## BCD436HP_V1_99_05.bin (based on v1.99.04)
* Visual information about the mod version (boot screen)
* Output debugging information about DMR traffic.

To get debugging information, you need to turn on the scanner by pressing POWER+AVOID, 
then in the "Settings" menu in the submenu "Set Debug Log Mode" you need to select 
"SD Card(File)" or "USB (Serial)".

## BCD436HP_V1_99_04.bin (based on v1.99.03)

Fix: Show extended Net/System/Site/TG info for any custom search name

Description of the problem: https://forums.radioreference.com/threads/custom-search-bcd436hp.343396/

Video of the problem: https://www.youtube.com/watch?v=j64LAJJox2Y

## BCD436HP_V1_99_03.bin (based on v1.28.14)

* Removed gaps on bands
* Unmute when received all encrypted traffic

## BCD436HP_V1_99_02.bin (based on v1.28.14)

* Unmute when received all encrypted traffic

## BCD436HP_V1_99_01.bin (based on v1.28.14)

* Sound On when received encrypted DMR traffic

## BCD436HP_V1_28_16.bin

* Set min alarm low voltage to 2700 mV

## BCD436HP_V1_28_15.bin

* Removed gaps on bands (based on BCD436HP 1.28.14)

### Sentinel (Control Software)

pss. patched sentinel (2.05.03) .exe file for support scanners with mod fw located here: https://mega.nz/file/NBtlRKxC#54LBK3Qiuqtsd0ZzQWZ_SfnRTqukdHuPXGChtUu5mXY

official version sentinel (2.05.03) located here: https://info.uniden.com/twiki/pub/UnidenMan4/BCD536HP/BCDx36HP_Sentinel_Version_2_05_03.zip

### How To Flash

To flash the Firmware, download the firmware to the computer.

Connect the Scanner to the computer as Mass Storage (Press "E" on the Scanner).

Copy the Firmware to the "\BCDx36HP\firmware" directory of the Scanner's memory card (for example, E:\BCDx36HP\firmware).

Wait till the copy process is done.

Safely disconnect the Scanner from the computer and wait about half a minute for the Firmware to automatically flash and for the Scanner to start working.

### Revert To Official Version

Custom Firmware doesn't change the bootloader so you can go back to the official version using [Sentinel](https://info.uniden.com/twiki/bin/view/Unidenman4/BCDx36HPSentinel) at any time. ([YouTube](https://www.youtube.com/watch?v=ypdtc7nnMfk))

