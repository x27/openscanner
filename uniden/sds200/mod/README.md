# MOD firmwares

To get the most from the latest custom firmware you must use the [CFT program](https://github.com/x27/CFT)

All firmware versions are now posted in [releases](https://github.com/x27/openscanner/releases)

## SDS200 V1.99.28 (based on v1.99.27)

* Removed Band Gaps. 25-1300 MHz now.
* Fixed KeyID bug in P25

## SDS200 V1.99.27 (based on v1.99.23)

* Added Tytera EP decryption
* Added Tytera BP decryption
* Added DMR AES decryption
* Added Easter Egg: 999.9999Mhz for dmr and nxdn

## SDS200 V1.99.23 (based on v1.99.22)

* Added P25 DES-OFB decryption

## SDS200 V1.99.22 (based on v1.99.18)

* Added P25 Phase1 ADP decryption with known key
  
## SDS200 V1.99.18 (based on v1.23.07)

* Initial release

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
- download the latest official firmware (1.23.07) from [here](https://github.com/x27/openscanner/tree/main/uniden/sds200/official)
- rename the file to SDS200_V1_23_08.BIN. This is necessary for the bootloader to accept this firmware version as the new one.
- copy to the scanner directory /BCDx36HP/FIRMWARE and reboot the scanner.
