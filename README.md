# Esports PCs

## Drive Configuration

Partition scheme:
- SSD:
  - C: ~150GB Windows
  - D: Rest (~350GB) NTFS `Comp Games ONLY`, with following directories:
    - `SteamLibrary`
    - `BattleNet`
    - `RiotGames`
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

### Battle.net

__Settings/Downloads:__
- Default Install Directory: `D:\BattleNet\`
- Turn off automatically create desktop icons

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

### Epic Games

Log in, do the following, then log out:
- Click profile in the top right, then settings
  - Uncheck everything except enable cloud saves

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

Hit ALT+Z, click settings, HUD Layout, turn Status indicator off

### NVIDIA Broadcast

Microphone Source: `Headset Microphone (HyperX Virtual Surround Sound)`
- Effects: `Noise Removal`, max strength

### Riot Launcher

When installing Valorant/LoL, install on D:

### Steam

Go to `Steam` in top left, click `Settings`:

__Account:__
- Check `Don't save account credentials on this computer`

__Interface:__
- `Select which Steam window appears when the program starts...`: `Library`
- Uncheck `Notify me about additions or changes to my games...`

__Downloads__:
- Check `Display download rates in bits per second`
- Click `STEAM LIBRARY FOLDERS`, then
  - Add library folder on `D:` and `E:` (should auto-create `\SteamLibrary`)
  - Make `E:` default


### Windows Settings

__System/Display/Advanced display settings:__
- Refresh rate: 144Hz (or whatever's closest)

__System/Sound:__
- Output device: `Headset Earphone (HyperX Virtual Surround Sound)`
- Input device: `Microphone (NVIDIA Broadcast)`

Click `Manage sound devices`, under output disable `ZOWIE XL LCD (NVIDIA High Definition Audio)` and `Speakers (NVIDIA Broadcast)`

__System/Ease of Access/Interaction/Keyboard:__
- Turn literally everything off

__Taskbar:__
- Right click taskbar and turn of `Show Cortana button` and `Show Task View button`
- Pins, from left to right:
  - File Explorer
  - Google Chrome
  - Firefox
  - Discord
  - Steam
  - Epic Games
  - Battle.net
  - Ubisoft Connect
  - Riot Games
  - Spotify
  - ASTRO Command Center

__Start Menu:__
- Unpin everything
