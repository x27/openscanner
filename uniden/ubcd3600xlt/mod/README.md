# MOD firmwares

Each firmware builds upon the previous firmware (usually), so you get all the benefits of the past versions.

To get the most from the latest custom firmware you must use the [CFT program](https://github.com/x27/CFT)

All firmware versions are now posted in [releases](https://github.com/x27/openscanner/releases)

## UBCD3600XLT V1.99.42

* The mod base has been moved from official firmware 1.28.15 to 1.28.24
* Fixed bugs when debug output is enabled

## UBCD3600XLT V1.99.41

* Added P25 Phase1 AES256
* Added Scanner option: LED alert while the digital voice goes on (need any license)
* Fixed debug string D1
* Fixed MFID JVC->KEN

## UBCD3600XLT V1.99.40

* Added MFID showing

## UBCD3600XLT V1.99.38

* New RSSI calculation algo

## UBCD3600XLT V1.99.36

* Added Hytera EP encryption support (need CFT v2.0.0.36 and later)

## UBCD3600XLT V1.99.35

* !!! Fixed a serious bug, when in the presence of heterogeneous systems in the list (P25, NXDN, DMR) the required encryption row was not selected because it was discarded by the handler of another system.
* Added new Display Additional Info Item: Algo + KeyID (DEC) for display the KeyID in DEC mode (need CFT v2.0.0.35 and later)

## UBCD3600XLT V1.99.34

* Added support Caltta/Kirisun BP encryption
* Added show additional info (rssi, algo and keyid encryption). for setting need CFT 2.0.0.33 and higher
* Added Debug Logs menu item for key mapping
* Improved detection of encryption algorithms
* Encryption information is shown for a limited time (less 10s).
* DMR BP is defined by exclusion method, by residual principle.

## UBCD3600XLT V1.99.30

* Added Zip and F+Zip Key Mapping

## UBCD3600XLT V1.99.29

* Fixed floating bug KeyID in P25
* Added Activate Option: Frequency (CFT v2.0.0.30 and higher)

## UBCD3600XLT V1.99.27

* Added Tytera EP decryption
* Added Tytera BP decryption
* Added DMR AES decryption
* Added Easter Egg: 999.9999Mhz for dmr and nxdn

## UBCD3600XLT V1.99.25

* Removed band gaps (25-1300MHz)

## UBCD3600XLT V1.99.24

* Added P25 DES-OFB decryption

## UBCD3600XLT V1.99.23

* Fixing DMR processing bug (again)

## UBCD3600XLT V1.99.22

* Added P25 Phase1 ADP decryption with known key

## UBCD3600XLT V1.99.19 (based on v1.28.15)

* Fixed DMR processing bug

## UBCD3600XLT V1.99.18 (based on v1.28.15)

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
- download the latest official firmware (1.28.15) from [here](https://github.com/x27/openscanner/tree/main/uniden/ubcd3600xlt/official)
- rename the file to UBCD3600XLT_V1_28_16.BIN. This is necessary for the bootloader to accept this firmware version as the new one.
- copy to the scanner directory /BCDx36HP/FIRMWARE and reboot the scanner.
