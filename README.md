# Undead Legacy Mod Launcher

[![License](https://img.shields.io/badge/License-Proprietary-red.svg)](LICENSE)
[![Platform](https://img.shields.io/badge/Platform-Windows%2010%20%7C%2011-blue.svg)](#requirements)
[![Game](https://img.shields.io/badge/7%20Days%20to%20Die-v2.6%20b14-orange.svg)](https://7daystodie.com/)
[![Mod](https://img.shields.io/badge/Undead%20Legacy-v2.7.40-2ea44f.svg)](https://ul.subquake.com)

An official standalone utility for installing, updating, and playing Subquake's Undead Legacy overhaul mod for 7 Days to Die.

<p align="center">
  <img width="800" alt="Undead Legacy Mod Launcher" src="https://github.com/user-attachments/assets/3095e956-ac90-4a87-8bc5-387df9f2cd89" />
</p>

## Highlights

- **Portable**: No installation required. Runs directly from any folder.
- **Keeps Steam Clean**: Clones the game into a separate folder so your normal Steam 7 Days to Die install is never modified.
- **Safe Save Games**: All saves, settings, and player data are isolated in `./UserData/`, completely separate from your vanilla worlds.
- **Automatic Backups**: Automatically zips up your save files before applying any game updates.
- **Smart Downloads**: Fast multi-part streaming with progress tracking, pause, resume, and cancel controls.
- **File Verifier**: Scans and automatically repairs missing or corrupted files.
- **Official Patch Notes**: Reads the live changelogs directly from `ul.subquake.com`.

## Download

Download the latest official build from the **[GitHub Releases page](https://github.com/SM1ThaYe/UndeadLegacyModLauncher/releases/latest)**.

The release archive contains the standalone portable executable. Extract the archive into a dedicated folder of your choice (e.g. `D:\UndeadLegacyLauncher`) and run `Undead Legacy Mod Launcher.exe`.

## Requirements

- **Operating System**: Windows 10 or Windows 11 (64-bit). *(Windows 8.1 may work, but is not officially supported. macOS and Linux are not supported.)*
- **Base Game**: A clean install of 7 Days to Die (v2.6 b14) on Steam.
- **Disk Space**: At least 15 GB free disk space on your chosen install drive.

## Quick Start

1. Start `Undead Legacy Mod Launcher.exe`.
2. Confirm your Steam 7 Days to Die folder when prompted on first launch.
3. Click **INSTALL** to download and unpack the mod files.
4. When finished, click **PLAY** to start the game.

### Updating Later
- **Updating the Launcher**: Replace your existing `.exe` with the new version from Releases. All paths and settings are preserved automatically.
- **Updating the Mod**: When an update is released, the launcher notifies you on startup. Click **UPDATE** to sync the latest files. (Your custom modlets and save games are not affected).

## Troubleshooting & Important Notes

- **Game takes 30 to 60 seconds to open after clicking PLAY**:  
  Undead Legacy is massive with thousands of custom models and textures. When you click PLAY, the button locks to prevent duplicate clicks while Unity loads in the background. It has not frozen; give it up to a minute to reach the main menu.

- **Game crashes with EasyAntiCheat (EAC) error**:  
  Undead Legacy uses custom code patches that EAC will block. Always start the game through the launcher's **PLAY** button (which automatically bypasses EAC) rather than launching from Steam.

- **Windows SmartScreen or Antivirus popup**:  
  Because this is a free community tool without an expensive commercial certificate, Windows may show *"Windows protected your PC"*. The launcher is 100% safe. Click **"More info"** -> **"Run anyway"**, or add the launcher folder to your antivirus exclusions.

- **Download or extraction seems stuck near the end**:  
  Windows Search Indexer is scanning new files in the background. Open Task Manager (`Ctrl` + `Shift` + `Esc`), find **Windows Search**, and click **End Task** to immediately speed it up.

- **"Access is Denied" or permission errors**:  
  Make sure the launcher is placed in a normal folder (e.g. `D:\UndeadLegacyLauncher` or `C:\Games\UndeadLegacy`) and not inside a restricted Windows system directory like `C:\Program Files`.

- **Steam Overlay not working**:  
  Steam overlay is not supported because the game runs directly from your standalone folder. If you want the overlay, you can add `7DaysToDie.exe` as a non-Steam shortcut in Steam.

- **Game crashes or red console errors**:  
  Grab your `Player.log` (press `Win` + `R`, paste `%USERPROFILE%\AppData\LocalLow\The Fun Pimps\7 Days To Die\`) and submit a report on our **[Bug Tracker](https://github.com/SM1ThaYe/UndeadLegacyModLauncher/issues/new/choose)**.

## Save Files & Backups

- **Save Location**: All worlds and player data are stored in `<LauncherFolder>\UserData\Saves\`.
- **Automatic Backups**: The launcher automatically zips your save folder into `<LauncherFolder>\UserData\Backups\` before any mod update is extracted, keeping the 3 most recent backups to save disk space.

## Log Locations & Bug Reports

If you experience an issue or crash, please include your log files:

- **Game Logs (`Player.log` & `Player-prev.log`)**:  
  Press `Win` + `R`, paste:  
  `%USERPROFILE%\AppData\LocalLow\The Fun Pimps\7 Days To Die\`  
  and press **Enter** to open your log folder directly.
- **Mod & Harmony Logs**: `<LauncherFolder>\Subquakes_Undead_Legacy\BepInEx\LogOutput.log`
- **Launcher Debug Log**: `<LauncherFolder>\update_debug.log`

Found a bug? Report it here with your logs attached:  
**[Submit a Bug Report](https://github.com/SM1ThaYe/UndeadLegacyModLauncher/issues/new/choose)** or reach out in the official Undead Legacy Discord.

## About the Code & License

The Undead Legacy Mod Launcher is closed-source freeware, created and maintained by SMiThaYe & Subquake.

- **Personal Use**: You are welcome to use this launcher freely for personal gaming.
- **Closed Source**: Please do not decompile, reverse engineer, modify, re-host, or redistribute this software on other websites without permission.
- **Disclaimer**: This software is provided "as is" without warranty of any kind.
- **Trademarks**: 7 Days to Die is a registered trademark of The Fun Pimps Entertainment LLC. This is an independent community tool created in collaboration with Subquake.

## Helpful Links

- [Undead Legacy Official Site](https://ul.subquake.com)
- [Official Patch Notes](https://ul.subquake.com/patch-notes)
- [Mod Download](https://ul.subquake.com/download)
- [Launcher Releases](https://github.com/SM1ThaYe/UndeadLegacyModLauncher/releases/latest)

(c) 2026 SMiThaYe & Subquake
