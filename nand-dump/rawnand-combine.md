---
layout: default
title: NAND dumping (combining partial dumps)
---

If you have a single rawnand.bin file when dumping your NAND, you do not need to follow this section. Instead, continue to [Launching CFW]({{ '/launching-cfw/' | relative_url }}).
{: .info-box}

### Combining rawnand.bin files

Note that you *cannot* restore partial NAND backups. If you need to restore a NAND backup, you will need to have an SD card that is at least 30GB in size and it must be formatted as exFAT.
{: .info-box}

1. Go to the latest release of [hekate](https://github.com/CTCaer/hekate/releases/latest){: .a-table} and download the `joiner_scripts_for_windows_linux_macos.zip` file and extract it.
2. Add `.sh` to the end of the filenames of `join_15_2GBparts_linux_macosx` and `join_30_1GBparts_linux_macosx`.
3. Count how many partial dumps you have (you should have either 15 or 30 files, if you have a different amount, you are missing partial dumps) and move all the partial dumps to the folder you extracted the zip to.
4. Open the appropriate script for your system and your amount of dumps:
  - If you had 15 files and are on Windows, open the `join_15_2GBparts_windows.bat` file.
  - If you had 15 files and are on macOS/Linux, open the `join_15_2GBparts_linux_macosx.sh` script. (Note: Linux users may need to run this file from a terminal instead and mark it as executable.)
  - If you had 30 files and are on Windows, open the `join_30_1GBparts_windows.bat` file.
  - If you had 30 files and are on macOS/Linux, open the `join_30_1GBparts_linux_macosx.sh` script. (Note: Linux users may need to run this file from a terminal instead and mark it as executable.)
5. Once the script finishes running, you should have a file called `rawnand.bin` in the same folder. This file is your NAND backup. Store it somewhere safe.

Now that you have made a NAND dump, you can properly launch Atmosphere by following the instructions [here]({{ '/launching-cfw/' | relative_url }}).
{: .info-box}