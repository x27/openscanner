# MOD firmwares

## BCD436HP_V1_99_05.bin (based on v1.99.04)
* Visual information about the mod version (boot screen)
* Output debugging information about DMR traffic.

To get debugging information, you need to turn on the scanner by pressing POWER+AVOID, 
then in the "Settings" menu in the submenu "Set Debug Log Mode" you need to select 
"SD Card(File)" or "USB (Serial)".

In addition to the debugging information provided by Uniden, I have added my debugging data.

#### DMR VOICE FRAME LOG
**Format:**
*:V0XXXXXXXXXXXXXXXXXYYYYYYYYYYYYYYYYYYZZZZZZZZZZZZZZZZZZ*

**:V0** - DMR voice frame log signature, version 0

**XXXXXXXXXXXXXXXXXX** - voice frame #0, ASCII HEX, 72bits = 9byte = 2*9 ASCII HEX symbols
**YYYYYYYYYYYYYYYYYY** - voice frame #1
**ZZZZZZZZZZZZZZZZZZ** - voice frame #2

#### DMR SYSTEM INFO LOG (and not only)
**Format:**
*:D0AAAAAAAABCDEEFGHHHHIJKLMNOOPPQQQQQQQQRRRRRRRRSSSSTTTTUUUU*

**:D0** - DMR system info log signature, version 0

**AAAAAAAA** - current frequency, ASCII DEC
**B** - DMR trunk type, 0:DMR One?, 1:DMR, 2:CAP, 4:DT3, 3:CON, 5:XPT
**C** - DMR data type
- 0: PI Header
- 1: Voice LC Header
- 2: Terminator with LC
- 3: CSBK
- 4: MBC Header
- 5: MBC Continuation
- 6: Data Header
- 7: Rate 1/2 Data
- 8: Rate 3/4 Data
- 9: Idle
- A: Rate 1 Data
- B: Unified Single Block Data
- C: Reserved for future use
- D: Reserved for future use
- E: Reserved for future use
- F: Reserved for future use

**D** - FS type
**EE** - DMR call type
**F** - TDMA ch
**G** - TDMA ch0
**HHHH** - C-CH
**I** - DMR color code
**J** - DMR superframe count (0-B)
**K** - DMR encrypt
**L** - DMR privacy 
**M** - DMR protect
**N** - EMB privacy
**OO** - EMB FID
**PP** - EMB FLCO
**QQQQQQQQ** - EMB TGID
**RRRRRRRR** - EMB UID
**SSSS** - DMR SLC LCN
**TTTT** - DMR SLC NID
**UUUU** - DMR SLC SID

This packet will be transmitted before the triad of voice frames, so some of the fields will be constant. The meaning of some variables is unknown to me, the redundancy of this is aimed at the future.

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

Allowed freq band list in 1.28.14 (in MHz):

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

Allowed freq band list in 1.28.15 (in MHz):

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

pss. patched sentinel (2.05.03) .exe file for support scanners with mod fw located here: https://mega.nz/file/NBtlRKxC#54LBK3Qiuqtsd0ZzQWZ_SfnRTqukdHuPXGChtUu5mXY

official version sentinel (2.05.03) located here: https://info.uniden.com/twiki/pub/UnidenMan4/BCD536HP/BCDx36HP_Sentinel_Version_2_05_03.zip


