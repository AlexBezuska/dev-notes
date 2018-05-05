# Unity for Linux


## How to install

[Unity on Linux: Release Notes and Known Issues](https://forum.unity.com/threads/unity-on-linux-release-notes-and-known-issues.350256/)

## Dependencies

Here is a script to install dependencies

```bash
sudo apt install  gconf-service  lib32gcc1  lib32stdc++6  libasound2  libc6 libc6-i386  libcairo2 libcap2  libcups2  libdbus-1-3  libexpat1  libfontconfig1  libfreetype6  libgcc1 libgconf-2-4  libgdk-pixbuf2.0-0  libgl1-mesa-glx libgl1 libglib2.0-0 libglu1-mesa libglu1 libgtk2.0-0  libnspr4  libnss3  libpango1.0-0  libstdc++6 libx11-6  libxcomposite1  libxcursor1  libxdamage1  libxext6 libxfixes3 libxi6  libxrandr2  libxrender1 libxtst6 zlib1g  debconf
```


## Discovered Issues (not yet solved)

**v2017.3.1f1**
- No support for installing Vuforia AR/VR toolkit [Vuforia Downloads Page](https://developer.vuforia.com/downloads/sdk)
- Anchor presets `Alt` and `Shift` key modifiers do not work [Unity Manual: Basic Layout](https://docs.unity3d.com/Manual/UIBasicLayout.html)
- Automatic API Updater - both options `I Made a Backup, Go Ahead!` and `No Thanks!` result in editor closing and no changes beign made
