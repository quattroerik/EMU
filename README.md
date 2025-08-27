[![CC BY-NC-SA 4.0][cc-by-nc-sa-shield]][cc-by-nc-sa]

# EMU – Expandable Multi-material Unit
### A new take on a MMU by <a href="https://github.com/DW-Tas">DW-Tas</a> and <a href="https://github.com/igiannakas">igiannakas</a><br/>
<a href="https://ko-fi.com/O5O5OCC0K"><img src="docs/images/Ko-fi_smol.png"> Ko-Fi</a>


> [!WARNING] 
> ***Under Active/Early Development*** <br/>
> Build at your own risk

**Introducing the EMU, the Expandable Multi-material Unit from down under.** The EMU is a modular, flexible, upgradable, reliable and service-friendly MMU designed around the proven filamentalist V3 platform.

The EMU supports any number of lanes and base configurations; whether it is a **single lane setup** to assist filament loading, a **dual lane configuration** for endless spool, or a **multi-lane, multi-box setup** for multi-material printing. It is also **expandable**, with no re-printing of parts required when upgrading from a 2 lane to a multiple lane setup.

<p align="center">
  <img src="docs/images/EMU_multi_lane_unit.png" width="100%">
</p>

#### Highlights:
- **Modular & Expandable** design, able to add lanes anytime and in any configuration. No reprints when upgrading from a 2 lane setup.
- **One screw or tool-free** access and servicing, even mid-print.
- **Sealed dry boxes** able to maintain humidity in the 15% range (with silica gel) or 5–8% range (with molecular sieves) for weeks.  
- **Humidity** sensors per lane for environmental monitoring.
- **Reliable endless spool** with no chance of the rewound filament interfering with neighbouring gates.
- **Off-the-shelf electronics** (EBB42 with EBB36 also fully compatible).  
- **Per-lane controls** - eject button + LEDs.

<p align="center">
  <img src="docs/images/EMU_single_lane_unit_front.png" width="49%">
  <img src="docs/images/EMU_two_lane_unit_front.png" width="49%">
</p>


## Design Objectives

#### Modularity & Upgradeability  
Each lane is fully self-contained, so you can choose **exactly how many lanes you need and group them as you like**. You can also **mix and match** lanes across multiple base units, or use a stand-alone single lane for extruder loading and print assistance. 

Expanding later is also straightforward. Just print lane expanders for the base and add another dry box assembly. There is no need to reprint or replace existing parts when upgrading from a 2 lane base. 

#### Ease of Servicing 
All electrical and mechanical components are either **one screw or completely tool-free and immediately accessible**, making live troubleshooting possible even during a print. 

Access to the electronics is easy - just lift the dry box off its base for full access. The gate stepper tensioning screw is accessible without any dissassembly allowing on the fly tuning of gate tension. Finally, removing the filamentalist, stepper and stepper assembly is possible via one screw.

#### Sealed Dry Boxes  
Each spool sits in its own purpose built, **fully sealed dry box with an integrated desiccant holder**. The boxes use foam cord in areas of potential air ingress to create a tight seal, with the clear 1.5mm PETG/PC panel also offering visibility inside the dry box.

The dry boxes can maintain humidity in the 15% range (with silica gel) or 5–8% range (with molecular sieves) for weeks. Finally, as each dry box is self contained, opening one to reload filament, doesn’t disturb its neighbours, extending the effective desiccant life.

<p align="center">
  <img src="docs/images/EMU_single_lane_unit_open.png" width="90%">
</p>

#### Integrated Humidity Sensors 
Each lane monitors its own environment, letting you know when it’s **time to refresh the desiccant**. The humidity sensors are integrated into Mainsail (and optionally in Home Assistant for historical data tracking via the mainsail HA integration).

#### Endless Spool Reliability
Dual pre-gate sensors ensure **consistent run-out detection** and reliable re-wind, as the filament is always gripped by the gate hobbed gear assembly. 

In addition, the isolated boxes ensure that any left over, rewound, filament cannot interfere with neighbouring lanes, **preventing a jam**.

#### Built on the Filamentalist
The lane assembly is based on the proven **filamentalist V3 design with 688 bearings**, with no modifications necessary. 
- Existing 688 bearing version filamentalist parts can be reused when building an EMU.
- Optionally, the revised tensioner mount further improves pre-gate switch actuation.
- Wide spool size compatibility - built on the 74mm filamentalist stock setup and fits even KVP filament spools.

<p align="center">
  <img src="docs/images/EMU_integrated_gate_unit_close_up.png" width="49%">
  <img src="docs/images/EMU_integrated_gate_unit.png" width="49%">
</p>

#### Integrated Gate Stepper 
Each lane has its own gate stepper inside the dry box, resulting in a compact, **fully self-contained mechanical design**. In case of mechanical issue, you can swap out filamentalist assemblies with 3 screws, unplugging 2 JST plugs and unplugging the bowden tube. 

In addition, you can **swap out complete dry boxes** by unplugging two JST plugs and the bowden tube. This is helpful if you want to maintain a particularly moisture sensitive filament undisturbed when swapping it out from the EMU.

#### Simple Electronics
The recommended BOM uses **readily available EBB42 boards** (with EBB36 fully compatible). MMB v2 boards can also be reused, though without humidity sensing due to I²C limitations and a slightly more intricate wiring.

In addition, **each lane has its own ventilation fan**, ensuring the stepper drivers do not overheat, even when the unit is placed on top of a hot printer. With the EBB42 and EBB36, the ventilation fans can also be speed controlled to minimize noise.

#### Easy mounting
The EMU base assembly can be securely **mounted on extrusions** or using **rubber feet** directly on the printer or besides it. In either case the **electronics remain accessible** without needing to remove the unit from its mounts.

#### Per-lane Controls  
Each lane includes its own eject button, status LED, and a filament colour LED that illuminates the dry box. 

## BOM
ToDo: BOM Link

## Assembly videos
ToDo: Video links


#### This work is licensed under a
[Creative Commons Attribution-NonCommercial-ShareAlike 4.0 International License][cc-by-nc-sa].

[![CC BY-NC-SA 4.0][cc-by-nc-sa-image]][cc-by-nc-sa]

[cc-by-nc-sa]: http://creativecommons.org/licenses/by-nc-sa/4.0/
[cc-by-nc-sa-image]: https://licensebuttons.net/l/by-nc-sa/4.0/88x31.png
[cc-by-nc-sa-shield]: https://img.shields.io/badge/License-CC%20BY--NC--SA%204.0-lightgrey.svg

### License clarification regarding non-commercial use:
The non-commercial aspect of this license is for cases where EMU is the product, not the use of EMU to create products.<br/>
I.e. If you wish to sell EMU as a product, you would need to seek a commercial license before doing so. </br>
It is NOT intended to prevent the use of EMU with a printer that you use to provide commercial services. If you want to run EMU in your print farm, go right ahead.
