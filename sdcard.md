---
layout: default
title: Setting up your SD card and bootkit
---

### What you will need

- The latest release of [Atmosphére](https://github.com/Atmosphere-NX/Atmosphere/releases/latest){: .a-table target="_blank"}. For this step, you will need the zip file and `fusee-primary.bin`.
- The latest release of [Hekate](https://github.com/ctcaer/hekate/releases/latest){: .a-table target="_blank"}
- The latest release of the [homebrew launcher](https://github.com/switchbrew/nx-hbmenu/releases/latest){: .a-table target="_blank"}.
- The latest release of [Checkpoint](https://github.com/FlagBrew/Checkpoint/releases/latest){: .a-table target="_blank"}. Download the `.nro` file.
- The latest release of [hb-appstore](https://github.com/vgmoose/hb-appstore/releases/latest){: .a-table target="_blank"}.
- [sys-ftpd.kip](https://noirscape.github.io/SwitchGuide/assets/sys-ftpd.kip){: .a-table} ([source](https://github.com/jakibaki/sys-ftpd){: .a-table target="_blank"})
- [hekate_ipl.ini](https://noirscape.github.io/SwitchGuide/assets/hekate_ipl.ini){: .a-table}
- [hbl.nsp](https://noirscape.github.io/SwitchGuide/assets/hbl.nsp){: .a-table}

### Setting up your sd card

1. Turn off your Switch and put your microSD card in your computer.
2. Copy the `bootloader` folder from the Hekate zip to your SD card.
3. Copy the `atmosphere` folder from the Atmosphére zip to your SD card.
4. Copy `fusee-secondary.bin` from the Atmosphére zip to the root of your SD card.
5. Copy `fusee-primary.bin` to the to the root of your SD card.
6. Copy `hbmenu.nro` to the root of your SD card.
7. Make a folder called `switch` on the root of your SD card.
8. Copy `checkpoint.nro` to the `switch` folder.
9. Extract the `hb-appstore` zip and copy `appstore.nro` to the switch folder.
10. In the `atmosphere` folder on your SD card, place `hbl.nsp`.
11. In the `atmosphere` folder on your SD card, make a folder called `kips`.
12. In the `kips` folder, place `sys-ftpd.kip`.
13. In the `bootloader` folder on your SD card, place `hekate_ipl.ini`.
14. Safely remove your microSD card and plug it back in your Switch.

---

### Next step

The next step depends on the platform you want to boot CFW from.

- If you plan on booting CFW from a Windows system, go [here](os-specific-preparations/windows.html){: .a-table}
- If you plan on booting CFW from a macOS or Linux system, go [here](os-specific-preparations/linux.html){: .a-table}
- If you plan on booting CFW from an Android or chromeOS device, go [here](os-specific-preparations/android.html){: .a-table}