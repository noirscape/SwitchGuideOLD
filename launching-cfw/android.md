---
layout: default
title: Launching CFW (Android/chromeOS)
---

{%include launch-cfw.md %}

### Launch Hekate

1. Boot your Switch into RCM and connect it to your device, see [this guide](https://noirscape.github.io/RCM-Guide){: target="_blank" .a-table} for more information on RCM.
2. Go to [this website](https://atlas44.s3-us-west-2.amazonaws.com/web-fusee-launcher/index.html){: .a-table target="_blank"}.
3. Under the Payload section, select upload payload and upload the .bin file you previously downloaded.
4. Click `do the thing`, select `APX` and click connect.

### Launch Atmosphère

1. Once Hekate loads, using the volume and power buttons, select `Launch - > Atmosphere`.
2. To verify that Atmosphère launched properly, go to the System Settings and then scroll down to "System". Behind the line `Current system version:`, you should see your Switch's firmware version and `(AMS x.y.z)`. `x.y.z` are numbers that indicate the version of Atmosphère you are currently running.
3. Once your Switch boots, you can open the album applet to load the Homebrew Launcher.

You should dump your [keys]({{ '/keydump.html' | relative_url }}) next.
{: .info-box}
