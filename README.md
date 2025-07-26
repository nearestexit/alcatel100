# alcatel100

Custom keyboard designed to use the GMK keycaps from the [Alcatel-Lucent MMK](https://deskthority.net/viewtopic.php?t=23887).
Designed in Onshape and KiCad.
Powered by [QMK](https://github.com/qmk/qmk_firmware).

![Front](https://github.com/nearestexit/alcatel100/blob/main/Pictures/Main.JPG)

## Overview
The Alcatel MMK has a beautiful set of keycaps, but the Enter, Backspace, and Right Shift are 0.25u shorter than normal. They are rarely, if ever, used on customs.
The keycaps were originally made by Cherry, but later GMK took over production.

![Front](https://github.com/nearestexit/alcatel100/blob/main/Pictures/Front.JPG)

I designed this for fun. It is not an entry-level keyboard, and it is not intended for a Group Buy.
I'm sharing the production and source files with the goal of serving as a reference for other designers.

![combo2](https://github.com/nearestexit/alcatel100/blob/main/Pictures/combo2.png)

## Design Goals
- Box-on-wedge with seamless sides all around, including the back
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
| Ribbon Cable | 1 | https://www.digikey.com/en/products/detail/molex/0151660207/3281088 |
| 3M SJ5302 | 4  | https://www.3m.com/3M/en_US/p/d/b5005035183/ |
| Unified Daughterboard  | 1  | https://cannonkeys.com/products/unified-daughterboard-and-jst-cable |
| M2.5x0.45x8mm SHCS | 6  | https://www.mcmaster.com/91292A012/ |
| 10cm Molex to JST Cable | 1 | https://cannonkeys.com/products/unified-daughterboard-and-jst-cable |
| M2.5x0.45x16mm SHCS | 1 | https://www.mcmaster.com/91292A018/ |
| M2.5x0.45x20mm SHCS | 6 | https://www.mcmaster.com/91292A019/ |
| M2x0.4x4mm SHCS | 10 | https://www.mcmaster.com/91292A005/ |
| M3x0.5x6mm Countersunk Screw | 5 | https://www.mcmaster.com/92125A126/ |
| M3x0.5x8mm Countersunk Screw | 8 | https://www.mcmaster.com/92125A128/ |

## Backlight

Each lock light is controlled by a separate pin and has a fixed brightness. The remainder of the windowed keys are all on the same PWM dimmable circuit.
I used [these LEDs](https://www.digikey.com/en/products/detail/american-bright-optoelectronics-corporation/BL-B8141-TRS20A/22486924), which have a nice color, but MX LEDs are actually supposed to be 3mm *flangeless* LEDs. These LEDs are *flanged* 3mm. I had to clip off all the flanges (not fun).

![backlight](https://github.com/nearestexit/alcatel100/blob/main/Pictures/backlight.JPG)

## Firmware

A QMK .bin file is provided for flashing, as well as QMK source files. I can port it to Vial upon request.

## Credits

Everyone in the Keyboard Atelier who has helped me over the past 2 years.

![bottom](https://github.com/nearestexit/alcatel100/blob/main/Pictures/backlight2.JPG)