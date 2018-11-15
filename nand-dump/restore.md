---
layout: nosidebar
title: Restoring a NAND dump
---

#### About restoring NAND backups

When restoring NAND backups, you must use an exFAT filesystem! FAT32 filesystems will not work for restoring NAND backups due to size limitations on FAT32 filesystems (FAT32 cannot hold files larger than 4GB and the rawnand.bin is ~29GB). Hekate comes with it's _own_ exFAT driver. This means you do not need to install the exFAT "update" from Nintendo to restore your NAND.