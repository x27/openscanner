# MOD firmwares

To get the most from the latest custom firmware you must use the [CFT program](https://github.com/x27/CFT)

## SDS-100_V1_99_10.bin (based on v1.23.07)

* Add Hytera BP (Basic Privacy) and Motorola BP (Basic Privacy) decryption with known key
* Now "Set Debug Log Mode" submenu always enabled in the "Settings" menu
* Visual information about the mod version (boot screen)
* Output debugging information about DMR traffic

https://github.com/x27/openscanner/releases/tag/SDS100_1.99.10

## SDS-100_V1_99_02.bin (based on v1.23.03)

- DPMR in SDS100 now

ps. inside fw version is not changed

### How To Flash

To flash the Firmware, download the firmware to the computer.

Connect the Scanner to the computer as Mass Storage (Press "E" on the Scanner).

Copy the Firmware to the "\BCDx36HP\firmware" directory of the Scanner's memory card (for example, E:\BCDx36HP\firmware).

Wait till the copy process is done.

Safely disconnect the Scanner from the computer and wait about half a minute for the Firmware to automatically flash and for the Scanner to start working.

### Revert To Official Version

Custom Firmware doesn't change the bootloader so you can go back to the official version using [Sentinel](https://info.uniden.com/twiki/bin/view/Unidenman4/BCDx36HPSentinel) at any time. ([YouTube](https://www.youtube.com/watch?v=ypdtc7nnMfk))
