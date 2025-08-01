# RealBattery Recharged

**RealBattery Recharged** is a complete overhaul of the stock electric system in Kerbal Space Program, originally designed by Blackliner. 
It brings a more realistic and engaging battery simulation, adding depth to spacecraft design and power management without overcomplicating gameplay.

## Features

*RealBattery Recharged* replaces the simplistic stock EC storage system with a more nuanced model: batteries **store energy** (StoredCharge) and **supply power** (ElectricCharge) up to their rated capacity.  
Discharge and recharge occur dynamically based on system demand, charge level, and efficiency.

Each battery reports its energy/power density, charge/discharge efficiency, current state (Idle / Charging / Discharging), and more.  
The new system rewards thoughtful planning, buffering for peak loads, and progressive tech improvements.

### This mod includes:
- A dynamic battery module applied to all parts containing ElectricCharge
- Realistic simulation of power (kW) and energy (kWh), based on internal capacity and output limits
- Discharge and recharge mechanics with efficiency losses and power buffering
- A range of battery chemistries inspired by real-world technologies
- Tech-tree progression with unlockable battery upgrades per part
- Seamless integration with B9PartSwitch and localization support
- Optional language files to rename ElectricCharge and StoredCharge

> See also the [Changelog](https://github.com/Rjoande/RealBattery/blob/master/RealBattery/Changelog.md) for a list of newly-released features.

### Extras
Optional patches are included in the release to enhance immersion and realism. Extra patches are modular and can be removed or disabled if undesired:

- **Alternator Fix**: disables alternators on most rocket engines (for realism), but enables them on multi-mode engines like the *RAPIER*.
- **EC-to-current** and **EC-to-kW** localization packs: rename Electric Charge to *Electric Current*, or alternatively to *kW/kWh* (replacing EC/SC with power units). *Only install one at a time!* See the [wiki](https://github.com/Rjoande/RealBattery/wiki/Understanding-EC-and-SC-Units) for details.
- **Electric-pump-fed Engines**: the *Goldfish* and *Angora* engines from [Near Future Launch Vehicles](https://github.com/post-kerbin-mining-corporation/NearFutureLaunchVehicles/releases) now require electric charge to operate.
- **Fuel Cell Output**: fuel cells internal buffer aligns with actual electrical output.

To install an extra, simply place the corresponding patch into your `GameData` folder. See the `Extras/` folder in the release package for details.

## Planned Features

Several improvements and expansions are planned for future updates:

- [x] Adjustable settings in the difficulty menu
- [x] Ability to manually enable/disable individual batteries
- [x] Background simulation support for unloaded vessels
- [x] Battery obsolescence system (degradation over time)
- [x] Self-discharge for inactive batteries
- [x] Thermal behavior (heat production and damage with [SystemHeat](https://github.com/post-kerbin-mining-corporation/SystemHeat) compatibility)
- [ ] Fix battery stats not updating correctly when switching subtypes in the editor
- [ ] Refine background simulation for improved accuracy and broader compatibility with third-party modules  
- [ ] Add texture switching support for stock and stockalike battery parts  
- [ ] Create a custom KSPedia page for in-game documentation

Suggestions and contributions are welcome! See the [Contributing](#contributing) section below.

## Dependencies

### Required:
- [Module Manager](https://github.com/sarbian/ModuleManager/releases)
- [B9PartSwitch](https://github.com/blowfishpro/B9PartSwitch/releases)
- [Community Resource Pack](https://github.com/UmbraSpaceIndustries/CommunityResourcePack/releases)
- [SystemHeat](https://github.com/post-kerbin-mining-corporation/SystemHeat/releases)

### Suggested:
- [Community Tech Tree](https://github.com/post-kerbin-mining-corporation/CommunityTechTree/releases)
- [System Monitor (Dynamic Battery Storage)](https://github.com/post-kerbin-mining-corporation/DynamicBatteryStorage/releases)
- [DangIt! Continued](https://github.com/linuxgurugamer/DangIt/releases)


## Installation

1. Remove any previous `RealBattery` install.
3. Download the latest release from the [Releases](https://github.com/Rjoande/RealBattery/releases) page.
2. Extract into your `GameData` folder.
4. Ensure [dependencies](#dependencies) are installed.
5. (Optional) Install the [extras](#extras) as you like.

> Starting a new save is recommended to enjoy the full tech progression. Installing mid-career is possible, but may affect in-flight vessels' power and mass balance.

## External Mod Compatibility

RealBattery Recharged dynamically applies to any part with ElectricCharge, including most modded parts.  
Known compatibility or special support includes:

- Airplane Plus
- Planetside Exploration Technologies
- Artemis Construction Kit
- Shuttle Orbiter Construction Kit
- Buran Orbiter Construction Kit
- Bluedog Design Bureau
- HabTech 2
- Knes
- Mk3 Expansion
- Near Future Technologies
- OPT Spaceplane Continued
- reDIRECT
- Restock+
- Starship Expansion Project 
- Stockalike Station Parts Redux
- Tantares
- Tundra Exploration 
- Universal Storage II

> Parts from mods not listed above still benefit from RealBattery’s automatic patching system. These will receive a default, generic set of subtypes. A number of third-party modules is also supported for background simulation. This includes *SystemHeat, CryoTanks, Near Future Tech, SpaceDust, SCANsat, Snacks*. Future updates will include more mods and modules.

## Contributing

Pull requests, translations, and feedback are welcome!  
Please fork the repository and submit a PR against the `master` branch.  
To report bugs or suggest features, open an issue or post in the [KSP Forum Thread](https://forum.kerbalspaceprogram.com/topic/227955-112x-realbattery-recharged-v2-realistic-battery-simulation/).

## Translations

Localization is supported. If you'd like to help translate RealBattery into your language, check out the `/Localization` folder and submit a pull request.

Current languages:
- English (`en-us`)
- Italian (`it-it`)

## Licensing

Original mod by **Blackliner**, rewritten and maintained by **Rjoande**.

Licensed under the **[MIT licence](https://opensource.org/license/mit)**.
