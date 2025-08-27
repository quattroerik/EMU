[![CC BY-NC-SA 4.0][cc-by-nc-sa-shield]][cc-by-nc-sa]

# EMU – Expandable Multi-material Unit

**Introducing the EMU, the Expandable Multi-material Unit from down under.** The EMU is a modular, flexible, upgradable, reliable and service-friendly MMU designed around the proven filamentalist V3 platform.

The EMU supports any number of lanes and base configurations; whether it is a **single lane setup** to assist filament loading, a **dual lane configuration** for endless spool, or a **multi-lane, multi-box setup** for multi-material printing. It is also **expandable**, with no re-printing of parts required when upgrading from a 2 lane to a multiple lane setup.

#### Highlights:
- **Modular & Expandable** design, able to add lanes anytime and in any configuration. No reprints when upgrading from a 2 lane setup.
- **One screw or tool-free** access and servicing, even mid-print.
- **Sealed dry boxes** able to maintain humidity in the 15% range (with silica gel) or 5–8% range (with molecular sieves) for weeks.  
- **Humidity** sensors per lane for environmental monitoring.
- **Reliable endless spool** with no chance of the rewound filament interfering with neighbouring gates.
- **Off-the-shelf electronics** (EBB42 with EBB36 also fully compatible).  
- **Per-lane controls** - eject button + LEDs.

![alt text](docs/images/EMU_render.png)

## Design Objectives

#### Modularity  
Each lane is fully self-contained, so you can choose exactly how many lanes you need and group them as you like. Mix and match lanes across multiple base units, or use a stand-alone single lane for extruder loading and print assistance.

#### Upgradeability  
Expanding later is straightforward. Just print lane expanders for the base and add another dry box assembly — no need to reprint or replace existing parts when upgrading from a 2 lane base. 

#### Ease of Servicing 
All electrical and mechanical components are either one screw or completely tool-free and immediately accessible, making live troubleshooting possible even during a print.

#### Sealed Dry Boxes  
Each spool sits in its own purpose built, fully sealed dry box with an integrated desiccant holder. 
- Humidity can be maintained in the 15% range (with silica gel) or 5–8% range (with molecular sieves) for weeks.
- Opening one box doesn’t disturb its neighbours, extending effective desiccant life.

#### Integrated Humidity Sensors 
Each lane monitors its own environment, letting you know when it’s time to refresh the desiccant. Humidity sensors integrated into Mainsail (and in Home Assistant for historical data tracking via the mainsail HA integration).

#### Endless Spool Reliability
Dual pre-gate sensors and isolated spools ensure consistent run-out detection and reliable re-wind/feeding. Left over, rewound, filament interfering with neighbouring lanes is eliminated by design.  

#### Built on the Filamentalist
The lane design is based on the proven filamentalist V3 with 688 bearings, with no modifications necessary. 
- Existing 688 bearing version filamentalist parts can be reused when building an EMU.
- Optionally, the revised tensioner mount further improves pre-gate switch actuation.

#### Integrated Gate Stepper 
Each lane has its own gate stepper inside the dry box, resulting in a compact, fully self-contained mechanical design.

#### Simple Electronics
The recommended BOM uses readily available EBB42 boards (with EBB36 fully compatible). 
- MMB v2 boards can also be reused, though without humidity sensing due to I²C limitations and slightly more intricate wiring.

#### Per-lane Controls  
Each lane includes its own eject button, status LED, and a filament colour LED that illuminates the dry box. 

## BOM
BOM Link

## Assembly videos
Video links


#### This work is licensed under a
[Creative Commons Attribution-NonCommercial-ShareAlike 4.0 International License][cc-by-nc-sa].

[![CC BY-NC-SA 4.0][cc-by-nc-sa-image]][cc-by-nc-sa]

[cc-by-nc-sa]: http://creativecommons.org/licenses/by-nc-sa/4.0/
[cc-by-nc-sa-image]: https://licensebuttons.net/l/by-nc-sa/4.0/88x31.png
[cc-by-nc-sa-shield]: https://img.shields.io/badge/License-CC%20BY--NC--SA%204.0-lightgrey.svg

### License clarification regarding non-commercial use:
The non-commercial aspect of this license is for cases where EMU is the product, not the use of EMU to create products.<br/>
I.e. If you wish to sell MMU as a product, you would need to seek a commercial license before doing so. </br>
It is NOT intended to prevent the use of EMU in a printer that you use to provide commercial services. If you want to run EMU as a toolhead for your print farm printers, go right ahead.
