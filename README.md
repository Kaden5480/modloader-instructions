# modloader-instructions
Install instructions for BepInEx and MelonLoader.

# Overview
- [BepInEx (Windows)](#bepinex-windows)
- [BepInEx (Linux)](#bepinex-linux)
- [MelonLoader (Windows)](#melonloader-windows)
- [MelonLoader (Linux)](#melonloader-linux)

# BepInEx (Windows)
- Download the latest stable win_x64 version of BepInEx
[here](https://github.com/BepInEx/BepInEx/releases).
- Find your game directory, this is most easily done by going to the game in steam,
  pressing the settings for the game (⚙️), selecting "Manage", then "Browse local files".
- Extract the contents of `BepInEx_win_x64_<version>.zip` into your game directory.
- You should now have files/directories such as `BepInEx` and `winhttp.dll`
  in the same place as `UnityPlayer.dll`.
- Start the game so BepInEx can generate other necessary files for modding.
- Close the game.

# BepInEx (Linux)
## Prerequisites
- Install [protontricks](https://pkgs.org/download/protontricks).

## Prefix configuration
- Open protontricks.
- Select the game you intend to mod.
- Select "Select the default wineprefix" and press "OK".
- Select "Run winecfg" and press "OK".
- Change "Windows Version" to "Windows 10" and press "Apply".
- Switch to the "Libraries" tab.
- Where it says "New override for library:", choose "winhttp", press "Add", then press "OK".

## Installing BepInEx
- Download the latest stable win_x64 version of BepInEx
[here](https://github.com/BepInEx/BepInEx/releases).
- Find your game directory, this is most easily done by going to the game in steam,
  pressing the settings for the game (⚙️), selecting "Manage", then "Browse local files".
- Extract the contents of `BepInEx_win_x64_<version>.zip` into your game directory.
- You should now have files/directories such as `BepInEx` and `winhttp.dll`
  in the same place as `UnityPlayer.dll`.
- Start the game so BepInEx can generate other necessary files for modding.
- Close the game.

# MelonLoader (Windows)
## Prerequisites
- Install Microsoft Visual C++ 2015-2022 Redistributable from
[this link](https://aka.ms/vs/17/release/vc_redist.x64.exe)
or by running `winget install Microsoft.VCRedist.2015+.x64` in cmd/powershell/terminal.
- Install Microsoft .NET Desktop Runtime 6 from
[this link](https://download.visualstudio.microsoft.com/download/pr/d0849e66-227d-40f7-8f7b-c3f7dfe51f43/37f8a04ab7ff94db7f20d3c598dc4d74/windowsdesktop-runtime-6.0.29-win-x64.exe)
or by running `winget install Microsoft.DotNet.DesktopRuntime.6` in cmd/powershell/terminal.

## Installing MelonLoader
- Download the latest nightly MelonLoader build
[here](https://nightly.link/LavaGang/MelonLoader/workflows/build/alpha-development/MelonLoader.Windows.x64.CI.Release.zip).
- Find your game directory, this is most easily done by going to the game in steam,
  pressing the settings for the game (⚙️), selecting "Manage", then "Browse local files".
- Extract the contents of the downloaded zip file into your game directory.
- You should now see files/directories such as `MelonLoader` and `version.dll`
  in the same place as `UnityPlayer.dll`.
- Run the game and then quit it.
- If MelonLoader was installed correctly, you should notice new directories
  in your game directory (such as Mods).

# MelonLoader (Linux)
## Prerequisites
- Install [protontricks](https://pkgs.org/download/protontricks).

## Prefix configuration
- Open protontricks.
- Select the game you intend to mod.
- Select "Select the default wineprefix" and press "OK".
- Select "Run winecfg" and press "OK".
- Change "Windows Version" to "Windows 10" and press "Apply".
- Switch to the "Libraries" tab.
- Where it says "New override for library:", choose "version", press "Add", then press "OK".

## Installing prefix components
- Open protontricks.
- Select the game you intend to mod.
- Select "Select the default wineprefix" and press "OK".
- Select "Install Windows DLL or component" and press "OK".
- Select the packages "dotnetdesktop6" and "vcrun2019" and press "OK".
- You may get errors that say checksums didn't match, you can ignore these. When
  you are asked to "Continue anyway", choose "Yes".

## Installing MelonLoader
- Download the latest nightly MelonLoader build
[here](https://nightly.link/LavaGang/MelonLoader/workflows/build/alpha-development/MelonLoader.Windows.x64.CI.Release.zip).
- Find your game directory, this is most easily done by going to the game in steam,
  pressing the settings for the game (⚙️), selecting "Manage", then "Browse local files".
- Extract the contents of the downloaded zip file into your game directory.
- You should now see files/directories such as `MelonLoader` and `version.dll`
  in the same place as `UnityPlayer.dll`.
- Run the game and then quit it.
- If MelonLoader was installed correctly, you should notice new directories
  in your game directory (such as Mods).
