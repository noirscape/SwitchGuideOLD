---
layout: default
title: OS-Specific preparations (Windows)
---

You will only have to do these steps once for each device you want to launch CFW from.
{: .info-box}

### Install Zadig

1. Boot your Switch into RCM and connect it to your PC, see [this guide](https://xghostboyx.github.io/RCM-Guide){: target="_blank" .a-table} for more information on RCM.
2. Download the latest version of [Zadig](http://zadig.akeo.ie/downloads/zadig.exe){: .a-table target="_blank"} and run it with the appropriate permissions.
3. From the device list, choose `APX` (if it's not showing up in the list, go to Options menu and check List All Devices).
4. For the driver type, use the arrows to navigate until you see `libusbK (v3.0.7.0)`.
5. Click the big `Install Driver` button. Device Manager should now list `APX` under the `libusbK USB Devices` tree item.

[Continue to Launching CFW (Windows)]({{ '/launching-cfw/windows.html' | relative_url }}){: .a-table}
{: .info-box}