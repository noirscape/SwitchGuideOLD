---
layout: default
title: OS-Specific preparations (macOS/Linux)
---

You will only have to do these steps once for each device you want to launch CFW from.
{: .info-box}

### What you will need

- The following files (use Ctrl-S or Apple key-S to save these):
  - [fusee-launcher.py](https://github.com/Cease-and-DeSwitch/fusee-launcher/raw/master/fusee-launcher.py){: target="_blank" .a-table}
  - Linux: [boot_Linux.sh.zip](https://noirscape.github.io/SwitchGuide/assets/boot_Linux.sh.zip){: target="_blank" .a-table}
  - macOS: [boot_macOS.command.zip](https://noirscape.github.io/SwitchGuide/assets/boot_macOS.command.zip){: target="_blank" .a-table}
- [intermezzo.bin](https://github.com/Cease-and-DeSwitch/fusee-launcher/raw/master/intermezzo.bin){: .a-table}
- Python 3. This will be installed during the next steps, so no need to download anything.
- `pyusb`. This will be installed during the next steps, so no need to download anything.

### Installing python3

#### macOS users

1. Open a terminal window
2. Enter the following command: `/usr/bin/ruby -e "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/master/install)"`
3. Enter your password when prompted.
4. Enter the following command: `brew install python`.
5. Enter the following command: `brew install libusb`.

#### Linux users

If you are on Linux, install Python 3 using your package manager. On Ubuntu systems it can be installed by doing `sudo apt install python3` and then providing your password and pressing Y. On other distro's, it's best to take a look what package offers Python 3.

### Installing pyusb

1. Open a terminal window
2. Run the following command. `python3 -m pip install --user pyusb`

### Making your bootkit

1. Make a new folder called `bootkit`.
  - Linux: Extract `boot_Linux.zip`, and place `boot_Linux.sh` in the `bootkit` folder.
  - Mac: Extract `boot_macOS.command.zip`, and place `boot_macOS.command` in the `bootkit` folder.
2. In the `bootkit` folder, make a folder called `bin`.
3. In the `bin` folder, place `fusee-launcher.py` and `intermezzo.bin`.
4. From the Hekate zip, copy the file starting with `hekate_ctcaer` to the `bin` folder and rename it to `payload.bin`.

[Continue to NAND dumping (macOS/Linux)]({{ '/nand-dump/linux.html' | relative_url }}){: .a-table}
{: .info-box}
