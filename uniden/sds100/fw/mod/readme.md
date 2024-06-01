# MOD firmwares

To get the most from the latest custom firmware you must use the [CFT program](https://github.com/x27/CFT)

All firmware versions are now posted in [releases](https://github.com/x27/openscanner/releases)

##  SDS-100 V1.99.17 (based on v1.99.16)

* Fixed problem in DMR/Simplex mode when KeyID is set because the scanner does not catch PI HEADER in this mode.

## SDS-100 V1.99.16 (based on v1.99.14)

* Added Motorola EP (Enhanced Privacy) decryption

## SDS-100 v1.99.14 (based on v1.99.11)

* Added NXDN Scrambler decryption

## SDS-100 v1.99.10 (based on v1.23.07)

* Add Hytera BP (Basic Privacy) and Motorola BP (Basic Privacy) decryption with known key
* Now "Set Debug Log Mode" submenu always enabled in the "Settings" menu
* Visual information about the mod version (boot screen)
* Output debugging information about DMR traffic

https://github.com/x27/openscanner/releases/tag/SDS100_1.99.10

## SDS-100 v1.99.02 (based on v1.23.03)

- DPMR in SDS100 now

ps. inside fw version is not changed

### How To Flash

To flash the Firmware, download the firmware to the computer.

Connect the Scanner to the computer as Mass Storage (Press "E" on the Scanner).

Copy the Firmware to the "\BCDx36HP\firmware" directory of the Scanner's memory card (for example, E:\BCDx36HP\firmware).

Wait till the copy process is done.

Safely disconnect the Scanner from the computer and wait about half a minute for the Firmware to automatically flash and for the Scanner to start working.

### Revert To Official Version

Custom Firmware doesn't change the bootloader so you can go back to the official version.

Since custom firmware does not change the internal version number, you can go back to the official firmware as follows:
- download the latest official firmware (1.23.07) from [here](https://github.com/x27/openscanner/tree/main/uniden/sds100/fw/official)
- rename the file to SDS-100_V1_23_08.BIN. This is necessary for the bootloader to accept this firmware version as the new one.
- copy to the scanner directory /BCDx36HP/FIRMWARE and reboot the scanner.
