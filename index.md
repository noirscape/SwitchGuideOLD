---
layout: default
title: Switch Homebrew Guide
---

If you need assistance, visit us on [Discord](https://discord.gg/C29hYvh){: target="_blank" .a-table}.
{: .info-box}

This guide uses sdsetup. sdsetup is used because it has the most up-to-date files. That said, sdsetup also allows generating SX OS/ReiNX setups. These are not supported by this guide and not supported on the previously linked Discord.
{: .alert-box}

The Hekate bootmenu will reference a Discord server. This Discord server is not considered supported by this guide and not supported on the previously linked Discord. 
{: .alert-box}

### Terminology used in this guide

- **Hekate**: A bootloader for the Nintendo Switch.
- **Atmosphére**: The CFW made by the Atmosphere-NX org.
- **CFW**: A Custom Firmware. Custom Firmware permits access to homebrew on the Nintendo Switch.
- **RCM**: A special mode of the Nintendo Switch's Tegra X1 chip that thanks to a bug allows us to push any payload to it. This exploit is known as ShofEL2 or fusee-gelee.
- **bootkit**: A folder on your computer that you will use to launch CFW from RCM. It contains a few scripts, TegraRCMSmash, fusee-gelee and the Hekate payload. You will set one up during this guide. You will need access to this folder each time you want to launch CFW, so keep it in a safe spot where you can find it later.

### What are we doing to run homebrew on the Switch

This guide will boot you into Atmosphére using a combination of the RCM, the Hekate bootloader and Atmosphére CFW. In addition, this guide will enable an FTP server on your Switch to simplify transferring files while in Horizon. You will also be able to access the Homebrew menu by launching the album applet. This has only been tested from firmware 5.0.2 upwards, but theoretically should work on all firmware versions. Certain applications may not work on certain firmware versions so YMMV.

### What you will need

- A "first-generation" Switch. (All Switch consoles before July 2018 will work.)
- A way to put your Switch into RCM. See [this guide](https://xghostboyx.github.io/RCM-Guide){: target="_blank" .a-table} for more information. Users on 1.0.0 can also enter RCM from a software side by using a program called reboot_to_rcm. See [here](1-0-0.html){: target="_blank" .a-table} for more details.
- A host PC running Windows, Linux, macOS or ChromeOS, or an Android device.
- A USB Type-C to USB-A cable, or a USB Type-C to USB Type-C cable. (Depending on what your host PC supports.)
- If you are using an Android device, you need a way to connect the Switch to it, either a USB OTG cable, or USB-C to USB-C cable depending on what your device supports.
- A microSD card 2GB or larger, formatted to either FAT32, or exFAT (only if your switch has the exFAT support "update".)

### What are the advantages to running homebrew

Running homebrew will allow you to run tools such as [Checkpoint](https://github.com/BernardoGiordano/Checkpoint){: target="_blank" .a-table}, a save manager.
You also can run emulators like [RetroArch](https://www.retroarch.com/?page=platforms){: target="_blank" .a-table} to play retro games on the Switch.
In addition, you can run homebrew games such as [tetriswitch](https://gbatemp.net/threads/tetriswitch-a-tetris-clone-for-the-switch.498481){: target="_blank" .a-table} and [Pong](https://github.com/I-EAT-CHEEZE-YO/switch_sdl_pong){: target="_blank" .a-table}.

### Are there any risks to running homebrew

Yes. Nintendo has increased the Telemetry on the Nintendo Switch compared to previous consoles and does ban if they detect you using homebrew. You can find more details on this and a comprehensive list [in the FAQ](faq.html#ban){: target="_blank" .a-table}.

Go to [Setting up your SD card](sdcard.html){: .a-table} to get started.
{: .info-box}