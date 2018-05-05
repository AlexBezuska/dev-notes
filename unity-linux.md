# Unity for Linux


## How to install

[Unity on Linux: Release Notes and Known Issues](https://forum.unity.com/threads/unity-on-linux-release-notes-and-known-issues.350256/)

### 2018 
[Download 2018.2.0b2](https://beta.unity3d.com/download/7b8938f7fa83/public_download.html) | [dev forum post](https://forum.unity.com/threads/unity-on-linux-release-notes-and-known-issues.350256/page-2)

[Download 2018.1.0f2](https://beta.unity3d.com/download/170f0691b973/public_download.html) | [dev forum post](https://forum.unity.com/threads/unity-on-linux-release-notes-and-known-issues.350256/page-2)

[Download 2018.2.0b2](https://beta.unity3d.com/download/7b8938f7fa83/public_download.html) | [dev forum post](https://forum.unity.com/threads/unity-on-linux-release-notes-and-known-issues.350256/page-2)

[Download 2018.1.0b1]( https://beta.unity3d.com/download/77a142ac9989/public_download.html) | [dev forum post](https://forum.unity.com/threads/unity-on-linux-release-notes-and-known-issues.350256/page-2)

[Download 2018.1.0b8](https://beta.unity3d.com/download/ee2fb9f9da52/public_download.html) | [dev forum post](https://forum.unity.com/threads/unity-on-linux-release-notes-and-known-issues.350256/page-2)


### 2017
[Download 2017.4.0f1](https://beta.unity3d.com/download/0ec691fce5c2/public_download.html) | [dev forum post](https://forum.unity.com/threads/unity-on-linux-release-notes-and-known-issues.350256/page-2)

[Download 2017.4.2f2](https://beta.unity3d.com/download/79b540374219/public_download.html) | [dev forum post](https://forum.unity.com/threads/unity-on-linux-release-notes-and-known-issues.350256/page-2) 

[Download 2017.4.2f2](https://beta.unity3d.com/download/79b540374219/public_download.html) | [dev forum post](https://forum.unity.com/threads/unity-on-linux-release-notes-and-known-issues.350256/page-2) 

[Download 2017.3.1f1](https://beta.unity3d.com/download/aea5ecb8f9fd/UnitySetup-2017.3.1f1) | [dev forum  post](https://forum.unity.com/threads/unity-on-linux-release-notes-and-known-issues.350256/page-2)

[Download 2017.2.1f1](https://beta.unity3d.com/download/ce9f6a0436e1+/public_download.html) | [dev forum post](https://forum.unity.com/threads/unity-on-linux-release-notes-and-known-issues.350256/page-2)

[Download 2017.3.0p2](http://beta.unity3d.com/download/7807bc63c3ab/public_download.html) | [dev forum post](https://forum.unity.com/threads/unity-on-linux-release-notes-and-known-issues.350256/page-2)

[Download 2017.3.0f1](http://beta.unity3d.com/download/3c89f8d277f5/public_download.html) | [dev forum post](https://forum.unity.com/threads/unity-on-linux-release-notes-and-known-issues.350256/page-2)

[Download 2017.2.0f3](http://beta.unity3d.com/download/ee86734cf592/public_download.html) | [dev forum post](https://forum.unity.com/threads/unity-on-linux-release-notes-and-known-issues.350256/page-2)

[Download 2017.1.2f1](http://beta.unity3d.com/download/7598623e6ed6/public_download.html) | [dev forum post](https://forum.unity.com/threads/unity-on-linux-release-notes-and-known-issues.350256/page-2)

[Download 2017.2.0f1](http://beta.unity3d.com/download/ad31c9083c46/public_download.html) | [dev forum post](https://forum.unity.com/threads/unity-on-linux-release-notes-and-known-issues.350256/page-2)

[Download 2017.2.0b1]( http://beta.unity3d.com/download/fd37f3680b5f/public_download.html) | [dev forum post](https://forum.unity.com/threads/unity-on-linux-release-notes-and-known-issues.350256/)

[Download 2017.1.1f1](http://beta.unity3d.com/download/f4fc8fd4067d/public_download.html) | [dev forum post](https://forum.unity.com/threads/unity-on-linux-release-notes-and-known-issues.350256/)

[Download 2017.2.0b6](http://beta.unity3d.com/download/2b451a7da81d/public_download.html) | [dev forum post](https://forum.unity.com/threads/unity-on-linux-release-notes-and-known-issues.350256/)



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
