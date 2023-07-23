![](https://raw.githubusercontent.com/Oghma-Infinium/Fahluaan/main/images/Banner.webp)

<p align="center">
  [ <a href="https://www.nexusmods.com/skyrimspecialedition/mods/87820">Nexus</a> |
  <a href="https://github.com/Oghma-Infinium/Fahluaan/blob/main/README.md">Installation</a> |
  <a href="https://github.com/Oghma-Infinium/Fahluaan/blob/main/GAMEPLAY.md">Gameplay Guide</a> |
  <a href="https://github.com/Oghma-Infinium/Fahluaan/blob/main/CHANGELOG.md">Changelog</a> |
  <a href="https://loadorderlibrary.com/lists/fahluaan">Modlist</a> |
  <a href="https://github.com/Oghma-Infinium/Fahluaan/blob/main/Documentation/FAQ.md">FAQ</a> |
  <a href="https://github.com/Oghma-Infinium/Fahluaan/blob/main/Documentation/NPCs.md">NPCs</a> |
  <a href="https://ko-fi.com/aljoxo">Ko-fi</a> | 
  <a href="patreon.com/aljoxo">Patreon</a> ]
</p>

---

# Installation

**Modlist Support: [Waking Dreams](https://discord.gg/4WwqfK5yHg)**

***Fahluaan requires the full AE upgrade, which means you must purchase the AE edition of the game for the list to function.***

# Contents
- [Installation](#installation)
- [Contents](#contents)
  - [Introduction](#introduction)
    - [System Requirements](#system-requirements)
  - [Installation](#installation-1)
    - [Pre-Installation](#pre-installation)
      - [Installing Microsoft Visual C++ Redistribution Package](#installing-microsoft-visual-c-redistribution-package)
      - [Pagefile and crash prevention](#pagefile-and-crash-prevention)
      - [Setting Shader Cache Size](#setting-shader-cache-size)
      - [Steam Setup](#steam-setup)
      - [Game Language](#game-language)
      - [Installing Creation Club Content](#installing-creation-club-content)
    - [Wabbajack Installation](#wabbajack-installation)
      - [Installing Wabbajack](#installing-wabbajack)
      - [Downloading and Installing Fahluaan](#downloading-and-installing-fahluaan)
    - [Problems with installation](#problems-with-installation)
  - [Post-Installation and Optional Setup](#post-installation-and-optional-setup)
    - [Game Folder](#game-folder)
    - [Antivirus Exceptions](#antivirus-exceptions)
    - [Widescreen Fixes](#widescreen-fixes)
    - [Controller and Gamepad Setup](#controller-and-gamepad-setup)
    - [Optional Tweaks](#optional-tweaks)
    - [Performance](#performance)
  - [Playing the List](#playing-the-list)
    - [Starting the Game](#starting-the-game)
    - [In-Game MCM options](#in-game-mcm-options)
    - [Note about Survival Mode](#note-about-survival-mode)
    - [Note For Content Creators](#note-for-content-creators)
  - [Updating the modlist](#updating-the-modlist)
    - [Tweaking the Game Settings](#tweaking-the-game-settings)
      - [Performance INI Options](#performance-ini-options)
      - [BethINI](#bethini)
  - [Removing the Modlist](#removing-the-modlist)
  - [Contact](#contact)
  - [Credits and Thanks](#credits-and-thanks)

## Introduction

Fahluaan (fa·lu·an) is a comprehensive modlist that focuses on bringing the combat and gameplay of Skyrim to the modern age, without compromising on the original lore and vision of the Elder Scrolls Series. Meticulously balanced and full of handpicked content, new gear, spells, and quest mods that are designed to integrate seamlessly into the game.

The full modlist can be viewed [here](https://loadorderlibrary.com/lists/fahluaan).

You can find a summary of all relevant changes on the [Gameplay Guide](https://github.com/Oghma-Infinium/Fahluaan/blob/main/GAMEPLAY.md).

This work is licensed under a [Creative Commons Attribution-NonCommercial-ShareAlike 4.0 International License](https://creativecommons.org/licenses/by-nc-sa/4.0/).

### System Requirements

>  Please note these specs are the best idea of a baseline that I can provide at the current moment, based on feedback I have gotten from testers and my own experiences. In the future this will be updated depending on feedback received.


| Spec Category | My Specs (1440p) | Recommended (1080p) |
|     :---:    |     :---:     |     :---:     
| **CPU**   | R7 5800X |  R7 3700x / i5 10600k |
| **Video Card**    | 3080 | 3060 Ti / 2070 / 6700 XT |
| **Ram**    | 32gb (2x16) | 16gb (2x16) |
| **Storage**    | 970 EVO NVMe | SATA SSD |

Please note that the below numbers are current estimates and the actual may be larger or smaller depending on version.

Downloads: ~170 GB  
Install: ~210 GB  
Temp Files: ~40 GB (on OS drive)  
**TOTAL:** ~390 GB  

 > Wabbajack requires around 30 GB of space on your main OS drive for temporary and working files during the installation, this space is not counted towards the total install space of the list for sake of this guide, however Wabbajack roughly accounts for it in the UI.

## Installation

Installing Fahluaan is relatively easy and, if you have Nexus Premium, will be a simple waiting game. If you are updating the modlist, you can safely skip to the [updating section](#updating-the-modlist).

### Pre-Installation

These steps are only required for installing the Modlist for the first time. Additionally, many of these steps may be covered in other modlist installs, for new users I suggest reading through here regardless.

#### Installing Microsoft Visual C++ Redistribution Package

 1. Install [Visual C++ x64](https://aka.ms/vs/16/release/vc_redist.x64.exe) & [.Net Runtime v6 desktop x64](https://dotnet.microsoft.com/en-us/download/dotnet/6.0/runtime).
 2. Change Skyrim so it does not [automatically update](https://help.steampowered.com/en/faqs/view/71AB-698D-57EB-178C#disable).
 3. Right click on Skyrim SE and click on properties, untick the "Enable Steam Overlay while in-game."
 4. You also need to start the games to the main menu in order to download all the creations. **DO NOT SKIP THIS STEP, IF YOU DO SO WABBAJACK WILL FAIL**

#### Pagefile and crash prevention

Larger Skyrim modlists require a significant amount of memory, running out of memory **will** result in crashes and other potential issues. Due to Fahluaan's size and number of files required to be handled for the list, this step is **NOT** optional, I do not care how much RAM or VRAM you have, please do this step.

 To set up your pagefile:
 1. Press **Win Key + R**
 2. Type *sysdm.cpl ,3* and hit **ENTER**
 3. Navigate to *Performance* and click the box "Settings..."
 4. Click the *Advanced* tab at the top
 5. Under *Virtual Memory* click the box "Change..."
 6. Uncheck *Automatically manage* if it is checked
 7. Select your disk drive, ideally your fastest solid state drive
 8. Click the **Custom size:** button
 9. In the box next to **Initial Size (MB)** type `40960`
 10. In the box next to **Maximum Size (MB)** type `40960`
 11. Click the *Set* button
 12. Click *OK*
 13. Click *Apply*
 14. Click *OK*
 15. Restart your computer in order for your new pagefile to take effect.

#### Setting Shader Cache Size
 Additionally, if you have an NVIDIA GeForce Graphics Card, please do the following: 

 1. Right-click on your desktop and select **NVIDIA Control Panel**
 2. Navigate and click on **Manage 3D settings**. It is the 2nd one to the top.
 3. Scroll down in Global Settings until you see **Shader Cache Size**
 4. Double Click **Driver Default** to the right of Shader Cache Size and select **10 GB**
 5. Click **Apply** in the bottom right hand corner. 
 6. You may exit out of the application.
![](https://raw.githubusercontent.com/iAmMe27/Tahrovin/main/img/ShaderCache.png)

#### Steam Setup

 If you have your Steam Library in Program Files, read [this](https://github.com/LostDragonist/steam-library-setup-tool/wiki/Usage-Guide) and move it elsewhere. Locations such as Desktop, Documents, Downloads, OneDrive, etc. will cause issues with installing and playing the list.

#### Game Language

The English Steam version of Skyrim is the only supported version. I understand that this may be frustrating for non-English speaking users or users with the GOG/Bethesda.net versions, but due to the core file differences between the different versions, I am only able to support one game version.

 1. Right click on your Skyrim in Steam
 2. Click *Properties*
 3. Click *Language*
 4. Set the Language to English.

#### Installing Creation Club Content

 If you have never installed the Creation Club Content before, please do the following:
 1. Purchase the *Skyrim Anniversary Edition* Upgrade from Steam. If you do not do this, you can not install or play the list. 
   > **There is no work around for this and pirating this content will not work. If you pirate the content and come asking for assistance, you will be banned.**
 2. Once you have the Anniversary Edition bought, do the following steps below.
 3. In your Steam Library, right-click on the menu entry for Skyrim, select `Properties` and then select `Local Files`. Click `Verify Integrity of Game Files` and wait.
 4. Once this is completed, launch the game once from Steam. You may receive a prompt that your settings were detected or not detected, this does not matter, nor do any options you select here. Simply open the launcher and launch the game.
 5. Once the intro logo finishes displaying and the Skyrim logo appears, you should receive a prompt to "Download All Content?" Accept this option.
 6. If you did not receive a prompt to download, select the Creation Club option from the menu, and you should find a "Download All" prompt in there somewhere. If this message does not appear, you have not purchased the $20 Upgrade. Begin again from step 1.
 7. Wait for the download process to complete. Do **NOT** ALT-TAB during this process as it will cause the process to fail and you will have to start over again.
 8.  Proceed with the rest of the installation.


### Wabbajack Installation

#### Installing Wabbajack

Once you have completed pre-installation, download the [latest version of Wabbajack](https://github.com/wabbajack-tools/wabbajack/releases) on this github and place it in a folder such as `C:\Wabbajack`. **DO NOT place it in Program Files, User folders (such as Desktop, Documents, Downloads, OneDrive, etc.), or in your Skyrim's Steam folder**. I recommend placing it on an SSD as it will work quicker on there.

#### Downloading and Installing Fahluaan

Downloading and installing Fahluaan can take a while depending on your internet connection and computer. To install Fahluaan, complete the following steps.

**FAHLUAAN BETA RELEASE IS ONLY AVAILABLE ON THE [NEXUS PAGE](https://www.nexusmods.com/skyrimspecialedition/mods/87820).**

Until official release, please download the .wabbajack file from the above link.
1. Download the file called **Fahluaan** from the Files tab. You **DO NOT** need to download the other files on the page, unless Wabbajack fails to do it later on.
2. Use 7zip to extract the downloaded file. You should now see **Fahluaan.wabbajack**.
3. Doubleclick **Fahluaan.wabbajack**. Wabbajack should automatically open for you. If it does not, open the Wabbajack app manually and select the **Install from disk** option.
4. Proceed as usual from this point.

**THE BELOW INSTRUCTIONS ARE A PLACEHOLDER FOR OFFICIAL RELEASE, PLEASE REFER TO THE NEXUS INSTRUCTIONS ABOVE**

1. Open Wabbajack and click `Browse Modlists`
2. Press the download button on Fahluaan and wait for it to download.
3. Set the installation folder to be somewhere like C:\Games\Fahluaan. **DO NOT place it in Program Files, User folders (such as Desktop, Documents, Downloads, etc.), or in your Skyrim's Steam folder**
> The download location does not need to be on a SSD, but it makes installing faster.
4. Press the play button to begin.
5. Turn on your favorite show or a nice long video essay Wabbajack does its thing. Alternatively read through this readme again.
6. If the installation is successful, then rejoice and move onto [post installation](#post-installation-and-optional-setup). If the installation is unsuccessful, follow what is below or join the [discord server](https://discord.gg/WakingDreams) for support.

Sometimes Google Drive and MEGA will experience bandwidth caps, so below I have included the links to the files that require them.
- [High Poly Head](https://drive.google.com/file/d/15_0njBUjHKidNnJPmLXEygzGVWsA3Zbq)

### Problems with installation

It is possible that you may encounter an error with Wabbajack when installing. Some common issues are listed below.

- Could not download **X**:
	- Big files can fail to download due to connection issues. You can either run wabbajack again or download the file manually. If you decide to manually download it, make sure to place it in the same place as the other downloads.

- **X** is not a whitelisted download:

	 - This may happen when I update the modlist. Please check if there is a new update or wait until you see a release ping.

- Wabbajack could not find my game folder:

	- Either buy the game or go back to the [Pre-Installation](#pre-installation) step.

- Antivirus reports a virus:
	- Windows 10/11 may automatically quarantine a key file which is needed for Mod Organizer. You can fix this by [adding an exclusion for Mod Organizer in windows defender](https://www.thewindowsclub.com/exclude-a-folder-from-windows-security-scan).

- Unable to download `Data_ccXXXXX - *.bsa` or `*.esp`:
	- This error means that there is an issue where Wabbajack is unable to hash your Creation Club Content. If you have followed the steps outlined under [Pre-Installation](#installing-creation-club-content), are not on a pirated copy of the game, and have verified your steam files, then it is very likely that Wabbajack or Bethesda has messed up the hashing for these files. If this is the case, please wait for it to be resolved before continuing to download the list.

- Unable to download `Skyrim_Default.ini`:
 - This error means you failed to follow the readme. Go back to the [game language](#game-language) section and set your game language to English.

## Post-Installation and Optional Setup

### Game Folder

Fahluaan uses a Wabbajack feature called Stock Game to keep your Skyrim installation clean. All the files that you need to run the list are in a folder called `Stock Game`. You don’t need to copy anything at all.

### Antivirus Exceptions

Generally speaking, using Windows Defender is advised as it is a solid antivirus software that will have minimal interference with the game. Antivirus programs can be notorious for false flagging MO2's VFS as problematic, causing crashes or other problems. Antivirus programs like BitDefender, Norton, and Webroot are especially aggressive, and you will very likely need to fully remove them from your PC in order to actually launch the game through MO2.

If you use Windows Defender, it is advised that you set up an Exception for the modlist. To do this follow these steps.
 1. Press the Windows Key.
 2. Type "Windows Defender" in the search bar and select "Windows Security".
 3. Click on "Virus & threat protection" in the left pane.
 4. Click the "Manage settings" option under "Virus & threat protection settings".
 5. Scroll down to "Exclusions" and click "Add or remove exclusions".
 6. Windows Defender will prompt you with a run as administrator screen, just hit yes.
 7. Click the "Add an exclusion" button at the top and choose "Folder".
 8. Navigate to your Install folder for the list and click "Select Folder".
 9. **(OPTIONAL)** You can repeat these steps for the other executables:
    - ModOrganizer.exe (`[Path to Modlist]\ModOrganizer.exe`)
    - Nemesis Unlimited Behavior Engine.exe (`[Path to Modlist]\mods\Project New Reign - Nemesis Unlimited Behavior Engine\Nemesis_Engine\Nemesis Unlimited Behavior Engine.exe`)
    - Synthesis.exe (`[Path to Modlist]\tools\Synthesis\Synthesis.exe`)

### Widescreen Fixes

Fahluaan offers some mods to provide Ultrawide and Widescreen Support. Under the **Ultrawide Patches** Separator in MO2 you will find some mods that you will want to activate if you are playing on Ultrawide or Widescreen resolutions (21:9 or 32:9).

### Controller and Gamepad Setup

Fahluaan offers some mods to provide support for individuals who wish to play with a controller or gamepad. In order to set it up correctly please follow these steps:
 1. Under the **Gamepad Support** Separator in MO2, activate the mods under it.
 2. Refer to the controlmap and set up your binds in the in-game Mod Configuration Menus as some of these can not be set in advanced.
   - [Keybinds](https://github.com/Oghma-Infinium/Fahluaan/blob/main/images/Keybinds.png)
   - [Gamepad](https://github.com/Oghma-Infinium/Fahluaan/blob/main/images/Gamepad.png)

### Optional Tweaks

This section will cover the following Optional Tweaks that are included as a part of the modlist. Please note that if you do any of these tweaks, it is in your best interest to share this information when reporting any potential bugs that you encounter when playing the modlist.
 1. **Yet Another Music Merge - Content Creator Version**: Read more [here](#note-for-content-creators).
 2. **Content Creator Music Patches**: Read more [here](#note-for-content-creators).
 3. **Blade and Blunt - Vanilla Difficult Modifiers**: Restores Vanilla Difficulty Multipliers for those who want an easier experience.
 4. **QuickLoot RE - Disable in Combat**: An edited `.toml` file for QuickLoot RE to disable the loot box from appearing while in combat.
 5. **No Survival Camera Effects**: Removes the image space effects added by CC Survival Mode.
 6. **Vigilant - No Enemy Blur**: Removes the image space blur effects that some enemies produce in Act 3 of Vigilant.
 7. **Lux - Brighter Templates**: Overwrites Lux's base lighting templates with brighter ones, for those who find interiors to be too dark.
 8. **NeverNude**: (Enabled by default), Removes Female nudity from the list, the list does not support male nudity without modifications.

In Addition to the optional tweaks, for those with arachnophobia and/or entomophobia, the `Insects Begone` Separator contains some mods to remove most of the spider and insect adjacent models and enemies from the list.

 ### Performance

 Supported performance options for Fahluaan, more information is written in the notes in MO2. If you choose to use the performance ENB Preset, make sure to also read the [performance ini options](#performance-ini-options) section. Sound Fix for Large Sector Drives can be enabled if you have a large sector drive, I have heard conflicting accounts on whether or not there is a downside to having it enabled on non-Large sector drives. If in doubt, just enable the mod.

## Playing the List

### Starting the Game
 - Head over to the installation folder and locate an executable named ModOrganizer.exe and launch it.
 - **(Optional)** For those of you with arachnophobia, the list includes a mod called *bingus hates spiders.esp*, this is my personal patch that removes spiders from the leveled list and replaces spiders with other creatures within the list. It also has a few other tweaks to make it a bit more in depth than something like *Insects begone*.

 1. Launch the "Fahluaan" Executable in MO2.
 2. Click "New Game".
 3. After about 30 seconds, press `esc` and open the Mod Configuration Menu.
 4. Navigate to the Skyrim Unbound Menu and customize your starting equipment.
 5. Once you are satisfied, leave the MCM and hit `Enter` to begin Character Creation.
 6. After Character Creation finishes, you will get a popup to select your Pronouns and the MCM Recorder will begin to run, make sure to choose "STAY HERE" from the popup after Pronouns, otherwise you could cause some issues from the overlap of Skyrim Unbound's scripts and MCM configuration. (Note: Sometimes the Pronouns popup will occur twice, just select the same option both times).
 7. Once the MCM Recorder finishes (you will get a notification), you can proceed to customize any other MCMs, then press `Enter` and choose "Continue".

### In-Game MCM options

 - **Skyrim Unbound**: Choose your Standing Stone, starting location, starting equipment, starting wealth, etc. By default, the player is set to become Dragonborn, so if you do not want that for some reason, turn it off. **I highly suggest against choosing to not become Dragonborn, as it will lock you out of a lot of content within the list.**
 - **Better Third Person Selection**: Enable or Disable certain Filters here (ex: Stealing Only WHile Undetected).
 - **Improved Alternate Conversation Camera**: Edit the dialogue view. Can also be done through the `.ini` file in Mod Organizer.
 - **OBody Standalone**: Set OBody menu key here. (Default: `;`).
 - **Simple Offence Suppression**: Toggle SOS off or on. Should be unnecessary in the vast majority of cases.
 - **SmoothCam**: Default preset is a slightly modified version of Vanilla Enhanced 2.0.
 - **Ultimate Immersion Toggle**: Hide UI Keybind. (Default: `X`).
 - **Weapon Styles**: If you change where your weapon sheathes via IED, then change the animation here so it matches correctly.

### Note about Survival Mode

Survival Mode is **NOT** enabled by default, to do so you must do it in the in-game settings menu accessed via the System Page.
Fast Travel is **disabled** by default when Survival Mode is **enabled**. If you would like to have Fast Travel active while playing with Survival Mode, navigate to the `SurvivalModeImproved.ini` located at `[Path to Modlist]\mods\Survival Mode Improved - Settings\SKSE\Plugins` and change the line `bDisableFastTravel=1` to `bDisableFastTravel=0`.

### Note For Content Creators

[Yet Another Music Merge](https://www.nexusmods.com/skyrimspecialedition/mods/48725) includes some songs from Nir Shor which are not allowed to be played on Twitch or YouTube due to DMCA rules. The list includes a version of YAMM that does not have the copyrighted music and fixed patches that can be used for those who make content. While I can not promise this will completely avoid any and all DMCA claims, it should remove the key offenders.

## Updating the modlist

Versioning for the list will adhere to the following format: `MAJOR.MINOR.PATCH`.
 - `MAJOR`: Any release with a number change here will be considered a major update as at least 1 area of the list was massively overhauled. These updates with **NEVER** be save safe.
 - `MINOR`: Any release with a number change here will be considered a minor update, these updates will usually not be save safe, unless otherwise specified.
 - `PATCH`: Any release with a number change here will be considered a patch, these updates should be save safe and will be used primarily for bugfixes.
 - In some rare cases you may see a fourth slot be used, which I will refer to as `HOTFIX`. These list "updates" will be used if the list needs to be recompiled for any reason. There will be no changes in these "updates" as they are purely for maintenance.
Before updating, please check the [changelog](https://github.com/Oghma-Infinium/Fahluaan/blob/main/CHANGELOG.md) and back up your saves. You may need to start a new game after certain updates.
Updating is like installing the list. Simply make sure your paths are the same and tick the `overwrite existing modlist` button. **Note**: Any mods you have added will be deleted when updating. To make sure that Wabbajack does not delete your added mods upon updating, prefix your mods with **[NoDelete]**.

**ALWAYS** back up saves before an update. Because of the method Wabbajack uses to include the start save, any save within the profile will be wiped. 

*Please make sure you back up your saves if you plan on continuing a playthrough across a **save safe** update.*

*Please make sure to back up your RaceMenu Presets when updating. You can place them in the `[NoDelete] Fahluaan RaceMenu Presets` mod.*

### Tweaking the Game Settings

#### Performance INI Options

This section requires a rewrite - Stay tuned.

#### BethINI

Before running BethINI please make sure that your paths are correctly set. I also suggest backing up the original `.ini` files just in case. 

 - **Game**: `Skyrim Special Edition`
 - **Game Path**: `[Path to Modlist]\Stock Game`
   - example: `F:\Fahluaan\Stock Game`
 - **Mod Organizer**: `[Path to Modlist]` 
   - example: `F:\Fahluaan`
 - **INI Path**: `Mod Organizer > Fahluaan - Default`

To get some more FPS, tweak the following value in the detail section in BethINI.

- `Shadow Resolution`: 2048
- `Ambient Occlusion`: Either use this or the ENB version. The ENB version is more intensive. Do not have both turned on.
- `Remove Shadows`: I really don’t recommend turning this on, but if you must, then you can.
    - Do make note that if you remove shadows you must also disable the [Shadow Boost](https://www.nexusmods.com/skyrimspecialedition/mods/73133) mod in the ENB Menu.

## Removing the Modlist
Simply delete the folder. Congratulations, you have uninstalled Fahluaan.

## Contact

Please check the [FAQ](https://github.com/Oghma-Infinium/Fahluaan/blob/main/Documentation/FAQ.md) first if you have any issues. **PLEASE DO NOT DM ME ON DISCORD.** If you have an issue with the list, please join the [Waking Dreams](https://discord.gg/4WwqfK5yHg) discord server for support.


## Credits and Thanks

- _YOU_ for reading this.
- [Bingus](https://ko-fi.com/beangas) for ENB tweaking, asset editing, mod page screenshots, and branding art for Fahluaan (Logo, Banner, and Splash).
- Curly for the original iteration of Ascensio that provided me a baseline to work off of.
- [iAmMe27](https://ko-fi.com/iamme27) for general modding, documentation, and WJ assistance.
- A Helping Hand, AnnieDOS, Chanka, Felivath, Izol, Maelstrom, Roxiie, and Vigo for their time and effort playtesting, providing feedback, and miscellaneous help.
- [Jolly Co-Operators](https://discord.gg/jolly-coop) and [Cacophony](https://www.patreon.com/cacophony1979) for their wonderful community that inspired me to start modding more.
- JustThatKing, jdsmith2816, and Total for their feedback on graphics and other things.
- Bethesda Game Studios for Skyrim and the Creation Kit.
- [ElminsterAU](https://www.patreon.com/ElminsterAU) and the xEdit team for SSEEdit.
- Noggog for Mutagen and Synthesis.
- Halgari and the WJ Team for this amazing platform.
- [LivelyDismay](https://github.com/LivelyDismay) for his GuideBook and modding guides.
- [The Animonculory](https://github.com/The-Animonculory) for their modding guides.
- [Styyx](https://github.com/Styyx1) for assistance with scripting and backend work.
- [SimonMagus](https://www.patreon.com/simonmagus), [DeltaRider](https://www.patreon.com/Delta011), and the Simon Makes Mods Discord for many ideas and mod assistance.
- [Cosmofujia](https://www.patreon.com/fujiacosmo) for a significant amount of high quality Weapon Models.
- [Aelarr](https://www.nexusmods.com/skyrim/users/6843757) and Anreme for permissions to use some custom mods from The Owl Archives server.
