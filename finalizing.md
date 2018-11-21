---
layout: default
title: Final notes
---

### Updating Atmosphère and Hekate

To keep track of new releases of Atmosphère and Hekate, I recommend subscribing to [/r/switchhacks](https://reddit.com/r/switchhacks).

#### Installing pyNX

1. Open the Homebrew Launcher.
2. Open `hb App Store` through the Homebrew Launcher.
3. Look for the program called `Pynx` and use the arrow buttons to select it.
4. Press `A` to view the detail menu.
5. Press `A` to download Pynx.

#### Download the latest version of SwitchGuide-Updater

1. Press `B` to go back to the main menu for `hb App Store`.
2. Look for the program called `SwitchGuide-Updater` and use the arrow buttons to select it.
3. Press `A` to view the detail menu.
4. Press `A` to download SwitchGuide-Updater.
5. Press the home button to exit `hb App Store`.

#### Updating Atmosphère or Hekate

1. Open the Homebrew Launcher.
2. Open `PyNX` through the Homebrew Launcher.
3. Press the green button with the text `switchguideupdater.py` on it using the touch screen.
4. Press `Update Atmosphère` or `Update Hekate` to update Atmosphère or Hekate respectively.
5. To use the updated version of Atmosphère, reboot your Switch. You'll need to boot CFW again using the instructions at [Launching CFW](/launching-cfw/) for your system.

<!-- #### Updating Atmosphère

1. [Download the latest release of Atmosphère](https://github.com/Atmosphère-NX/Atmosphère/releases/latest). Download both the zip file and `fusee-primary.bin`.
2. Turn off your Switch and put your microSD card in your computer.
3. Delete `fusee-primary.bin` and `fusee-secondary.bin` from the root your SD card.
4. Copy `fusee-secondary.bin` from the Atmosphère zip to the root of your SD card.
5. Copy `fusee-primary.bin` to the to the root of your SD card.
6. Safely remove your microSD card and plug it back in your Switch.
7. Boot CFW again using the instructions at [Launching CFW](/launching-cfw/) for your system.

### Updating Hekate

1. [Download the latest release of Hekate](https://github.com/CTCaer/hekate/releases/latest).
2. Turn off your Switch and put your microSD card in your computer.
3. Open the `bootloader` folder on your SD card and if it exists, remove `update.bin`.
4. From the Hekate zip, copy the file starting with `hekate_ctcaer` to the `bootloader` folder on your SD card.
5. Open the `bootloader` folder on your SD card and rename the file starting with `hekate_ctcaer` to `update.bin`. 
6. Safely remove your microSD card and plug it back in your Switch.
7. Boot CFW again using the instructions at [Launching CFW](/launching-cfw/) for your system. -->


### What next?

- You have now succesfully installed CFW on your Nintendo Switch.
- You can manage save data using Checkpoint (by Flagbrew), a save manager.
- You can download new homebrew using hb App Store (also known as Appstore-NX, by vgmoose).
- You can transfer files to your Switch over FTP using sys-ftpd (by jakibaki) if you are running a firmware above 3.0.0. No authentication is needed and the FTP server runs on port 5000. If you don't want this, remove the `sys-ftpd.kip` file from the `kips` folder in the `Atmosphère` folder.
- You can load any KIP file you want by placing them in the `kips` folder in your `Atmosphère` folder. These KIPs will be loaded automatically when booting Atmosphère. **Loading KIPs from unknown sources may damage your system. Be careful with what KIPs you load.**
- When rebooting, your access to CFW will be lost, unless you follow the steps at Launching CFW again.
- If you need to launch Stock firmware, select the `Stock` option when in Hekate's `Launch...` menu. You should not need to do this under normal circumstances, but it may be useful for troubleshooting.
  - **If you use the homebrew ChoiDuJourNX to update your Switch's firmware to prevent burning these fuses, this option will burn fuses!**

It is highly advised to also read the [FAQ](faq.html){: .a-table target="_blank")}
{: .info-box}
