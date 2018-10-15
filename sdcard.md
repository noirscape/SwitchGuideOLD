---
layout: default
title: Setting up your SD card and bootkit
---

### Setting up your sd card

When Hekate updates, it is advised to replace all folders except for the `switch` and `Nintendo` folders with those from a newly generated zip from sdsetup.com (using the URL provided to you from What You Will Need).
{: .info-box}

1. Turn off your Switch and put your microSD card in your computer.
2. Copy over all files in the `sd` folder from the sdsetup.com zip to the root of your Switch's microSD card.
3. Safely remove your microSD card and plug it back in your Switch.

---

### Making your bootkit

You will not have to create this bootkit if you are running Android or ChromeOS.\\
[Continue to OS-Specific preparations if you use Android or chromeOS]({{ site.url }}/os-specific-preparations/android.html){: .a-table}.
{: .info-box}

You will only have to create this bootkit once. When an update for hekate releases, generate a new zip file on sdsetup.com (using the URL provided to you from What You Will Need) and replace `payload.bin` with the file starting with `hekate_ctcaer` in the `payloads` folder (rename it to `payload.bin` and copy it to the `bin` folder).
{: .info-box}

1. Extract the sdsetup.com zip to a folder.
2. Make a new folder called `bootkit`.
3. In the `bootkit` folder, place `boot_cfw_win32.bat`, `boot_cfw_win64.bat` and `boot_macOS-Linux.sh`.
4. In the `bootkit` folder, make a folder called `bin`.
5. In the `bin` folder, place `fusee-launcher.py` and `intermezzo.bin`.
6. From the sdsetup.com zip, copy the following files to the `bin` folder:
  - From the `pc` - > `tegrarcmsmash` folder copy both exes in the directories to the `bin` folder. Name the one from the `Win32` folder `TegraRcmSmash_Win32` and the one in the `x64` folder `TegraRcmSmash_Win64`. (If you have file extensions enabled, make sure that they still end in .exe).
  - From the `payloads` folder copy the file starting with `hekate_ctcaer` to the `bin` folder and rename it to `payload.bin`.

---

### Next step

The next step depends on the platform you want to boot CFW from.

- If you plan on booting CFW from a Windows system, go [here]({{ site.url }}/os-specific-preparations/windows.html){: .a-table}
- If you plan on booting CFW from a macOS or Linux system, go [here]({{ site.url }}/os-specific-preparations/linux.html){: .a-table}
- If you plan on booting CFW from an Android or chromeOS device, go [here]({{ site.url }}/os-specific-preparations/android.html){: .a-table}