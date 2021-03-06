# Esports PCs

## Drive Configuration

Partition scheme:
- SSD:
  - C: ~150GB Windows
  - D: Rest (~350GB) NTFS `Comp Games ONLY`, with following directories:
    - `SteamLibrary`
    - `BattleNet`
    - `Riot Games`
    - `rocketleague`
    - `MOSS`
- HDD:
  - E: 1TB `Casual Games and Clips`, with following directories:
    - `Epic_HDD`
    - `Recordings`
    - `SteamLibrary`

## Apps

Note, do not install all of these games before taking the image. Only Call of Duty and Valorant are required because of kernel-level anticheat. You may need to ask a club member to install them for you, as Call of Duty costs money. If you own them, League of Legends and Rocket League are small enough to be on the image.

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
- Don't `Remember login emails & phone numbers`, clear saved login info
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
- Go back a level, then under `APP SETTINGS`, uncheck everything
- Uncheck `ENABLE AUTOMATIC UPDATES` in the top right

### GeForce Experience

Update to the latest Game-Ready driver. Will need to sign in with club Google account. Make sure to log out of browser afterwards and remove esports gmail as a sign-in option.

Hit ALT+Z, click settings, HUD Layout, turn Status indicator off. Same for performance.

Under recordings, set videos directory to `E:\Recordings`

Make sure to turn Instant Replay on before closing out (by hitting ALT+Z again)

### MOSS

Download x64 from [nohope.eu](https://nohope.eu/). Install [7-zip](https://www.7-zip.org/download.html). Extract with 7-zip, password `Moss`. Move `MOSS.exe` to `D:\`. Run and set to Rainbow Six in parameters. Close out. Open command prompt as admin and run `mklink /d "C:\Users\WSU Esports\Desktop\MOSS" D:\MOSS`


### NVIDIA Broadcast

Microphone Source: `Headset Microphone (HyperX Virtual Surround Sound)`
- Effects: `Noise Removal`, max strength

### Riot Launcher

When installing Valorant/LoL, install on `D:\Riot Games`

### Steam

Go to `Steam` in top left, click `Settings`:

__Account:__
- Check `Don't save account credentials on this computer`

__Interface:__
- `Select which Steam window appears when the program starts...`: `Library`
- Uncheck `Notify me about additions or changes to my games...` and `Run steam when my computer starts`

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

__System/Powwer & sleep:__
- Click additional power settings, and in the window that pops up, go to `Choose what the power buttons do` then `Change settings that are currently unavailable` and uncheck `Turn on fast startup (recommended)`

__Ease of Access/Interaction/Keyboard:__
- Turn literally everything off

__Personalization/Background:__
- Set our wallpaper (available on Google Drive or another system)

__Personalization/Colors:__
- `Choose your color`: `Dark`
- Transparency effects: `On`
- Custom accent color: `#047A40`
- Check `Start, taskbar, and action center`
- Check `Title bars and window borders`

__Personalization/Lock screen:__
- Set our wallpaper (available on Google Drive)

__Accounts/Sign-in options:__
- Password: set to empty string
- Require sign-in: `never`


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

## Other Configuration

- Log out of everything
- Clear all browsing data on all browsers
- When everything above is done, go to Task Manager > Startup and disable everything except for Discord and Vanguard
- Remove all desktop icons except for the MOSS folder and Recycle Bin
- Set Chrome to the default browser
- Delete everything from Downloads
- Empty the recycle bin
- Launch `User Account Control Settings` and drag the slider to the bottom
- Copy the deepfreeze installer to Music (don't install until after deploying the image)

# POST-DEPLOYMENT

1. Set refresh rate back to 144Hz
2. Check for windows updates (hopefully catch drivers)
3. Launch G hub and do the following:
  -  Click mouse in middle
  -  Click slot 1
  - Set desktop default to slot 1
  - Turn DPI lighting always on
4. Make sure D: and E: are configured properly. Use `Create and format hard disk partitions`. You may need to do any of the following:
  - Extend D:
  - Reletter either or both D: and E:
  - Rename E:
  - Recreate Steam libraries
  - Reset GeForce Experience recording directory (Remember to start instant replay afterwards)
6. Reboot
7. Install deepfreeze
