# Pixel Sparkle Cursor

A Chrome extension that makes pixel sprites (gnome, heart, mushroom) trail behind your cursor on every webpage.

![License: GPL-3.0](https://img.shields.io/badge/License-GPLv3-blue.svg)

## Features

- Pixel sprites follow your mouse across any website
- 4 physics modes: **Gravity**, **Float**, **Burst**, **Rain**
- Adjustable spawn count and sprite size
- Settings persist between sessions (via `chrome.storage.local`)
- Pure vanilla JS — no dependencies, no build step

## Installation

1. Download or clone this repository
2. Open `chrome://extensions` in Chrome
3. Enable **Developer mode** (top-right corner)
4. Click **Load unpacked** and select the project folder
5. Move your mouse — sparkles!

## Usage

Click the extension icon to open the popup:

| Control | Description |
| --- | --- |
| Count slider | Number of particles spawned per cursor movement |
| Size slider | Base size of the sprites |
| Physics buttons | Gravity (default), Float, Burst, Rain |

## Project structure

```
├── content.js      # Canvas overlay + particle animation
├── popup.html      # Settings popup UI
├── popup.js        # Popup logic + storage sync
├── manifest.json   # Extension manifest (MV3)
└── sprites/        # Pixel art sprites (gnome, heart, mushroom)
```

## License

This project is licensed under the [GNU General Public License v3.0](LICENSE).
