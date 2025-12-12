# NanoArcade Manager

A beautiful, browser-based tool to manage your retro game collection for RG Nano, Miyoo Mini, and other handheld devices.

![NanoArcade](assets/images/logo.png)

## Try It Now

**[Launch Live App](https://audioslayer.github.io/NanoArcade/)** - Use instantly in your browser, no download required

Or download this repository for offline use.

---

## Supported Devices

- **RG Nano** - Anbernic's tiny retro handheld
- **Miyoo Mini / Mini+** - With Onion OS support
- **Miyoo Flip** - With Onion OS support
- **TrimUI Smart Pro** - Coming soon

## Features

### Device Support
- **Multi-Device Selector** - Switch between device profiles with different folder structures and image sizes
- **Onion OS Integration** - Full support for Onion OS folder structure (`Roms/[Console]/Imgs/`)
- **Auto-Resize** - Images automatically resized to optimal dimensions per device (240px for RG Nano, 250px for Miyoo)

### Box Art Management
- **Dual Image Sources** - Search both TheGamesDB and The Cover Project for box art
- **Upload Local Images** - Drag & drop or browse for local artwork
- **URL Import** - Paste image URLs directly with automatic download
- **Smart Processing** - Auto-resize, format conversion, and optimization

### Organization & Filtering
- **Console Detection** - Automatically detects and organizes games by console folder
- **Missing Art Filter** - Quickly find games that need artwork
- **A-Z Sorting** - Toggle alphabetical sorting
- **Search** - Filter games by name
- **All Games View** - Browse your entire collection across all consoles

### Game Management
- **Batch Upload** - Upload multiple ROMs with automatic filename cleaning
- **Right-Click Menu** - Quick actions: edit art, search, rename, delete
- **Google Images Integration** - One-click search for hard-to-find artwork
- **Rename & Delete** - Manage your ROM files directly

### User Experience
- **Loading Indicators** - Visual feedback when loading large collections
- **Ultrawide Support** - Responsive layout for any screen size
- **Persistent Storage** - Remembers your folder selection between sessions
- **Modern Dark UI** - Beautiful interface with smooth animations and neon accents

## How to Use

1. Download or clone this repository
2. Open `index.html` in a modern browser (Chrome, Edge, or Chromium-based)
3. Select your device type from the dropdown (RG Nano, Miyoo Mini, etc.)
4. Click "Select ROMs Folder" and choose your device's ROM directory
5. Click on any console to view and manage your games
6. Click a game to add/edit box art, or right-click for quick actions

## Folder Structures

### RG Nano
```
ROMs/
├── GBA/
│   ├── Pokemon Emerald.gba
│   ├── Pokemon Emerald.png  (box art next to ROM)
│   └── ...
├── SNES/
└── NES/
```

### Miyoo Mini / Flip (Onion OS)
```
Roms/
├── GBA/
│   ├── Pokemon Emerald.gba
│   └── Imgs/
│       └── Pokemon Emerald.png  (box art in Imgs subfolder)
├── SNES/
└── NES/
```

## Supported Consoles

The app recognizes and displays icons for:
- Game Boy / Game Boy Color / Game Boy Advance
- NES / SNES / N64 / GameCube
- Sega Master System / Genesis / Saturn / Dreamcast / Game Gear
- PlayStation / PS2 / PSP / PS Vita
- PC Engine / TurboGrafx-16
- Nintendo DS
- Neo Geo / Neo Geo Pocket Color
- Atari (2600, 7800, Lynx)
- WonderSwan / WonderSwan Color
- Arcade (MAME/FinalBurn)
- PICO-8
- And more!

## Requirements

- Modern web browser with File System Access API support (Chrome, Edge, Opera)
- JavaScript enabled

## Changelog

### v1.2
- Added device selector (RG Nano, Miyoo Mini, Miyoo Flip)
- Full Onion OS support with Imgs subfolder structure
- Added The Cover Project as second image source
- Loading spinner for large collections
- Ultrawide monitor support
- Clickable stats to navigate to games
- Streamlined sort toggle (A-Z/Z-A button)
- Fixed file:// protocol compatibility
- Memory and performance optimizations
- Production-ready code cleanup

### v1.1
- Added JPG image support

### v1.0
- Initial release

## Credits

- Box art from [TheGamesDB](https://thegamesdb.net/)

## License

Free for personal use. Template design by HTML5 UP under CCA 3.0 license.
