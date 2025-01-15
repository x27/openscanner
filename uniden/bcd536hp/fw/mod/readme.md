# MOD firmwares

To get the most from the latest custom firmware you must use the [CFT program](https://github.com/x27/CFT)

All firmware versions are now posted in [releases](https://github.com/x27/openscanner/releases)

## BCD536HP V1.99.41

* Added P25 Phase1 AES256
* Added Scanner option: LED alert while the digital voice goes on (need any license)
* Fixed debug string D1
* Fixed MFID JVC->KEN

## BCD536HP V1.99.40

* Fixed MFID showing for P25 and NXDN

## BCD536HP V1.99.38

* New RSSI calculation algo
* Changed Replay Duration from 240 to 600 sec

## BCD536HP V1.99.35

* !!! Fixed a serious bug, when in the presence of heterogeneous systems in the list (P25, NXDN, DMR) the required encryption row was not selected because it was discarded by the handler of another system.
* Added new Display Additional Info Item: Algo + KeyID (DEC) for display the KeyID in DEC mode (need CFT v2.0.0.35 and later)

## BCD536HP V1.99.34

* Added support Caltta/Kirisun BP encryption
* Added show additional info (rssi, algo and keyid encryption). for setting need CFT 2.0.0.33 and higher
* Added Debug Logs menu item for key mapping
* Improved detection of encryption algorithms
* Encryption information is shown for a limited time (less 10s).
* DMR BP is defined by exclusion method, by residual principle.

## BCD536HP V1.99.32

* Fixed RANGE key mapping

## BCD536HP V1.99.29

* Fixed floating bug KeyID in P25
* Added Activate Option: Frequency (CFT v2.0.0.30 and higher)

## BCD536HP V1.99.23

* Added P25 DES-OFB decryption

## BCD536HP V1.99.22

* Added P25 Phase1 ADP decryption with known key

## BCD536HP V1.99.18

* Added support for Anytone Encryption (Test)

## BCD536HP V1.99.17

* Fixed problem in DMR/Simplex mode when KeyID is set because the scanner does not catch PI HEADER in this mode.

## BCD536HP V1.99.16

* Added Motorola EP (Enhanced Privacy) decryption

## BCD536HP V1.99.14

* Added NXDN Scrambler decryption

This can be configured in the CFT program

https://github.com/x27/openscanner/releases/tag/BCD536HP_1.99.11

## BCD536HP V1.99.11

* Add Zip Key Assignment

This can be configured in the CFT program

https://github.com/x27/openscanner/releases/tag/BCD536HP_1.99.11

## BCD536HP V1.99.10

* Add Hytera BP (Basic Privacy) and Motorola BP (Basic Privacy) decryption with known key
* Now "Set Debug Log Mode" submenu always enabled in the "Settings" menu
* Visual information about the mod version (boot screen)
* Output debugging information about DMR traffic.

https://github.com/x27/openscanner/releases/tag/BCD536HP_1.99.10

## BCD536HP_V1_99_04.bin

Fix: Show extended Net/System/Site/TG info for any custom name

Description of the problem: https://forums.radioreference.com/threads/custom-search-bcd436hp.343396/

Video of the problem: https://www.youtube.com/watch?v=j64LAJJox2Y

## BCD536HP_V1_99_03.bin (based on v1.28.16)

* Unmute when received all encrypted traffic
* Removed gaps on bands

## BCD536HP_V1_99_02.bin (based on v1.28.16)

* Unmute when received all encrypted traffic

## BCD536HP_V1_28_17.bin

* Removed gaps on bands (based on BCD536HP 1.28.16)

Allowed freq band list in 1.28.16 (in MHz):

- 25.0000 - 53.9999
- 54.0000 - 107.9999
- 108.0000 - 136.9999
- 137.0000 - 150.8149
- 150.8150 - 154.6250
- 154.6251 - 199.9999
- 200.0000 - 224.9999
- 225.0000 - 272.9999
- 273.0000 - 319.9999
- 320.0000 - 387.9999
- 388.0000 - 512.0000
- 758.0000 - 805.9999
- 806.0000 - 823.9875
- 849.0000 - 868.9875
- 894.0000 - 960.0000
- 1240.0000 - 1300.0000 

Allowed freq band list in 1.28.17 (in MHz):

- 25.0000 - 53.9999
- 54.0000 - 107.9999
- 108.0000 - 136.9999
- 137.0000 - 150.8149
- 150.8150 - 154.6250
- 154.6251 - 199.9999
- 200.0000 - 224.9999
- 225.0000 - 272.9999
- 273.0000 - 319.9999
- 320.0000 - 387.9999
- 388.0000 - 639.9999
- 640.0000 - 805.9999
- 806.0000 - 848.9999
- 849.0000 - 893.9999
- 894.0000 - 1099.9999
- 1100.0000 - 1300.0000 

ps. inside fw version is not changed

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

Custom Firmware doesn't change the bootloader so you can go back to the official version.

Since custom firmware does not change the internal version number, you can go back to the official firmware as follows:
- download the latest official firmware (1.28.16) from [here](https://github.com/x27/openscanner/tree/main/uniden/bcd536hp/fw/official)
- rename the file to BCD536HP_V1_28_17.BIN. This is necessary for the bootloader to accept this firmware version as the new one.
- copy to the scanner directory /BCDx36HP/FIRMWARE and reboot the scanner.
