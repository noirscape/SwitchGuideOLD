---
layout: default
title: Dumping your console keys.
---

BIS keys are console-specific. Using another consoles BIS keys may result in a bricked system. Always use your own BIS keys.
{: .info-box}

Sharing your keys is considered piracy.
{: .info-box}

In this step we will dump your keys. You need these keys to decrypt NCAs and your NAND. Being able to decrypt your NAND is essential in case you ever need to downgrade your Nintendo Switch to a lower version.

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

## Installing lockpick

1. Open the Homebrew Launcher.
2. Open `hb App Store` through the Homebrew Launcher.
3. Look for the program called `Lockpick` and use the arrow buttons to select it.
4. Press `A` to view the detail menu.
5. Press `A` to download Lockpick.
6. Press the home button.

## Dumping keys

1. Open the Homebrew Launcher.
2. Open `Lockpick` through the Homebrew Launcher.
3. Press `+`.
4. In the `switch` folder should now be a file called `prod.keys`. Put this file in a safe location as it contains your device keys.

You should read the [Final Notes]({{ '/finalizing.html' | relative_url }}){: .a-table}.
{: .info-box}