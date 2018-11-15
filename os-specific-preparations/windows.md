---
layout: default
title: OS-Specific preparations (Windows)
---

You will only have to do these steps once for each device you want to launch CFW from.
{: .info-box}

### What you will need

- [TegraRCMSmash](https://files.sshnuke.net/TegraRcmSmash1213.zip){: .a-table}
- [intermezzo.bin](https://github.com/Cease-and-DeSwitch/fusee-launcher/raw/master/intermezzo.bin){: .a-table}
- [Zadig](http://zadig.akeo.ie/downloads/zadig.exe){: .a-table target="_blank"}
- The latest release of [Hekate](https://github.com/ctcaer/hekate/releases/latest){: .a-table target="_blank"}
- The following files (use Ctrl-S or Apple key-S to save these) Make sure these files end in `.bat` ! Some browsers might add `.txt` to the end of this filename. If your browser does this, remove the `.txt` extension! On Windows you might need to disable hiding extensions from files. To do so, [see this wikihow](https://www.wikihow.tech/Show-File-Extensions-on-Windows){: .a-table} .:
  - [boot_cfw_win32.bat](https://noirscape.github.io/SwitchGuide/assets/boot_cfw_win32.bat){: target="_blank" .a-table}
  - [boot_cfw_win64.bat](https://noirscape.github.io/SwitchGuide/assets/boot_cfw_win64.bat){: target="_blank" .a-table}

### Install Zadig

1. Boot your Switch into RCM and connect it to your PC, see [this guide](https://xghostboyx.github.io/RCM-Guide){: target="_blank" .a-table} for more information on RCM.
2. Open Zadig as Administrator (right click and choose "Run as Administrator...").
3. From the device list, choose `APX` (if it's not showing up in the list, go to Options menu and check List All Devices).
4. For the driver type, use the arrows to navigate until you see `libusbK (v3.0.7.0)`.
5. Click the big `Install Driver` button. Device Manager should now list `APX` under the `libusbK USB Devices` tree item.


### Making your bootkit

When Hekate updates, download the Hekate zip again and do step 6 again.
{: .info-box}

1. Make a new folder called `bootkit`.
2. In the `bootkit` folder, place `boot_cfw_win32.bat`, `boot_cfw_win64.bat`.
3. In the `bootkit` folder, make a folder called `bin`.
4. From the TegraRCMSmash zip, copy the following files to the `bin` folder:
  - From the `Win32` folder, copy TegraRCMSmash.exe and rename it to `TegraRcmSmash_Win32`.
  - From the `x64` folder, copy TegraRCMSmash.exe and rename it to `TegraRcmSmash_Win64`.
5. Place `intermezzo.bin` in the `bin` folder.
6. From the Hekate zip, copy the file starting with `hekate_ctcaer` to the `bin` folder and rename it to `payload.bin`.

[Continue to NAND dumping (Windows)]({{ '/nand-dump/windows.html' | relative_url }}){: .a-table}
{: .info-box}