# EpicTuner

<p align="center">
  <img src="imgs/ETLogo.png" width="400" alt="EpicTuner Logo">
</p>

[![Discord Chat](https://dcbadge.limes.pink/api/server/YfWXcVDauE)](https://discord.gg/YfWXcVDauE)

**Modern ECU calibration software.** A fast, cross-platform alternative to TunerStudio, Built from the ground up in C++ and Qt 6.

### 📥 [Download EpicTuner at sgkembedded.com/epictuner](https://www.sgkembedded.com/epictuner)

The [changelog](https://www.sgkembedded.com/epictuner/changelog) is on the website too. This repo is for bug reports and feature requests.

---

## 🎯 What we're doing

We're trying to build a modern alternative to TunerStudio.

- **Fast & Snappy**: No long startup times or laggy UI. Everything from 3D tables to high-speed logging is built to be responsive.
- **Modern Workflow**: A clean interface that doesn't feel like it was built 20 years ago.
- **Consistent**: Works and looks the same on every platform.
- **User Friendly**: We want to make common tasks easier, not harder.

## ✨ Inspiration

- **TunerStudio/MegaSquirt**: We're aiming for full compatibility with the standard INI definition system so it works with the ECUs you already have.
- **Haltech NSP**: We love the high-end, integrated feel and layout of NSP and want to bring that experience to more users.

---

## Features

- **INI-based ECU definitions**: works with the TunerStudio INI and MSQ formats your ECU already uses.
- **Table & curve editors**: 2D grid and 3D surface views with select, set/add/scale, interpolate, smooth and undo.
- **Dashboards**: configurable gauges, indicators and live graphs, in docked or floating windows.
- **Datalogging**: record `.mlg` logs, compare channels on synced graphs, and play logs back offline without an ECU.
- **AutoTune**: live VE table correction from measured AFR.
- **Tooth logger & trigger analyzer**
- **Lua editor**: syntax highlighting, completion and error checking for rusEFI/epicEFI Lua scripts.
- **ECU console**
- **Firmware updates**: flash epicEFI/rusEFI bundles directly from the app.
- **Plugins**: native plugin support with a [developer SDK](https://www.sgkembedded.com/epictuner/sdk/index.html).
- **Built-in updates**: the app updates itself.

## Platforms

| Platform | Status |
|----------|--------|
| Windows x64 | ✅ Installer or portable zip |
| Linux x64 | ✅ AppImage or .deb |
| Linux ARM64 | 🔜 Coming later |

Tested with **rusEFI**, **epicEFI**, **FOME** and **Speeduino**.

---

## Bugs & feature requests

1. Check whether it's [already reported](../../issues).
2. Open an issue with the **Bug Report** or **Feature Request** template.
3. For bugs, include your EpicTuner version, OS, steps to reproduce, and screenshots or logs if you have them.

Questions are welcome on [Discord](https://discord.gg/YfWXcVDauE).

---

## Trademarks

EpicTuner is an independent project built for interoperability. It is not affiliated with, endorsed by or sponsored by Haltech, Speeduino, rusEFI, MegaSquirt (Bowling and Grippo) or EFI Analytics.
All trademarks belong to their respective owners.

## 🔒 Status

**Alpha Release** - EpicTuner is currently in heavy development. Expect bugs, and please report them.

## License

EpicTuner is closed-source software by [SGK Embedded Performance](https://www.sgkembedded.com).
