# Project Manager Simulator (Симулятор руководителя проекта)

## Overview
A Russian-language HTML5 browser game where the player takes on the role of a Project Manager at "Pervy Bit" IT company. The game features four levels with different gameplay modes (2D platformer, top-down, and stealth).

## Architecture
- **Pure static site**: Single `index.html` file containing all HTML, CSS, and JavaScript
- **No build system**: No npm, webpack, or bundlers — pure vanilla browser technologies
- **Assets**: `assets/` directory contains PNG images and MP3 audio files

## Running the App
The app is served via Python's built-in HTTP server:
```
python3 -m http.server 5000
```

## Workflow
- **Start application**: Serves the static site on port 5000 (webview)

## Deployment
- Configured as a **static** deployment with `publicDir: "."`

## Known Issues
- `assets/music_level4.mp3` is missing from the repository (404 on load, but the game continues without it)
