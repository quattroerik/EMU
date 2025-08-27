[![CC BY-NC-SA 4.0][cc-by-nc-sa-shield]][cc-by-nc-sa]

# EMU – Expandable Multi-material Unit

**Introducing the EMU, the Expandable Multi-material Unit from down under.** The EMU is a modular, upgradable, and service-friendly MMU designed around the proven filamentalist V3 platform.  

The EMU is built for flexibility, reliability, and ease of use. Whether you want a single lane to assist loading or a multi-lane setup for true multi-material printing, the EMU is able to easily grow with your needs and is modular to support any number of lane and base combinations.

- 🧩 Modular. Add lanes anytime, no reprints  
- 🌫️ Sealed dry boxes maintain 5–8% humidity  
- 📡 Humidity + filament sensors per lane  
- 🔧 Tool-free servicing, even mid-print  
- 🔌 Off-the-shelf electronics (EBB42/36)  
- 💡 Per-lane eject + LEDs

![alt text](docs/images/EMU_render.png)

## Design Objectives

#### Modularity  
Each lane is fully self-contained, so you can choose exactly how many lanes you need and group them however you like.  
- Mix and match any number of lanes across multiple base units.  
- Use of a stand-alone, single lane for extruder loading and print assistance is also possible.  

#### Upgradeability  
Expanding later is straightforward. Just print lane expanders for the base and add another dry box assembly. No need to reprint or replace existing parts.  

#### Ease of Servicing  
All electrical and mechanical components have tool-free or one screw access, making them immediately accessible. Live troubleshooting is possible even during a print.  

#### Sealed Dry Boxes  
Each spool sits in its own fully enclosed dry box with an integrated desiccant holder.  
- Humidity can be maintained in the 5–8% range for weeks.  
- Opening one box doesn’t disturb its neighbours, extending desiccant life.  

#### Integrated Humidity Sensors  
Each lane monitors its own environment, letting you know when it’s time to refresh the desiccant. Humidity sensors integrated into Mainsail (and in Home Assistant for historical data tracking via the mainsail HA integration).

#### Endless Spool Reliability  
Dual pre-gate sensors and isolated spools ensure consistent run-out detection and reliable re-wind/feeding. No risk of the left over filament interfering with neighbouring lanes.  

#### Built on the Filamentalist  
The lane design is based on the proven Filamentalist V3. Existing filamentalist parts can be reused when building an EMU.  

#### Integrated Gate Stepper  
Each lane has its own gate stepper inside the dry box, resulting in a compact, fully self-contained design.  

#### Simple Electronics  
The recommended BOM uses readily available components:  
- **EBB42** boards (recommended)  
- **EBB36** boards (fully compatible)  
- **MMB v2** boards (compatible, but humidity sensing not supported due to I²C limitations)  

#### Per-lane Controls  
Each lane includes:  
- Eject button  
- Status LED  
- Filament colour LED that illuminates the filament in the dry box  

## BOM
<<Bom link....>>

## Assembly videos
<<Video links....>>


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
