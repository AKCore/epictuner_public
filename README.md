# EpicTuner

<p align="center">
  <img src="imgs/ETLogo.png" width="400" alt="EpicTuner Logo">
  <img width="1916" height="1109" alt="image" src="https://github.com/user-attachments/assets/3525c10b-3c81-415f-a2aa-8f7f2b57cc24" />

</p>


[![Discord Chat](https://dcbadge.limes.pink/api/server/YfWXcVDauE)](https://discord.gg/YfWXcVDauE)

**Modern ECU Calibration Software**

EpicTuner is a fast, cross-platform ECU tuning app built as a modern alternative to TunerStudio. It's written in .NET with Avalonia UI to stay snappy and look good on any OS.

---

## 🎯 What we're doing

We're trying to build a modern alternative to TunerStudio. 

- **Fast & Snappy**: No long startup times or laggy UI. Everything from 3D tables to high-speed logging is built to be responsive.
- **Modern Workflow**: A clean interface that doesn't feel like it was built 20 years ago.
- **Consistent**: Works and looks the same whether you're on Windows, Mac, or Linux.
- **User Friendly**: We want to make common tasks easier, not harder.

---

## ✨ Inspiration

- **TunerStudio/MegaSquirt**: We're aiming for full compatibility with the standard INI definition system so it works with the ECUs you already have.
- **Haltech NSP**: We love the high-end, integrated feel and layout of NSP and want to bring that experience to more users.

---

## 💻 Why .NET?

EpicTuner uses **.NET 9** and **Avalonia UI**. 

- **Comfort**: It's the language I'm most comfortable with and it's great for writing clean, maintainable code quickly.
- **Performance**: Modern .NET is incredibly fast, which matters for real-time comms and UI rendering.
- **Native AOT**: We use Native AOT compilation, which means:
  - **Instant Startup**: The app opens immediately.
  - **No Bloat**: Smaller binaries and less memory usage.
  - **Self-Contained**: You don't need to install any runtimes; it just runs.

---

## 🚀 What's inside

### The Core
- **Live Connection** - Reliable serial/USB communication.
- **Tuning Files** - MSQ support is currently in progress.
- **Definitions** - Working on full INI compatibility.
- **Scripting** - For ecus that support it, rusEFI and epicEFI have a Lua API that I added a Sytax aware Lua editor for.
- **Remote Tuning API** - Currently working on built in remote tuning functionality, that will keep the tuner and your local ecu in sync.

  

### 3D Tables
- **Heatmaps** - Clear color-coded cells to help you see the map at a glance.
- **Customization** - Swap between built-in colormaps or build your own.
- **Fast Editing** - Drag selection and multi-cell edits.
- **Shortcuts** - Use your keyboard to tune faster:
  - `=` : Set Value
  - `+` : Add
  - `-` : Subtract
  - `*` : Multiply (Scale)
  - `Page Up` : Add 10%
  - `Page Down` : Subtract 10%
- **Math Tools** - Horizontal, vertical, and bilinear interpolation.
- **Rebinning** - Smart axis scaling that handles Z-value interpolation for you.
- **Compatibility** - Imports and exports TunerStudio `.table` XML files.

### 2D Curves
- **Visual Editing** - Drag points directly on the graph.
- **Table Sync** - Table view stays in sync with your graph changes.

### Monitoring
- **Gauges** - Fast, smooth real-time monitoring.
- **Indicators** - Status lights for things like sync, limits, and sensors.
- **Graphs** - Scrolling time-series data for deep diagnostics.
- **Image Wigets** - State based image widgets allow you to bind conditions to the image widgets to acivate based on ranges. 

### The UI
- **Dark Mode** - High-contrast and easy on the eyes.
- **Pop-out Windows** - Great for multi-monitor setups. Pull any table or gauge into its own window.
- **Smart Tracking**: We track pop-out windows so you don't end up with duplicates by accident.
- **Built-in Help**: Hover over fields to see the help text from the INI.
- **Dash Mode**: A full on dashboard mode for use on something like a raspberry pi.

---

## 🖥️ Where it runs

| Platform | Architecture | Status |
|----------|-------------|--------|
| Windows | x64 | ✅ Supported |
| macOS | ARM64 (Apple Silicon) | ✅ Supported |
| macOS | X64 (Intel) | ✅ Supported |
| Linux | x64 | ✅ Supported |
| Linux | ARM64 | ✅ Supported |

---

## 🏁 Getting Started

1. **Download** the latest release for your OS (When Available).
2. **Extract** it.
3. **Run** `EpicTuner.exe` (Windows) or `EpicTuner` (Mac/Linux).
4. **Project Setup**: Point it to your ECU's INI file.
5. **Connect**, Sync, and start tuning.

---

## 🐛 Bugs & Support

If you find a bug, please let us know so we can fix it.

### How to report a bug
1. **Check the list** - See if someone else [already reported it](../../issues).
2. **Open an issue** - Use the "Bug Report" template.
3. **What to include**:
   - **Version**: Check the title bar.
   - **System**: Your OS and architecture.
   - **Steps**: How do we make it happen?
   - **Logs**: Found in `%LOCALAPPDATA%/EpicTuner/Logs` (Windows) or `~/.local/share/EpicTuner/Logs` (Mac/Linux).
   - **Screenshots**: Pictures make things much easier to understand.

### Got an idea?
Open a "Feature Request" and tell us what you'd like to see.

---

### Trademark Disclaimer

EpicTuner is an independent, project created for **interoperability purposes** under fair use principles. This software parses ini files created by ecu developers for operation with known software.

The following trademarks are the property of their respective owners:

- **Haltech** is a trademark of Haltech Engine Management Systems
- **Speeduino** is a trademark of the Speeduino project
- **rusEFI** is a trademark of the rusEFI project
- **MegaSquirt** is a trademark of Bowling and Grippo

**EpicTuner is not affiliated with, endorsed by, or sponsored by any of these companies or projects.** All product names, logos, and brands are property of their respective owners and are used solely for identification and interoperability purposes.

### Interoperability Statement

This software is developed under the principles established by [Sega v. Accolade](https://en.wikipedia.org/wiki/Sega_Enterprises,_Ltd._v._Accolade,_Inc.) and similar legal precedents that recognize the legitimacy of reverse engineering for interoperability. EpicTuner

1. **Reads publicly available data** - Parses ini, binary, and other formats that ECU manufacturers provide
2. **Does not circumvent copy protection** - Works only with user-accessible data files
3. **Enables data portability** - Allows users to work with their ECUs in a unified, cross-platform tool

## 🔒 Status & License

**Alpha Release** - EpicTuner is currently in heavy development. 

### Heads up
- Only tested on **rusEFI**, **epicEFI**, **FOME** and **Speeduino** hardware.
- Plugin system is coming later.

### Sponsorships
- EpicTuner is not sponsored by or affiliated with any specific hardware/firmware vendor although I am not against this. 
- If any would like to sponsor the project and help shape the development of ET, or have custom feature requests that are not in the standard ini spec, please reachout to me on our discord you can find at the top of the readme. 


### License
EpicTuner is **not** open source right now. 

For now,
this repo is for version tracking, bugs, docs, and alpha builds.

---

*Thanks for testing EpicTuner!*
