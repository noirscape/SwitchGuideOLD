---
layout: default
title: OS-Specific Preparations (iOS)
---

If this is your first time setting up CFW, please use a different device to set up your SD card and dump your NAND.
{: .info-box}

To set up iOS for launching CFW, you need to have a jailbroken device. Jailbreaking your iOS device is beyond the scope of this guide.
{: .info-box}

## What you will need

- A jailbroken iPhone with a lightning port.
- A USB-C to A cable.
- A Lightning OTG adapter.
- A computer (to upload the Hekate payload to iCloud).

## Installing NXBoot

1. Open `Cydia`.
2. Tap on the `Sources` tab.
3. Press the `Edit` button, then tap `Add`.
4. Enter the following URL in the resulting box: `https://mologie.github.io/repo/`.
5. Press `Add Source`.
6. Under individual sources, there should now be a new entry called `Mologie`.
7. Tap this entry.
8. Tap on `All Packages`.
9. Tap on `NXBoot`.
10. Press `Install`.
11. Press `Continue`.
12. Cydia will now install NXBoot.
13. Press the black button on the bottom after it says that NXBoot was succesfully installed.

If any errors show up please visit the r/jailbreak [Discord](https://discordapp.com/invite/jb){: target="_blank" .a-table}.
{: .info-box}

## Uploading the Hekate payload to iCloud

1. Download the latest release of Hekate [here](https://github.com/CTCaer/hekate/releases/latest) to your computer. Download the file starting with `hekate_ctcaer`.
2. Extract the file starting with `hekate_ctcaer` from this file.
3. Go to [iCloud](https://icloud.com).
4. Click on `iCloud Drive`.
5. Click the second icon in the top row (it looks like a cloud with an arrow going inside the cloud.)
6. Upload the file starting with `hekate_ctcaer`.
7. Wait for the upload to finish.

## Setting up NXBoot

1. Open NXBoot from your Home Menu.
2. Tap on `Select Bootcode`.
3. Tap `New Profile`.
4. Select the Hekate payload you uploaded in the previous step.

[Continue to Launching CFW (iOS)]({{ '/launching-cfw/ios.html' | relative_url }})
{: .info-box}
