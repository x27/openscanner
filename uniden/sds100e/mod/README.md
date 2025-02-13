# MOD firmwares

To get the most from the latest custom firmware you must use the [CFT program](https://github.com/x27/CFT)

All firmware versions are now posted in [releases](https://github.com/x27/openscanner/releases)

## SDS100E V1.99.41

* Added P25 Phase1 AES256
* Added Scanner option: LED alert while the digital voice goes on (need any license)
* Fixed debug string D1
* Fixed MFID JVC->KEN

## SDS100E V1.99.40

* Fixed MFID showing for P25 and NXDN

## SDS100E V1.99.36

* Added Hytera EP encryption support (need CFT v2.0.0.36 and later)

## SDS100E V1.99.35

* !!! Fixed a serious bug, when in the presence of heterogeneous systems in the list (P25, NXDN, DMR) the required encryption row was not selected because it was discarded by the handler of another system.
* Added new Display Additional Info Item: Algo + KeyID (DEC) for display the KeyID in DEC mode (need CFT v2.0.0.35 and later)
* Added support Caltta/Kirisun BP encryption
* Replaced "USB2 Voltage" by "Algo + KeyID" optional display item
* Added Debug Logs menu item for key mapping

## SDS100E V1.99.31

* Fixed Zip key mapping

## SDS100E V1.99.30

* Added Zip and F+Zip Key Mapping

## SDS100E V1.99.28

* Removed Band Gaps. 25-1300 MHz now.
* Fixed KeyID bug in P25

## SDS100E V1.99.27

* Added Tytera EP decryption
* Added Tytera BP decryption
* Added DMR AES decryption
* Added Easter Egg: 999.9999Mhz for dmr and nxdn

## SDS100E V1.99.23 (based on v1.99.22)

* Added P25 DES-OFB decryption

## SDS100E V1.99.22 (based on v1.99.18)

* Added P25 Phase1 ADP decryption with known key

## SDS100E V1.99.18 (based on v1.23.09)

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
- download the latest official firmware (1.23.09) from [here](https://github.com/x27/openscanner/tree/main/uniden/sds100e/official)
- rename the file to SDS100E_V1_23_10.BIN. This is necessary for the bootloader to accept this firmware version as the new one.
- copy to the scanner directory /BCDx36HP/FIRMWARE and reboot the scanner.
