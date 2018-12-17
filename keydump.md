---
layout: default
title: Dumping your console keys.
---

BIS keys are console-specific. Using another consoles BIS keys may result in a bricked system. Always use your own BIS keys.
{: .info-box}

Sharing your keys is considered piracy.
{: .info-box}

In this step we will dump your keys. You need these keys to decrypt NCAs and your NAND. Being able to decrypt your NAND is essential in case you ever need to downgrade your Nintendo Switch to a lower version.

## What you will need

- The latest version of [Lockpick](https://github.com/shchmue/Lockpick/releases).

## Dumping your TSEC and fuses

1. Power off your Switch.
2. Follow the instructions at [Launching CFW](/launching-cfw/) for your system, but stop at the point where it tells you to launch Atmosphere.
3. Use the volume and power buttons to select `Console info...`.
4. Use the volume and power buttons to select `Print fuse info`. (Note: **fuse** info, not **kfuse** info!)
5. Press the power button twice.
6. Use the volume and power buttons to select `Print TSEC keys`.
7. Press the power button twice.
8. Select `Back`.
9. Select `Reboot (RCM)`. This will make your Switch power on in RCM mode automatically on the next boot.
10. Follow the instructions at [Launching CFW](/launching-cfw/) for your system.

## Installing Lockpick

1. Turn off your Switch and put your SD card in your computer.
2. Open the `switch` folder on your SD card.
3. Copy `lockpick.nro`from the `lockpick` release to the `switch` folder.
4. Put your SD card back in your Switch.
5. Follow the instructions at [Launching CFW](/launching-cfw/) for your system.

## Dumping keys

1. Open the Homebrew Launcher.
2. Open `Lockpick` through the Homebrew Launcher.
3. Press `+`.
4. In the `switch` folder should now be a file called `prod.keys`. Put this file in a safe location as it contains your device keys.

You should read the [Final Notes]({{ '/finalizing.html' | relative_url }}){: .a-table}.
{: .info-box}