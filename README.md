⚠️ **Work in progress.** Mappings, documentation and file structure may change or contain inaccuracies. Verify critical settings against the official hardware manuals.

# uc33e-mappings

MIDI mappings for the **M-Audio Evolution UC33e** controller, one per target device. Everything here is about the UC33e as a controller. Patches for Axoloti (including AnDrone and AxoGlitch) live in [axoloti-patches](https://github.com/antonelse/axoloti-patches).

## Mappings

| Device | Status | MIDI channel | UC33e presets | Documentation |
|--------|--------|--------------|---------------|---------------|
| Elektron Machinedrum | ✅ Complete | 1–4 | P01–P17 | [GUIDE](./elektron_md-evolution_uc33e/GUIDE.md) |
| Korg microKORG | ✅ Complete | 5 | P20 | [GUIDE](./microkorg-evolution_uc33e/GUIDE.md) |
| Behringer XR18 | ✅ Complete | 6 | P30 | [GUIDE](./behringer_xr18-evolution_uc33e/GUIDE.md) |
| AnDrone (Axoloti) | ✅ Complete | 1 | P23–P25 | [axoloti-patches/androne](https://github.com/antonelse/axoloti-patches/tree/main/androne) |

Presets are on the UC33e. P23–P25 hold the AnDrone mapping; the complete dump in this repo includes them.

## Repository contents

- [`controllers/uc33e.md`](./controllers/uc33e.md): general UC33e mapping procedure, dump and restore, shortcuts.
- [`docs/`](./docs): studio MIDI capabilities and routing reference.
- `complete_dump_UC33e.syx`: full SysEx dump of the controller.
- `manuals/`: local copies of the manuals, not tracked here. Official sources are linked from each guide.

## License

The documentation, mapping tables and configuration files are licensed under [CC BY 4.0](./LICENSE). Manufacturer manuals and third-party material are not covered.

## Notes

- AnDrone's MIDI channel (1) is the same as the Machinedrum channel range (1–4). The routing reference in `docs/` describes the setup as it is.
