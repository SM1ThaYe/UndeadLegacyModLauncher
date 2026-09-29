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

## Updating Mod Launcher
Just replace the exe with the latest release. 
Your config and paths are saved automatically.
To update Undead Legacy mod, it will check when you first open the Mod Launcher and notify you, then press UPDATE.
Update also acts as a full mod download and install (does not affect your modlets).

## Troubleshooting
- If your Antivirus or Windows SmartScreen flags the launcher, this is a false positive. Community tools packaged with Python/PyInstaller are commonly flagged by automated scanners because they download and extract mod archives without an expensive commercial signing certificate. The launcher is 100% safe. Run anyway and add an exclusion.
- When you press PLAY, it only needs to be pressed once - I have now coded this so that pressing it once will prevent additional presses. The reason 7D2D seems to take longer is that the Mod Launcher is waiting for Unity engine to engage, and the mod to then load hundreds of custom files - the mod is MASSIVE. It may take up to 60 seconds for the mod to show the Main Menu. This is normal.
- If paths ever change with a new ML update, you don't lose anything. Set your folders as they were before.
- Supports Windows 11/10 64-bit officially. Windows 8 should work, older OS won't work.
- MacOS/Linux not supported.
- Steam overlay is not supported as the game is launched directly from the standalone UL folder. A workaround for Steam is to Add a non-Steam game for 7DaysToDie.exe, but you'd lose the backup/update protections of the Mod Launcher.
- When installing 7D2D game and the Undead Legacy mod fresh, if the status bar seems stuck it isn't, this is due to your Windows search indexer slowing this down due to the thousands of files from this mod. You can open TaskManager and end search indexer process to instantly speed this up.

## Common Issues
- Windows SmartScreen Blue Banner: Because this is an independent mod utility without an expensive enterprise certificate, Windows SmartScreen will show: "Windows protected your PC". Click "More info" -> "Run anyway".
- Antivirus False Positives: Compiled native Python/C++ binaries often trigger generic heuristic detections. Add the launcher folder to your antivirus exclusion list if blocked.
- EasyAntiCheat (EAC) Warning: Undead Legacy and custom Harmony C# modlets cannot run with EAC active. Always launch through the Mod Launchers PLAY button (which automatically bypasses EAC) rather than launching standard 7DTD from Steam. Mod Launchers own UserData folder is also why you should always use the launcher to avoid conflicts and ensure there are no issues.

## Save Game Locations and Backups
- Sandboxed Saves: Mod Launcher saves all game progress to ./UserData/ inside the mod folder. Your vanilla Steam 7 Days to Die worlds and character profiles are untouched.
- Automatic Backups: Mod Launcher automatically zips ./UserData/Saves to ./UserData/Backups/ before extracting any mod updates and is limited to 3 backups to save on disk space - downloaded UL ZIPs are automatically deleted unless changed in Mod Launcher Settings.

## Game and Mod Launcher Log File Locations
Log file locations are usually here:
(Game logs) C:/Users/YOURUSERNAME/AppData/LocalLow/The Fun Pimps/7 Days To Die/Player.log
(Game logs) C:/Users/YOURUSERNAME/AppData/LocalLow/The Fun Pimps/7 Days To Die/Player-prev.log
(Optional custom ML location): D:/UndeadLegacyLauncher/Subquakes_Undead_Legacy/BepInEx/LogOutput.log
(Optional custom ML location): D:/UndeadLegacyLauncher/update_debug.log

## Links
- [Undead Legacy Website](https://ul.subquake.com)
- [Patch Notes](https://ul.subquake.com/patch-notes)
- [Mod Download](https://ul.subquake.com/download)
- [Mod Launcher Download](https://github.com/SM1ThaYe/UndeadLegacyModLauncher/releases/latest)

© 2026 SMiThaYe & Subquake
