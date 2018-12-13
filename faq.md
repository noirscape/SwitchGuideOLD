---
layout: default
title: FAQ
---

Below you will find a list of commonly asked questions and answers.

## Table of Contents

- [RCM related](#rcm){: .a-table}
  - [My Switch shows no screen when turning on/"help I'm bricked"](#not-bricked){: .a-table}
  - [When I connect my Switch to my computer, there is no APX device listed in Zadig!](#not-zadig){: .a-table}
- [Ban related](#ban){: .a-table}
  - [How do I prevent getting banned? What are some of the common causes for bans?](#prevent-ban){: .a-table}
  - [How does Nintendo ban my system?](#how-ban){: .a-table}
  - [I want to prevent my Switch from connecting to Nintendo's servers!](#no-nintendo-network)
- [Homebrew related](#homebrew){: .a-table}
  - [My switch won't boot after I select Atmosphère in hekate!](#sys-ftpd)
  - [Does this guide work on system version x?](#can-i-run-on){: .a-table}
  - [What is the recommended microSD card size for Homebrew?](#recommended-size){: .a-table}
  - [What filesystem should I use on my microSD card?](#filesystem)
  - [Why is only Atmosphère and Hekate supported?](#why-atmosphere-hekate){: .a-table}
  - [I used SX OS/ReiNX and I want to use this setup instead. Do I need to do anything specific?](#reinx-sxos-earlier)
  - [My homebrew applications are not showing up!](#archive-bit)

## RCM related
{: #rcm}

**Q: My Switch shows no screen when turning on/"help I'm bricked"**{: #not-bricked}

A: You are not bricked. What this means is that your Switch has booted into RCM mode. Connect your Switch to a computer and follow the guide to start Hekate.

**Q: When I connect my Switch to my computer, there is no APX device listed in Zadig!**{: #not-zadig}

A: Make sure your Switch is in RCM before you connect it to your computer. If you see a device called "Nintendo Switch" in Zadig's list, you didn't connect your Switch in RCM. Close Zadig, unplug your Switch, put it in RCM, reconnect your switch and reopen Zadig.

---

## Ban related
{: #ban}

**Q: How do I prevent getting banned? What are some of the common causes for bans?**{: #prevent-ban}

A: Nintendo has been rather strict when it comes to banning homebrew systems. If you want to be safe, don't do any of the following:

- Install pirated content/gamecart dumps.
- Cheat or edit saves in games with online functionality
- Modify your NAND
- Using your Switch's client cert to connect to the CDN in an unauthorized manner.
- Using untested Homebrew on a system without a reimplemented creport KIP. (Note: Atmosphère patches creport by default.)

Note that the current setup given in the guide prevents you from doing the first bullet,as the given Atmosphère setup at the moment does not supply sigpatches, which are needed to install this type of content. Finally, Atmosphère will in the future release "Thermosphere". Thermosphere is Atmosphères implementation of emuNAND. This will result into being able to create an offline version of your NAND which you can use to safely test homebrew.

**Q: How does Nintendo ban my system?**{: #how-ban}

A: Depends on the context. By far the majority of bans are due to the Switch's error reporting and general telemetry (telemetry is the collection of data). If any of the collected data looks out of place to Nintendo, they can ban your system.

Users in European regions should go [here](https://accounts.nintendo.com/setting){: .a-table target="_blank"}, click on the "Edit" button next to usage information and untick both options and click "Save changes". While this will not fully disable telemetry, it will disable the majority of it.

**Q: I want to prevent my Switch from connecting to Nintendo's servers!**{: #no-nintendo-network}

A: A program called 90DNS can be used to accomplish this. 90DNS blocks all Nintendo domains, except for the connection test domain, meaning that while your Switch will think it's online, it won't actually connect to Nintendo's servers. See below on how to set this up.

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

---

## Homebrew related
{: #homebrew}

**Q: My switch won't boot after I select Atmosphère in hekate!**{: #sys-ftpd}

A: Make sure you _don't_ have `sys-ftpd.kip` in the `kips` directory. `sys-ftpd` does not work on firmware versions on or below 3.0.0.

**Q: Does this guide work on 6.2**{: #can-i-run-on}

A: This guide fully works on system version 6.2 and any version below.

**Q: What is the recommend microSD card size for homebrew?**{: #recommended-size}

A: The recommended size is 128GB. This will permit you to both have an emuNAND and allows you to make a full NAND dump without issue, while also leaving enough storage space for games and homebrew.

**Q: What filesystem should I use on my microSD card?**{: #filesystem}

A: It is highly advised to use FAT32. exFAT should only be used in case you want to restore a NAND dump. For detailed pro's and cons of each filesystem, see below.

FAT32

- Pro: Stable. Works with all homebrew.
- Pro: Only filesystem switch-linux based projects support (such as Lakka.)
- Con: Does not support files larger than 4GB.
- Con: Needs external tools to format on 32GB+ devices on Windows.
- Con: Cannot restore NAND dumps as a NAND dump is larger than 4GB.

exFAT

- Pro: Supports files larger than 4GB.
- Pro: Needed to restore NAND dumps, only filesystem that can hold a complete NAND dump that does not need to be combined later.
- Con: Highly unstable support. Very prone to corruption.
- Con: Wonky homebrew support.
- Con: Not supported at all by switch-linux.
- Con: Needs an update installed by Nintendo before it can be used.

**Q: Why is only Atmosphère and Hekate supported? What about SX OS and ReiNX?**{: #why-atmosphere-hekate}

A: SX OS is unsupported as it's primary usecase is piracy, as well as stealing code from Atmosphère. In addition, SX OS has homebrew compatability issues with Atmosphère and Hekate which wont be supported.

ReiNX on the other hand does not reimplement creport, which results in an increased chance of bans and makes development more difficult, as error reports are not dumped to the SD card, as well as making use of Atmosphère's sysmodules with a rename on the folders. This goes in combination with the fact that the way ReiNX modifies the system version to include ReiNXs version is done incorrectly, which results in bans as the way ReiNX does it means that the system version gets included in telemetry reports.

**Q: I used SX OS/ReiNX and I want to use this setup instead. Do I need to do anything specific?**{: #reinx-sxos-earlier}

A: If you've made a NAND backup before installing homebrew, restore it. This will remove the SX OS sysNAND "emuNAND". In addition, it will restore crash logs to their pristine state. If you have not done this, this should not matter, but it is advised you keep your Nintendo Switch offline to prevent it from being banned.

To clean up ReiNX and SX OS from the SD card, it is advised to remove all folders except for the following:

- `switch` This folder contains the homebrew applications you have installed.
- `Nintendo` This folder contains all games that have been installed on your SD card.

In addition, if you used unsigned NSPs (these include, but are not limited to 'backups'), you should uninstall these before following this guide.

The same should go for users of the "SDFiles"/"Kosmos" or similar setups.

Note: You will lose your SX OS SD card emuNAND.

**Q: My homebrew applications are not showing up!**{: #archive-bit}

A: First, these instructions only count if you can launch the Homebrew Launcher, but no applications show up. If you cannot launch the Homebrew Launcher, you have a different issue.

Try unsetting the archive bit in Hekate.

1. Launch Hekate using the instructions at [Launching CFW](/launching-cfw/) but stop at the point where it instructs you to launch Atmosphere.
2. Go to `Tools` -> `Unset archive bit (entire SD card)` using the power buttons.
3. Wait for Hekate to finish, then press power.
4. Go `Back` and go to `Launch` -> `Atmosphere` to boot Atmosphere.

This problem occurs if you copy files to your SD card if you are on macOS. macOS enables the archive bit on these files by default, which the Switch cannot read properly.

---

Please make any FAQ suggestions on the Issue Tracker.
