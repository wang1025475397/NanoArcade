# NanoArcade Manager

A beautiful, browser-based tool to manage your retro game collection for RG Nano and similar handheld devices.

![NanoArcade](assets/images/logo.png)

## Features

- **Console Organization** - Automatically detects and organizes games by console folder
- **Box Art Management** - Search, download, and manage box art for your games
  - Search TheGamesDB for official box art
  - Upload local images
  - Paste image URLs directly
  - Auto-resize images to 240px (optimized for RG Nano)
- **Smart Filtering & Sorting**
  - Filter to show only games missing art
  - Sort A-Z, Z-A, or by art status
  - Search games by name
- **Batch Upload** - Upload multiple ROMs at once with automatic filename cleaning
- **Right-Click Context Menu** - Quick actions for any game:
  - Edit box art
  - Search art
  - Google Images search
  - Rename game
  - Delete game
- **Persistent Storage** - Remembers your selected folder between sessions
- **Beautiful UI** - Modern dark theme with smooth animations

## How to Use

1. Download `NanoArcade Manager.html` and the `assets` and `icons` folders
2. Open `NanoArcade Manager.html` in a modern browser (Chrome, Edge, or other Chromium-based browser)
3. Click "Select Folder" and choose your ROMs folder
4. Your folder should be organized with subfolders for each console (e.g., `GBA`, `SNES`, `NES`)
5. Click on a console to view and manage your games
6. Click any game to add/edit box art, or right-click for quick actions

## Folder Structure

Your ROMs folder should look like this:
```
ROMs/
├── GBA/
│   ├── Pokemon Emerald.gba
│   ├── Pokemon Emerald.png  (box art)
│   └── ...
├── SNES/
│   ├── Super Mario World.sfc
│   └── ...
└── NES/
    └── ...
```

## Supported Consoles

The app recognizes and displays icons for:
- Game Boy / Game Boy Color / Game Boy Advance
- NES / SNES / N64 / GameCube
- Sega Master System / Genesis / Saturn / Dreamcast / Game Gear
- PlayStation / PS2 / PSP / PS Vita
- PC Engine / TurboGrafx
- Nintendo DS
- Atari Lynx
- WonderSwan
- Neo Geo Pocket
- Arcade (MAME/FBA)
- And more!

## Requirements

- Modern web browser with File System Access API support (Chrome, Edge, Opera)
- JavaScript enabled

## Credits

- UI based on [Hyperspace](https://html5up.net/hyperspace) by HTML5 UP
- Console icons included in the `icons` folder

## License

Free for personal use. Template design by HTML5 UP under CCA 3.0 license.
