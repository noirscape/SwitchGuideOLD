---
layout: default
title: Setting up your SD card
---

### What you will need

- The latest release of [Atmosphère](https://github.com/Atmosphere-NX/Atmosphere/releases/latest). For this step, you will need the zip file and `fusee-primary.bin`.
- The latest release of [Hekate](https://github.com/ctcaer/hekate/releases/latest){: .a-table target="_blank"}
- The latest release of the [homebrew launcher](https://github.com/switchbrew/nx-hbmenu/releases/latest){: .a-table target="_blank"}.
- The latest release of [Checkpoint](https://github.com/FlagBrew/Checkpoint/releases/latest){: .a-table target="_blank"}. Download the `.nro` file.
- The latest release of [hb-appstore](https://github.com/vgmoose/hb-appstore/releases/latest){: .a-table target="_blank"}.
- [sys-ftpd.kip](https://noirscape.github.io/SwitchGuide/assets/sys-ftpd.kip){: .a-table} ([source](https://github.com/jakibaki/sys-ftpd){: .a-table target="_blank"})
- [hekate_ipl.ini](https://noirscape.github.io/SwitchGuide/assets/hekate_ipl.ini) (use Ctrl-S or Apple key-S to save this file.) Make sure this file ends in `.ini` ! Some browsers might add `.txt` to the end of this filename. If your browser does this, remove the `.txt` extension! On Windows and macOS you might need to disable hiding extensions from files. To do so, [see this wikihow](https://www.wikihow.tech/Show-File-Extensions-on-Windows). On macOS, see [this iDownloadBlog page](https://www.idownloadblog.com/2014/10/29/how-to-show-or-hide-filename-extensions-in-os-x-yosemite/).
- The latest release of [nx-hbloader](https://github.com/switchbrew/nx-hbloader/releases/latest){: .a-table}

<!-- Below section to be uncommented whenever shit breaks on a FW update. -->
<!-- ### Blocking updates

1. Open the settings applet on your Switch.
2. Go to `Internet` -> `Internet Settings`.
3. You will see a list of all WiFi networks nearby and those you've ever been connected to.
4. For each network you've been connected to, select it and choose `Change settings`
5. Change `DNS` to `Manual`.
6. Set the primary DNS server to `163.172.141.219`.
7. Set the secondary DNS `45.248.48.62`.
8. Press the save button and then `B` to return to the network list.
9. Repeat steps 4 to 8 for all WiFi networks you've been connected to.
10. Press the Home button to get back to the main menu.

### Removing update data.

This is to remove a downloaded system update to prevent the update from nagging you whenever you start a game.

1. Power off your Switch.
2. Press Volume up + Volume down + Power at the same time until you see the Nintendo Switch logo appear.
3. Your Switch will boot into Maintenance mode.
4. Press the power button again to turn off your Switch. -->

### Setting up your sd card

1. Turn off your Switch and put your microSD card in your computer.
2. Copy the `bootloader` folder from the Hekate zip to your SD card.
3. Copy the `atmosphere` folder from the Atmosphère zip to your SD card.
4. Copy `fusee-primary.bin` to the to the `atmosphere` folder.
5. Copy `hbmenu.nro`from the `nx-hbmenu` release  to the root of your SD card.
6. Make a folder called `switch` on the root of your SD card.
7. Copy `checkpoint.nro` from the `Checkpoint` release to the `switch` folder.
8. Extract the `hb-appstore` zip and copy `appstore.nro` to the `switch` folder.
9. Copy `hbl.nsp` from the `nx-hbloader` release to the `atmosphere` folder.
10. In the `atmosphere` folder, make a folder called `kips`.
11. If you are above firmware 3.0.0, copy `sys-ftpd.kip` to the `kips` folder. Otherwise, skip this step.
12. Copy `hekate_ipl.ini` to the `bootloader` folder on your SD card.
13. Safely remove your microSD card and plug it back in your Switch.

---

### Next step

The next step depends on the platform you want to boot CFW from.

- If you plan on booting CFW from a Windows system, go [here](os-specific-preparations/windows.html){: .a-table}
- If you plan on booting CFW from a macOS or Linux system, go [here](os-specific-preparations/linux.html){: .a-table}
- If you plan on booting CFW from an Android or chromeOS device, go [here](os-specific-preparations/android.html){: .a-table}
