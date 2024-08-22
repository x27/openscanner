# MOD firmwares

Each firmware builds upon the previous firmware (usually), so you get all the benefits of the past versions.

To get the most from the latest custom firmware you must use the [CFT program](https://github.com/x27/CFT)

All firmware versions are now posted in [releases](https://github.com/x27/openscanner/releases)

## UBCD436PT V1.99.23 (based on v1.99.22)

* Added P25 DES-OFB decryption

## UBCD436PT V1.99.22 (based on v1.99.18)

* Added P25 Phase1 ADP decryption with known key

## UBCD436PT V1.99.18 (based on v1.23.02)

* Release first test firmware

### How To Flash

To flash the Firmware, download the firmware to the computer.

Connect the Scanner to the computer as Mass Storage (Press "E" on the Scanner).

Copy the Firmware to the "\BCDx36HP\firmware" directory of the Scanner's memory card (for example, E:\BCDx36HP\firmware).

Wait till the copy process is done.

Safely disconnect the Scanner from the computer and wait about half a minute for the Firmware to automatically flash and for the Scanner to start working.

### Revert To Official Version

Custom Firmware doesn't change the bootloader so you can go back to the official version.

Since custom firmware does not change the internal version number, you can go back to the official firmware as follows:
- download the latest official firmware (1.23.02) from [here](https://github.com/x27/openscanner/tree/main/uniden/ubcd436pt/official)
- rename the file to UBCD436-PT_V1_23_03.BIN. This is necessary for the bootloader to accept this firmware version as the new one.
- copy to the scanner directory /BCDx36HP/FIRMWARE and reboot the scanner.
