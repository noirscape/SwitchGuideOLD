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
4. Press `Update Atmosphere` or `Update Hekate` to update Atmosphère or Hekate respectively.
5. To use the updated version of Atmosphère, reboot your Switch. You'll need to boot CFW again using the instructions at [Launching CFW](/launching-cfw/) for your system.

### Changing the title the Homebrew Launcher uses

To do this, you need to have downloaded at least **1** game/application from the Nintendo eShop. If you have not done so, there are free games/applications available on the eShop. Which title you select does not matter, any will work.
{: .info-box}

In order to make use of some Homebrew, we need to give the Homebrew Launcher more memory. To do this, we need to run the Homebrew Launcher from an installed game on your Switch.

#### What you will need

- At least 1 installed game on your Switch.
- The title ID of this game (can be found [here](https://switchbrew.org/wiki/Title_list/Games)). Look up the title of your game. The Title ID is the text in the column to the left.

1. Turn off your Switch and put your SD card in your computer.
2. Open the `atmosphere` folder on your SD card.
3. Open the `loader.ini` file in Notepad (note: do **not** use Microsoft Word or Wordpad. Those are **not** suitable editors).
4. Remove the text after `hbl_tid=`
5. Put the Title ID of your game after `hbl_tid=`.
6. Save the file.
7. Put your SD card back in your Switch.
8. Follow the instructions at [Launching CFW](/launching-cfw/) for your system.

To launch the Homebrew menu from now on, you need to use this installed game. If you instead want to play the installed game, hold the `R` button while launching the game.

If you want to change the game used to launch the Homebrew Launcher, just follow these steps again.

### What next?

- You have now succesfully installed CFW on your Nintendo Switch.
- You can manage save data using Checkpoint (by Flagbrew), a save manager.
- You can download new homebrew using hb App Store (also known as Appstore-NX, by vgmoose).
- You can transfer files to your Switch over FTP using sys-ftpd (by jakibaki) if you are running a firmware above 3.0.0. No authentication is needed and the FTP server runs on port 5000. If you don't want this, remove the `sys-ftpd.kip` file from the `kips` folder in the `atmosphere` folder.
- You can load any KIP file you want by placing them in the `kips` folder in your `atmosphere` folder. These KIPs will be loaded automatically when booting Atmosphère. **Loading KIPs from unknown sources may damage your system. Be careful with what KIPs you load.**
- When rebooting, your access to CFW will be lost, unless you follow the steps at Launching CFW again.
- If you need to launch Stock firmware, select the `Stock` option when in Hekate's `Launch...` menu. You should not need to do this under normal circumstances, but it may be useful for troubleshooting.
  - **If you use the homebrew ChoiDuJourNX to update your Switch's firmware to prevent burning these fuses, this option will burn fuses!**

It is highly advised to also read the [FAQ](faq.html){: .a-table target="_blank")}
{: .info-box}
