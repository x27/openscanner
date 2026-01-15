# MOD firmwares

Each firmware builds upon the previous firmware (usually), so you get all the benefits of the past versions.

To get the most from the latest custom firmware you must use the [CFT program](https://github.com/x27/CFT)

All firmware versions are now posted in [releases](https://github.com/x27/openscanner/releases)

## UBCD436PT V1.99.41

* Added P25 DES-OFB decryption
* Added P25 Phase1 AES256
* Added Scanner option: LED alert while the digital voice goes on (need any license)
* Fixed debug string D1
* Fixed MFID JVC->KEN

## UBCD436PT V1.99.40

* Fixed MFID showing for P25 and NXDN

## UBCD436PT V1.99.37

* No Band Gaps

## UBCD436PT V1.99.36

* Added Hytera EP encryption support (need CFT v2.0.0.36 and later)
* !!! Fixed a serious bug, when in the presence of heterogeneous systems in the list (P25, NXDN, DMR) the required encryption row was not selected because it was discarded by the handler of another system.
* Added show additional info (rssi, algo and keyid encryption). for setting need CFT 2.0.0.33 and higher
* Added support Caltta/Kirisun BP encryption
* Added Debug Logs menu item for key mapping
* Added Activate Option: Frequency (CFT v2.0.0.30 and higher)
* Fixed floating bug KeyID in P25
* Added Tytera EP decryption
* Added Tytera BP decryption
* Added DMR AES decryption
* Added easter egg: 999.9999Mhz for dmr and nxdn
* Added new Display Additional Info Item: Algo + KeyID (DEC) for display the KeyID in DEC mode (need CFT v2.0.0.35 and later)

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
