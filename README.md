# uc33e-mappings

MIDI mappings for the M-Audio Evolution UC33e controller, one per target device. This repository covers the UC33e as a controller. Axoloti patches (AnDrone, AxoGlitch) are in [axoloti-patches](https://github.com/antonelse/axoloti-patches).

## Contents

| Device | MIDI channel | UC33e presets | Documentation |
|--------|--------------|---------------|---------------|
| Elektron Machinedrum | 1–4 | P01–P17 | [GUIDE](./elektron_md-evolution_uc33e/GUIDE.md) |
| Korg microKORG | 5 | P20 | [GUIDE](./microkorg-evolution_uc33e/GUIDE.md) |
| Behringer XR18 | 6 | P30 | [GUIDE](./behringer_xr18-evolution_uc33e/GUIDE.md) |
| AnDrone (Axoloti) | 1 | P23–P25 | [axoloti-patches/androne](https://github.com/antonelse/axoloti-patches/tree/main/androne) |

Also in this repository:

- [`controllers/uc33e.md`](./controllers/uc33e.md): general UC33e mapping procedure, dump and restore, shortcuts.
- [`docs/`](./docs): studio MIDI capabilities and routing reference.
- `complete_dump_UC33e.syx`: full SysEx dump of the controller.
- `manuals/`: local copies of the manuals, not tracked here. Official sources are linked from each guide.

## TODO

- [ ] Machinedrum: check that P17 (levels and mutes for all 16 machines) is mapped
- [ ] Machinedrum: understand how to change the predefined presets (upper-right buttons)
- [ ] XR18: check whether Mixing Station can also control bus and aux sends
- [ ] All devices: understand MSB/LSB for higher resolution control
- [ ] TD-3 and Zynthian: mappings not started (their MIDI channels are listed in `docs/`)
- [ ] Channel 1: AnDrone and Machinedrum share it; decide whether to move one of them

## License

The documentation, mapping tables and configuration files are licensed under [CC BY 4.0](./LICENSE). Manufacturer manuals and third-party material are not covered.
