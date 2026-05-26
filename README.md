# Flashing-Lights--Grammar-Police-and-MDT
# Grammar Police - Flashing Lights Mod
=====================================
Author: Erin
Version: 1.0.0

Description
-----------
Adds a voice-controlled radio dispatch system to Flashing Lights. Use push-to-
talk voice commands or a clickable radio UI to transmit 10-codes and dispatch
signals. Includes configurable panic detection and keyboard emulation for
auto-typing codes in-game.

Features
--------
- Voice recognition: hold configurable PTT key (default: Left Control) and
  speak 10-codes (e.g., "ten four", "ten seventy eight", "code three")
- Radio UI panel: browse all codes by category — click to transmit or
  navigate with arrow keys + Enter/Space
- Key emulation: automatically types mapped key sequences for 10-1 through
  10-10 when a voice command or button is activated
- Panic detection: rapid-press the panic key (default: F) to trigger a
  10-78 dispatch with optional key sequence emulation
- Transmission overlay: shows your sent codes and simulated dispatch responses
- Config hot-reload: saves and applies settings in real time

Supported Voice Commands
------------------------
- 10-1 through 10-99 standard police codes
- Code 2 / Code 3 / Code 4
- Radio Check, Signal 1, Signal 2
- Natural phrases: "officer needs assistance", "request backup",
  "arrived on scene", "pursuit", "stolen vehicle", etc.

Controls
--------
Left Control (hold)  - Push-to-Talk (voice recognition)
F12                  - Toggle radio UI panel
F (press rapidly x3) - Trigger panic (10-78)

Installation
------------
1. Requires MelonLoader v0.7.3+ installed for Flashing Lights
2. Extract all files from the Mods folder into:
     E:\SteamLibrary\steamapps\common\Flashing Lights\Mods\
   (or your equivalent game install path)
3. Launch the game — mod loads automatically

Dependencies
------------
- FlashingLights.ModKit.Core.dll (included)
- WinRT.Runtime.dll (included — required for speech recognition)
- Microsoft.Windows.SDK.NET.dll (included — required for speech recognition)

Configuration
-------------
All settings are configurable from the ModKit settings menu in-game:
- Push-to-Talk key, Radio UI toggle key, Panic trigger key
- Voice recognition on/off, confidence threshold
- Key sequences for 10-1 through 10-10 (comma-separated key names)
- Transmission overlay display duration
- Verbose logging, auto-dispatch backup on events
- Panic press count and time window


# MDT Terminal - Flashing Lights Mod
====================================
Author: Erin
Version: 1.0.0

Description
-----------
Adds an in-vehicle Mobile Data Terminal (MDT) to Flashing Lights. The MDT
provides a police/fire/EMS role-play interface for managing charges, citations,
court sessions, and subject records directly from your patrol vehicle.

Features
--------
- Toggle MDT with F11 (configurable)
- Role detection: automatically changes color scheme based on your vehicle
  (Police = blue, Fire = red, EMS = green)
- CHARGES tab: select from US-style traffic, criminal, drug, and weapon charges
  and file them against a subject
- CITATIONS tab: issue traffic citations with fine amounts
- COURT tab: auto-adjudication system that processes pending charges with
  configurable intervals — includes guilty/not guilty/plea bargain outcomes
- RECORDS tab: search and review all filed charges and citations by subject name
- Automatically blocks game input while MDT is open

Controls
--------
F11 (default) - Toggle MDT open/close

Installation
------------
1. Requires MelonLoader v0.7.3+ installed for Flashing Lights
2. Extract all files from the Mods folder into:
     E:\SteamLibrary\steamapps\common\Flashing Lights\Mods\
   (or your equivalent game install path)
3. Launch the game — mod loads automatically

Configuration
-------------
- Edit config.txt in the Mods folder to set the court auto-session interval
  in minutes (e.g., "5" = every 5 minutes). Default: 5.
- Edit the MDTConfig.cs source and rebuild to change the toggle key or court
  interval.


