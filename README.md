# Undead Legacy Mod Launcher

Official launcher for installing, updating, and managing Subquake's Undead Legacy overhaul mod for 7 Days to Die.

<p align="center">
  <img width="800" alt="Undead Legacy Mod Launcher" src="https://github.com/user-attachments/assets/3095e956-ac90-4a87-8bc5-387df9f2cd89" />
</p>


## Features
- **Portable**: No installation required. Run it from any folder.
- **One-Click Install & Update**: Installs and updates Undead Legacy automatically with custom folder location options.
- **Keeps Steam Game Clean**: Creates a standalone game copy so your original vanilla install is never modified.
- **Safe Save Games**: All saves, settings, and player data are kept separate in `./UserData/` to avoid conflicts with vanilla worlds.
- **Automatic Backups**: Automatically zips up your saves before extracting any game updates.
- **Fast Downloads**: Multi-part streaming with progress bar, live transfer speed, pause, resume, and cancel buttons.
- **File Integrity Verifier**: Scans and repairs missing or corrupted files automatically.
- **Built-in Patch Notes**: Reads the official update logs straight from `ul.subquake.com`.


## Requirements
- Windows 10 or 11 (64-bit). *(Windows 8.1 may work, but is not officially supported. macOS and Linux are not supported.)*
- 7 Days to Die (v2.6 b14) installed via Steam.
- 15 GB free disk space on your chosen install drive.


## Installation
1. Download the latest executable from **[Releases](https://github.com/SM1ThaYe/UndeadLegacyModLauncher/releases/latest)**.
2. Place it in a folder of your choice (e.g. `D:\UndeadLegacyLauncher`).
3. Run `Undead Legacy Mod Launcher.exe`. Folder locations are auto-configured on first launch (with options to change paths).
4. Click **INSTALL** and follow the status updates on the left.
5. A popup will inform you once everything is finished. Click **PLAY** to start.


## Updating the Launcher & Mod
- **Updating the Launcher**: Just replace the `.exe` with the latest release. Your config and paths are saved automatically.
- **Updating the Mod**: The launcher checks for mod updates when opened and will notify you. Click **UPDATE** when prompted. (Updates act as a clean mod sync and will not affect your custom modlets or saves).


## Good to Know & Common Questions

### When you press PLAY, give it up to 60 seconds
When you click PLAY, the button locks to prevent accidental double-clicks. Because Undead Legacy loads thousands of custom assets, models, and textures, Unity can take **30 to 60 seconds** before the main menu appears. This is completely normal—the game has not frozen.

### Always launch using the launcher's PLAY button (Not Steam)
Undead Legacy uses custom code patches that EasyAntiCheat (EAC) will block. The launcher's PLAY button automatically bypasses EAC and directs the game to your isolated `./UserData` folder.

### Antivirus and Windows SmartScreen popups
Because this is a free community tool without an expensive commercial code certificate, Windows or your antivirus may show a blue *"Windows protected your PC"* popup or flag it as unknown. The launcher is 100% safe. Click **"More info"** -> **"Run anyway"**, or add the folder to your antivirus exclusions.

### Extraction seems slow or paused?
When installing fresh, if the progress bar seems stuck near the end, Windows Search Indexer is usually scanning the thousands of newly extracted mod files in the background. You can open Task Manager and end the "Windows Search" process to immediately speed it up.

### Steam Overlay
Steam overlay is not supported because the game runs directly from your standalone folder. If you wish to use Steam overlay, you can add `7DaysToDie.exe` as a non-Steam game, though launching through the launcher is always recommended for save protection and update checks.


## Save Game Locations & Backups
- **Sandboxed Saves**: The launcher saves all game progress to `./UserData/` inside the mod folder. Your vanilla Steam 7 Days to Die worlds and character profiles are untouched.
- **Automatic Backups**: The launcher automatically zips `./UserData/Saves` to `./UserData/Backups/` before extracting any mod updates. It retains the 3 most recent backups to save disk space. Downloaded zip archives are cleaned up automatically.


## Log File Locations (For Bug Reports)
If you run into an issue or crash, please include your log files:

- **Game Logs (`Player.log` & `Player-prev.log`)**:  
  Press `Win` + `R`, paste:  
  `%USERPROFILE%\AppData\LocalLow\The Fun Pimps\7 Days To Die\`  
  and press **Enter** to open your log folder directly.
- **Mod & Harmony Logs**: `<LauncherFolder>\Subquakes_Undead_Legacy\BepInEx\LogOutput.log`
- **Launcher Debug Log**: `<LauncherFolder>\update_debug.log`

Found a bug? Report it here with your logs attached:  
**[Submit a Bug Report](https://github.com/SM1ThaYe/UndeadLegacyModLauncher/issues/new/choose)** or reach out in the official Undead Legacy Discord.


## About the Code & License
The Undead Legacy Mod Launcher is closed-source freeware, created and maintained by SMiThaYe and Subquake.

- **Personal Use**: You are welcome to use this launcher freely for your own gaming.
- **Closed Source**: Please do not decompile, reverse-engineer, modify, re-host, or redistribute this software on other websites without permission.
- **Disclaimer**: This software is provided "as is" without warranty of any kind.
- **Trademarks**: 7 Days to Die is a registered trademark of The Fun Pimps Entertainment LLC. This is an independent community tool created in collaboration with Subquake.


## Links
- [Undead Legacy Official Site](https://ul.subquake.com)
- [Official Patch Notes](https://ul.subquake.com/patch-notes)
- [Mod Download](https://ul.subquake.com/download)
- [Mod Launcher Download](https://github.com/SM1ThaYe/UndeadLegacyModLauncher/releases/latest)

(c) 2026 SMiThaYe & Subquake
