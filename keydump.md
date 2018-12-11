---
layout: default
title: Dumping your BIS keys.
---

BIS keys are console-specific. It is not possible to use another consoles BIS keys. Do not share your BIS keys!
{: .info-box}

In this step we will dump your BIS keys. Your BIS keys are needed in case you update your NAND to a version not supported by CFW (at the time of writing all firmware versions are supported by CFW) and wish to downgrade it later or if you want to extract files from your NAND dumps.

## What you will need

- The latest version of [biskeydump](https://switchtools.sshnuke.net/).

## Dumping your BIS keys

1. Turn off your switch and put your SD card in your computer.
2. From the biskeydump zip, extract `biskeydump.bin`.
3. Copy `biskeydump.bin` to the `payloads` folder in the `bootloader` folder on your SD card.
4. Plug your SD card back in your Switch.
5. Launch Hekate using the steps at [Launching CFW](/launching-cfw/). Stop at the step where it tells you to launch Atmosphère.
6. Go to `Launch` -> `Payloads` -> `biskeydump.bin`.
7. Wait a few seconds and your BIS keys should appear on top of the screen, as well as a QR code.
8. Scan the QR code using your phone.
9. You now have your BIS keys on your phone's clipboard.
10. Store these BIS keys in a safe place.
11. Power off your Switch by holding the power button for ~10 seconds.
12. You can launch CFW again using the instructions under [Launching CFW](/launching-cfw/).

You should read the [Final Notes]({{ '/finalizing.html' | relative_url }}){: .a-table}.
{: .info-box}