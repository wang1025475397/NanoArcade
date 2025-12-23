# NanoArcade Manager

A beautiful, browser-based tool to manage your retro game collection across multiple operating systems and devices.

base: https://github.com/audioslayer/NanoArcade

![NanoArcade](assets/images/logo.png)

## Try It Now

**[Launch Live App](https://wang1025475397.github.io/NanoArcade/)** - Use instantly in your browser, no download required

Or download this repository for offline use.

---

## :joystick: What's New in v1.6.branch

it now supports batch fetching of cover art from Libretro and searching for cover art directly via **Libretro**, delivering a more intuitive workflow that aligns with how users actually configure their handhelds while streamlining cover art management.

## Supported Operating Systems & Devices

### :potato: MustardOS (muOS)
Multi-device custom firmware with 3 resolution tiers:

**Standard (324px)** - 640×480 screens:
- Anbernic RG28XX H
- Anbernic RG35XX (original)
- Anbernic RG35XX Plus
- Anbernic RG35XX H
- Anbernic RG35XX SP

**High-Res (380px)** - 720p-1024p screens:
- Anbernic RG34XX
- Anbernic RGCUBEXX
- TrimUI Brick

**Ultra (450px)** - 1280×720 screens:
- TrimUI Smart Pro
- Anbernic RG40XX H
- Anbernic RG40XX V

### :onion: Onion OS
Custom firmware for Miyoo devices (250px):
- Miyoo Mini
- Miyoo Mini Plus
- Miyoo Flip
- Miyoo Mini Flip

### :key: DrUm78 (FunKey-OS)
Custom firmware for micro handhelds (240px):
- Anbernic RG Nano
- FunKey S
- Powkiddy Q36 Mini
- Powkiddy GBA Mini

### :zap: MinUI
Minimalist multi-device OS with 2 resolution tiers:

**Standard (200px)**:
- Anbernic RGB30
- Anbernic RG35XX series
- TrimUI Smart
- GKD Pixel
- Miyoo Mini series

**High-Res (300px)**:
- Anbernic RG405
- Anbernic RG40XX
- Anbernic RG CubeXX
- TrimUI Smart Pro

### :rocket: NextUI
MinUI fork with enhanced features and 3 resolution tiers:

**Standard (200px)**:
- Anbernic RG35XX SP

**High-Res (300px)**:
- TrimUI Brick

**Ultra (500px)**:
- TrimUI Smart Pro

## Features

### :joystick: Device Support
- **Multi-Device Selector** - Switch between device profiles with different folder structures and image sizes
- **Onion OS Integration** - Full support for Onion OS folder structure (`Roms/[Console]/Imgs/`)
- **Mustard OS Integration** - Full support for Mustard OS catalogue structure (`MUOS/info/catalogue/<System>/box/`)
- **MinUI Integration** - Full support for MinUI folder structure with `.res` folders and console tags
- **NextUI Integration** - Full support for NextUI folder structure with `.media` folders
- **Auto-Resize** - Images automatically resized to optimal dimensions per device (240px for RG Nano, 250px for Miyoo, 354px for Trimui Brick, 200px/300px for MinUI, 200px/300px/400px for NextUI)

### :art: Theme System
- **7 Color Themes** - Choose from Blue, Purple, Green, Red, Cyan, Orange, Pink
- **Persistent Selection** - Theme saves via localStorage

### :video_game: GameFAQs Integration
- **Dual Search** - Box art searched from both TheGamesDB and GameFAQs simultaneously
- **Game Info Display** - Rating, Difficulty, and Length shown in game modal
- **Styled Tooltips** - Hover for detailed breakdowns (votes, verdicts, playtime)

### :floppy_disk: Save Manager
- **Multi-Device Support** - Backup, restore, and delete game saves for RG Nano, Miyoo devices (Onion OS), MinUI, and NextUI
- **Emulator Core Mapping** - Automatic save path detection for Gambatte, gpSP, FCEUmm, Supafaust, and more
- **MinUI/NextUI Support** - Manages saves in `.userdata/[system]/Saves/` folders
- **Delete Confirmation** - Modal confirmation prevents accidental deletions
- **Hidden File Filtering** - Automatically ignores hidden files/folders (starting with `.`) except `.res` and `.media` used by MinUI/NextUI

### :trophy: Top 25 Must-Have Games
- **Curated Lists** - Top 25 rated games for 16 different consoles
- **Collection Tracker** - See which must-have games you own vs missing
- **Quick Upload** - Drag & drop missing ROMs directly into the Top 25 modal
- **Supported Consoles**: GB, GBC, GBA, NES, SNES, N64, Genesis, Game Gear, Master System, PS1, PC Engine, Neo Geo, Neo Geo Pocket, Atari 2600, Atari Lynx, WonderSwan

### :framed_picture: Box Art Management
- **Dual Image Search** - Search TheGamesDB and GameFAQs for box art
- **Upload Local Images** - Drag & drop or browse for local artwork
- **URL Import** - Paste image URLs directly with automatic download
- **Smart Processing** - Auto-resize, format conversion, and optimization

### :file_folder: Organization & Filtering
- **Console Detection** - Automatically detects and organizes games by console folder
- **Missing Art Filter** - Quickly find games that need artwork
- **A-Z Sorting** - Toggle alphabetical sorting
- **Search** - Filter games by name
- **All Games View** - Browse your entire collection across all consoles

### :hammer_and_wrench: Game Management
- **Batch Upload** - Upload multiple ROMs with automatic filename cleaning
- **Right-Click Menu** - Quick actions: edit art, search, rename, delete
- **Google Images Integration** - One-click search for hard-to-find artwork
- **Rename & Delete** - Manage your ROM files directly

### :sparkles: User Experience
- **Responsive Design** - Mobile-friendly hamburger menu for screens ≤1292px
- **Browser Detection** - Friendly warning for unsupported browsers (Firefox)
- **Subfolder Support** - Automatically scans nested ROM folders with visual indicators
- **Press Start 2P Font** - Retro pixel font for game titles and console names
- **Responsive Modal** - Game modal scales for smaller screens (1080p and below)
- **Button Hover Effects** - Pop-up animation on all buttons
- **Styled Tooltips** - Custom tooltips matching the theme
- **Styled Scrollbars** - Scrollbars match the app theme
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
7. Click the **Top 25** button to see must-have games for that console

## Folder Structures

### MustardOS (muOS)
```
MUOS/
└── info/
    └── catalogue/
        ├── gba/
        │   ├── Pokemon Emerald.gba
        │   └── box/
        │       └── Pokemon Emerald.png  (box art in box subfolder)
        ├── snes/
        └── nes/
```

### Onion OS
```
Roms/
├── GBA/
│   ├── Pokemon Emerald.gba
│   └── Imgs/
│       └── Pokemon Emerald.png  (box art in Imgs subfolder)
├── SNES/
└── NES/
```

### DrUm78 (FunKey-OS)
```
ROMs/
├── GBA/
│   ├── Pokemon Emerald.gba
│   ├── Pokemon Emerald.png  (box art next to ROM)
│   └── ...
├── SNES/
└── NES/
```

### MinUI (480p / High-Res)
```
Roms/
├── Game Boy (GB)/
│   ├── Pokemon Red.gb
│   ├── Pokemon Blue.gb
│   └── .res/
│       ├── Pokemon Red.gb.png  (box art with ROM extension)
│       └── Pokemon Blue.gb.png
├── Super Nintendo (SFC)/
└── Nintendo Entertainment System (FC)/
```

### NextUI (Trimui Brick/Smart Pro)
```
Roms/
├── Game Boy (GB)/
│   ├── Pokemon Red.gb
│   ├── Pokemon Blue.gb
│   └── .media/
│       ├── Pokemon Red.png  (box art without ROM extension)
│       └── Pokemon Blue.png
├── Super Nintendo (SFC)/
└── Nintendo Entertainment System (FC)/
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

### v1.6
:rocket: **MinUI Support** - Full support for MinUI operating system with `.res` folder structure and console tag parsing (e.g., "Game Boy (GB)")

:zap: **NextUI Support** - Full support for NextUI (MinUI fork) with `.media` folder structure for Trimui Brick/Smart Pro/RG35XX SP

:framed_picture: **Dual Resolution Support** - MinUI devices can choose between 480p (200px) or High-Res (300px) image sizes via resolution selector modal

:art: **Smart Image Naming** - MinUI images saved with ROM extension (`Pokemon Red.gb.png`), NextUI without (`Pokemon Red.png`)

:floppy_disk: **MinUI/NextUI Save Manager** - Full save management for MinUI and NextUI devices with automatic system mapping (`.userdata/[system]/Saves/`) - 18 supported consoles

**UI/UX Improvements:**
- :sparkles: Device selector modal optimized for 1080p displays with hidden scrollbar
- :sparkles: Generic device option moved to compact button below device grid
- :sparkles: Responsive device grid (3-column on desktop, 2-column on tablets, 1-column on mobile)
- :sparkles: Device selector description moved to tooltip for cleaner layout

**Bug Fixes:**
- :wrench: Fixed MinUI/NextUI folder scanning to properly detect Roms subfolder
- :wrench: Fixed image rendering for MinUI/NextUI devices in game grid
- :wrench: Fixed image detection and loading for all device types
- :wrench: Added WonderSwan support to MinUI/NextUI folder mappings

### v1.5
:art: **Theme Customization** - Choose from 7 color themes (Blue, Purple, Green, Red, Cyan, Orange, Pink) with persistent localStorage saving

:iphone: **Responsive Mobile Menu** - Hamburger menu at ≤1292px with fullscreen overlay for phones/tablets

:globe_with_meridians: **Browser Detection** - Friendly modal for unsupported browsers (Firefox) with logos for Chrome/Edge/Opera

:floppy_disk: **Onion OS Save Manager** - Full save management for Miyoo Mini/Mini+/Flip with emulator core mapping

:file_folder: **Recursive Subfolder Scanning** - Automatically detects ROMs in nested folders with visual indicators

**UI/UX Improvements:**
- :sparkles: Missing art indicator changed to picture icon with tooltip
- :sparkles: Synced pulse animation on SELECT DEVICE button (matches logo)
- :sparkles: Modernized browser requirements section with PNG icons
- :sparkles: Fixed sidebar layout - no more theme/version overlap
- :sparkles: Device name shown next to Home in sidebar
- :sparkles: Centered "Home" link when no device selected

**Bug Fixes:**
- :wrench: Images now save to correct standard device locations (not game subfolders)
- :wrench: Subfolder paths moved to tooltips for cleaner UI
- :wrench: Fixed sidebar height/overflow issues on small screens

### v1.4
- **GameFAQs Integration** - Additional box art source searching in parallel with TheGamesDB
- **Game Info Display** - Rating, Difficulty, and Length from GameFAQs shown in game modal
- **Styled Tooltips** - Hover over Rating/Difficulty/Length for detailed breakdowns
- **Save Manager** - Backup, restore, and delete saves for RG Nano
- **Press Start 2P Font** - Retro pixel font for game titles, console names, and sidebar
- **Responsive Modal** - Game modal scales for smaller screens (1080p and below)
- **Button Hover Effects** - All buttons now have pop-up animation on hover
- **Streamlined URL Input** - Google search icon inside input field
- **Game Title Tooltip** - Hover over truncated titles to see full name
- **Styled Scrollbars** - Top 25 list and other areas match theme
- **Top 25 Layout Fix** - Rank numbers and icons no longer clip
- **MustardOS Scanning Fix** - Fixed ROM folder scanning for Trimui Brick
- **Delete Confirmation** - Added modal confirmation for deleting saves

### v1.3
- **Trimui Brick support** - Added full Mustard OS integration
- Mustard OS catalogue structure support (`MUOS/info/catalogue/<System>/box/`)
- 354px image resolution for Trimui Brick's 1024x768 display
- Automatic 3-tier folder structure creation
- 30+ Mustard OS system mappings (GB, GBA, NES, SNES, PS1, etc.)
- Validation for Mustard OS folder structure

### v1.2
- Added device selector (RG Nano, Miyoo Mini, Miyoo Flip)
- Full Onion OS support with Imgs subfolder structure
- **Top 25 Games feature** - See must-have games per console with owned/missing status
- Top 25 lists for 16 consoles (400 curated games total)
- Upload ROMs directly from Top 25 modal
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

- UI based on [Hyperspace](https://html5up.net/hyperspace) by HTML5 UP
- Box art from [TheGamesDB](https://thegamesdb.net/) and [GameFAQs](https://gamefaqs.gamespot.com/)
- Console icons included in the `icons` folder
- Top 25 game lists curated from community rankings

## License

Free for personal use. Template design by HTML5 UP under CCA 3.0 license.
