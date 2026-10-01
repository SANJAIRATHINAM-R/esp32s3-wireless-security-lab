# 03 — Firmware Setup

## Overview

The firmware provides the software layer that allows the ESP32-S3 hardware to perform the supported functions.

## General workflow

1. Connect the ESP32-S3.
2. Open the compatible web flasher.
3. Select the **ESP32-S3** target.
4. Enter bootloader mode if required.
5. Select the compatible firmware build.
6. Erase existing flash when performing a clean installation.
7. Start the flash operation.
8. Wait for verification/completion.
9. Reboot the board.
10. Confirm that the firmware starts normally.

![Firmware flasher](../images/02-firmware-flasher.png)

![Board selection](../images/03-board-selection.png)

![Flashing](../images/04-flash-process.png)

> **Important:** Use firmware intended for the exact board/target. Flashing an incompatible build can prevent the board from booting correctly.

## Bootloader note

If automatic detection does not work, many ESP32-S3 development boards can be placed into download mode using their BOOT/RESET controls. The exact button sequence depends on the board design.
