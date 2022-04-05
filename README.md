# Esports PCs

## Drive Configuration

Partition scheme:
- SSD:
  - C: ~150GB Windows
  - D: Rest (~350GB) NTFS `Comp Games ONLY`, with following directories:
    - `SteamLibrary`
    - `BattleNet`
- HDD:
  - E: 1TB `Casual Games and Clips`, with following directories:
    - `Epic_HDD`
    - `Recordings`
    - `SteamLibrary`

## Apps

Comp Games (Install to D\:, directory respective to launcher):
- Steam
  - CS:GO
  - Rainbow Six: Siege
  - Rocket League
- Epic
  - Rocket League
- Riot
  - League of Legends
  - Valorant
- Battle.net
  - CoD: Vanguard
  - Overwatch

Other Apps:
- ASTRO Command Center
- Discord
- Firefox
- Google Chrome
- Logitech G HUB
- Nvidia GeForce Experience
- NVIDIA Broadcast
- Spotify
- Ubisoft Connect

__NOTE:__ Valorant and Call of Duty both use kernel-level anticheats. They _cannot_ be installed on the same systems. Row C (closest to windows) should have CoD, the rest Valorant.

## Notable Configs

### Discord

__App Settings/Voice & Video:__
- Input Device: `Microphone (NVIDIA Broadcast)`
- Output Device: `Headset Earphone (HyperX Virtual Surround Sound)`

__App Settings/Notifications:__
- Enable Taskbar Flashing: Off
- All sounds off except `Incoming Ring`

__App Settings/Windows Settings:__
- Open Discord: On
- Start Minimized: On
- Minimize to Tray: Off

__Activity Settings/Game Overlay:__
- Enable in-game overlay: Off

### Google Chrome

Make default browser. Ensure WSU Esports gmail is logged out and not available to sign in (go to log-in page and remove account)

### Logitech G HUB

Click the mouse in the middle to edit `DESKTOP: Default` profile. Make the following changes:
- Set sensitivity options to 400, 800, 1000, 1500
- Bind `DPI Up` (G8) to `F13`
- Bind `DPI Down` (G7) to `F14`
- Bind `Onboard Profile Cycle` (G9) to `DPI Cycle`
- Set lighting on primary and logo to `#00FF3F`, fixed

Back out to the main menu, then click the settings gear in the top right. Click `MY GEAR`, then the mouse in the bottom middle.
- Enable `ON-BOARD MEMORY MODE` and set `SLOT 1` to `DESKTOP DEFAULT`, and select slot 1.
- Enable DPI Lighting Always On and enable Device Startup Effect

### GeForce Experience

Update to the latest Game-Ready driver. Will need to sign in with club Google account. Make sure to log out of browser afterwards and remove esports gmail as a sign-in option.

### NVIDIA Broadcast

Microphone Source: `Headset Microphone (HyperX Virtual Surround Sound)`
- Effects: `Noise Removal`, max strength

### Windows Settings

__System/Display/Advanced display settings:__
- Refresh rate: 144Hz (or whatever's closest)

__System/Sound:__
- Output device: `Headset Earphone (HyperX Virtual Surround Sound)`
- Input device: `Microphone (NVIDIA Broadcast)`

Click `Manage sound devices`, under output disable `ZOWIE XL LCD (NVIDIA High Definition Audio)` and `Speakers (NVIDIA Broadcast)`

__System/Ease of Access/Interaction/Keyboard:__
- Turn literally everything off
