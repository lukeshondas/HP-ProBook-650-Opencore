# HP-ProBook-650-Opencore
## Overview

This EFI works perfectly and natively on Mac OS 12 `Monterey` and works fine with [OCLP patching](https://github.com/dortania/OpenCore-Legacy-Patcher) on Mac OS 13 `Ventura` Mac OS 14 `Sonoma` and Mac OS 15 `Sequoia`.


## Specs

| Part             | Description                                                                                                    |
| ---------------- | -------------------------------------------------------------------------------------------------------------- |
| CPU              | Intel® Core™ i5-4210M Processor (will work on core i7 variants too)                                            |
| iGPU             | Intel® HD 4600                                                                                                  |
| Memory           | 8Gb (2 x 8Gb 1600MHz) (will work fine with 8gb+)                                                               |
| Storage          | SSD 256gb                                                                                                      |
| Display          | 15.6 inch 1366x768 TN Panel (1080p display's work fine on this machine)                                        |
| Wifi & Bluetooth | Intel® Centrino Advanced-N 6235                                                                                |
| LAN              | Intel® Gigabit Ethernet, 10/100/1000                                                                           |
| Audio            | IDT                                                                                                 |
| External ports   | 5 x USB 3.0, 1 x Ethernet, 1 x SD Card Reader, 1 x Displayport, 1 x 3.5 headphone/microphone combo, 1 x VGA    |

### Working and Not Working

|                                                   | Status | Note                              |
| ------------------------------------------------- | ------ | ----------------------------------|
| Keyboard (with volume keys and brightness control keys) | ✅     |                                   |
| Touchpad with all gestures and buttons            | ✅     |                                   |
| Ethernet                                          | ✅     |                                   |
| Wifi                                              | ✅     |Intel only with [Heliport](https://github.com/OpenIntelWireless/HeliPort) on Sequoia|
| Bluetooth                                         | ✅     |                                   |
| SD Card Reader                                    | ✅     |Monterey only for now              |
| Camera & Mic                                      | ✅     |                                   |
| Speaker & 3.5mm audio port                        | ✅     |                                   |
| iGPU                                              | ✅     |Needs GPU patching with [OCLP](https://github.com/dortania/OpenCore-Legacy-Patcher) on anything newer than Monterey                                   |
| VGA & Displayport                                 | ❌     |Displayport Crashes when connected, I'll try fix when I can         |
| USB                                               | ✅     |                                   |
| Sleep                                             | ✅     |                                   |
| Handoff                                           | ❌     |                                   |
| Airdrop                                           | ❌     |                                   |


## Usage

Make sure to have your bios set to UEFI <b>with CSM</b> and VRAM set to 64MB

Download my EFI, Change your Serial with [GenSMBIOS](https://github.com/corpnewt/GenSMBIOS) and install.

If installing Sequoia to use Intel wifi you'll need to download [Heliport](https://github.com/OpenIntelWireless/HeliPort)
