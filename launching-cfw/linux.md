---
layout: default
title: Launching CFW (macOS/Linux)
---

You will have to do these steps each time you want to boot into CFW.
{: .info-box}

### Launch Hekate

1. Boot your Switch into RCM and connect it to your PC, see [this guide](https://xghostboyx.github.io/RCM-Guide){: target="_blank" .a-table} for more information on RCM.
2. Run the `boot_Linux.sh` or `boot_macOS.command` script included in the bootkit folder.

### Launch Atmosphère

1. Once Hekate loads, using the volume and power buttons, select `Launch - > Atmosphere`.
2. To verify that Atmosphère launched properly, go to the System Settings and then scroll down to "System". Behind the line `Current system version:`, you should see your Switch's firmware version and `(AMS x.y.z)`. `x.y.z` are numbers that indicate the version of Atmosphère you are currently running.
3. Once your Switch boots, you can open the album applet to load the Homebrew Launcher.

You should dump your [keys]({{ '/biskeydump.html' | relative_url }}) next.
{: .info-box}
