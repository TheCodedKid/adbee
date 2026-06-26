# adbee

ADB-to-USB adapter. Connect a vintage Apple Desktop Bus keyboard/mouse to a
modern host over USB. A Seeed XIAO ESP32-S3 reads the single-wire ADB bus and
presents itself as a USB HID device.

![adbee](design/name.png)

## BOM

| Ref | Value | Footprint | Qty | Notes |
|-----|-------|-----------|-----|-------|
| M1 | XIAO ESP32-S3 | SeeedStudio_XIAO_ESP32S3 | 1 | MCU module, USB-C |
| J1 | MD-40SM | mini-DIN 4-pin | 1 | CUI, ADB connector |
| Q1 | BSS138 | SOT-23 | 1 | level-shift MOSFET |
| D1 | PESD5V0S1BA | SOD-323 | 1 | TVS ESD diode |
| R1 | 2.2k | 0603 | 1 | bus pull-up |
| R2 | 1k | 0603 | 1 | gate/series |
