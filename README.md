# Undead Legacy Mod Launcher
Official launcher for installing, updating, and managing Subquake's Undead Legacy overhaul mod for 7 Days to Die.

<img width="1582" height="1213" alt="LauncherForGL" src="https://github.com/user-attachments/assets/2e543263-6707-41fc-ba8d-8a8d3cc29ced" />

## Features
- Portable, no installation required
- One-click install and update of Undead Legacy mod (custom folder location options)
- Automatic Steam 7 Days to Die detection
- Standalone game copy (doesn't modify your vanilla install)
- Isolated save game management with auto-backups
- Deep CRC32 integrity scanning & repair
- Multi-part download with progress bar
- Built-in patch notes from ul.subquake.com

## Requirements
- Windows 10 or 11 64-bit, Windows 8.1 may work but with small UI issues
- 7 Days to Die (v2.6 b14) via Steam
- 15 GB free disk space for mod installation

## Installation
1. Download the latest exe from [Releases](https://github.com/SM1ThaYe/UndeadLegacyModLauncher/releases/latest)
2. Place it in a folder of your choice (e.g. `D:\UndeadLegacyLauncher`)
3. Run it. Folder locations are auto-configured on first launch (with options to change paths)
4. Click INSTALL and follow the status updates to the left.
5. Popup will inform you everything is installed.

## Updating
Just replace the exe with the latest release. 
Your config and paths are saved automatically.

## Troubleshooting
- If your Antivirus or Windows SmartScreen flags the launcher, this is a false positive. Community tools packaged with Python/PyInstaller are commonly flagged by automated scanners because they download and extract mod archives without an expensive commercial signing certificate. The launcher is 100% safe. Run anyway and add an exclusion.
- When you press PLAY, it only needs to be pressed once - I have now coded this so that pressing it once will prevent additional presses. The reason 7D2D seems to take longer is that the Mod Launcher is waiting for Unity engine to engage, and the mod to then load hundreds of custom files - the mod is MASSIVE. It may take up to 60 seconds for the mod to show the Main Menu. This is normal.
- If paths ever change with a new ML update, you don't lose anything. Set your folders as they were before.
- Supports Windows 11/10 64-bit officially. Windows 8 should work, older OS won't work.
- MacOS/Linux not supported.
- Steam overlay is not supported as the game is launched directly from the standalone UL folder. A workaround for Steam is to Add a non-Steam game for 7DaysToDie.exe, but you'd lose the backup/update protections of the Mod Launcher.
- When installing 7D2D game and the Undead Legacy mod fresh, if the status bar seems stuck it isn't, this is due to your Windows search indexer slowing this down due to the thousands of files from this mod. You can open TaskManager and end search indexer process to instantly speed this up.

## Links
- [Undead Legacy Website](https://ul.subquake.com)
- [Patch Notes](https://ul.subquake.com/patch-notes)
- [Mod Download](https://ul.subquake.com/download)
- [Mod Launcher Download](https://github.com/SM1ThaYe/UndeadLegacyModLauncher/releases/latest)

© 2026 SMiThaYe & Subquake
