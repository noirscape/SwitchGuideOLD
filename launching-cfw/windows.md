---
layout: default
title: Launching CFW (Windows)
---

You will have to do these steps each time you want to boot into CFW.
{: .info-box}

### Launch Hekate

1. Boot your Switch into RCM and connect it to your PC, see [this guide](https://xghostboyx.github.io/RCM-Guide){: target="_blank" .a-table} for more information on RCM.
2. Depending on your processor architecture (32-bit or 64-bit), run the relevant `boot_cfw_Win*.bat` in the bootkit folder.
3. Once Hekate loads, using the volume and power buttons, select `Launch - > Atmosphere`.
4. To verify that Atmosphere launched properly, go to the System Settings and then scroll down to "System". Behind the line `Current system version:`, you should see your Switch's firmware version and `(AMS x.y.z)`. `x.y.z` are numbers that indicate the version of Atmosphere you are currently running.
5. Once your Switch boots, you can open the album applet to load the Homebrew Launcher.

You should read the [Final Notes]({{ '/finalizing.html' | relative_url }}){: .a-table} so you can dump your NAND.
{: .info-box}