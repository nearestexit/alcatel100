# alcatel100

Custom keyboard designed to use the keycaps from the Alcatel-Lucent MMK, manufactured by GMK.
Designed in Onshape and KiCad.
Powered by [QMK](https://github.com/qmk/qmk_firmware).

![Front](https://github.com/nearestexit/alcatel100/blob/main/Pictures/Front.JPG)


## Overview
A fullsize keyboard that utilizes the Cherry-profile keycaps made for the [Alcatel-Lucent MMK](https://deskthority.net/viewtopic.php?t=23887).
The Enter, Backspace, and Right Shift are 0.25u shorter than a normal keyboard, necessitating a keyboard designed specifically for them.

Complete, tested production files are provided in this repository. However, I mostly intend this to serve as a reference for others to design their own keyboards.

![Back](https://github.com/nearestexit/alcatel100/blob/main/Pictures/back.JPG)

## Design Goals
- OTD 356-style box on wedge with seamless sides all around, including the back
- Left half of the keyboard isolated from the right half
- Single-color PWM-dimmable backlight
- Uniform 4.8mm bezels

**Case Source (Onshape):** https://cad.onshape.com/documents/5081b96c77523c56bb0f8f6b/w/91dc47074a8fd3b0ca2e25d0/e/6e8ed4262c52380f9f8bfe9b

![Combo](https://github.com/nearestexit/alcatel100/blob/main/Pictures/combo.png)

## PCB
The PCB supports both configurations of split right shift, and also split numpad enter. Unfortunately, after the PCB was manufactured, I discovered that the Cherry version of the keyset has a 6.25u spacebar that only has an offset stem, while the GMK version of the keyset has a 6.25u spacebar that supports both centered and offset stems. The PCB and bottom case only support the centered stem location.
I ordered a single bare PCB from EuroCircuits and hand-soldered the components, so I do not have JLCPCB production files available.

![PCB](https://github.com/nearestexit/alcatel100/blob/main/Pictures/PCB.JPG)

## Bill of Materials

| Item  | Quantity | Link |
| ------------- | ------------- | ------------- | 
| 3M SJ5302 | 4  | https://www.3m.com/3M/en_US/p/d/b5005035183/ |
| Unified Daughterboard  | 1  | https://cannonkeys.com/products/unified-daughterboard-and-jst-cable |
| M2.5x0.45x8mm SHCS | 6  | https://www.mcmaster.com/91292A012/ |
| 10cm Molex to JST Cable | 1 | https://cannonkeys.com/products/unified-daughterboard-and-jst-cable |
| M2.5x0.45x16mm SHCS | 1 | https://www.mcmaster.com/91292A018/ |
| M2.5x0.45x20mm SHCS | 6 | https://www.mcmaster.com/91292A019/ |
| M2x0.4x4mm SHCS | 10 | https://www.mcmaster.com/91292A005/ |
| M3x0.5x6mm Countersunk Screw | 5 | https://www.mcmaster.com/92125A126/ |
| M3x0.5x8mm Countersunk Screw | 8 | https://www.mcmaster.com/92125A128/ |

The tolerances around the heads of the screws are very tight. Using hardware with dimensions that do not match these McMaster parts may have unintended consequences.

![backlight](https://github.com/nearestexit/alcatel100/blob/main/Pictures/backlight.JPG)

![bottom](https://github.com/nearestexit/alcatel100/blob/main/Pictures/bottom.JPG)