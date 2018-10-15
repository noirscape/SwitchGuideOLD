---
layout: default
title: OS-Specific preparations (macOS/Linux)
---

You will only have to do these steps once for each device you want to launch CFW from.
{: .info-box}


### Installing python3

Open a terminal window, then enter the following commands if you are on macOS. Enter your password when prompted.

`/usr/bin/ruby -e "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/master/install)"`

`brew install python`

The first command installs `brew.sh`, a package manager for macOS systems. The second uses brew to install Python.

If you are on Linux, install Python 3 using your package manager. On Ubuntu systems it can be installed by doing `sudo apt install python3` and then providing your password and pressing Y. On other distro's, it's best to take a look what package offers Python 3.

### Installing pyusb

Open a terminal window and run the following command. Enter your password when prompted.

`sudo pip3 install pyusb`

[Continue to Launching CFW (macOS/Linux)]({{ site.url }}/launching-cfw/linux.html){: .a-table}
{: .info-box}