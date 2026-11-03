# Unofficial LineageOS for Redmi Note 9 5G and 9T (cannon/cannong)

Welcome! This project aims to bring a clean, stable, and secure stock Android experience, with a focus on reliability. If you're looking for the latest Android version, customizations, etc., this isn't it. The goal is to provide a bloat-free alternative to MIUI with stock-like behavior.

---

## Prerequisites

Before installing, make sure you have:

- A supported cannon/cannong device.
- An unlocked bootloader.
- Required firmware: V14.0.4.0.SJEMIXM.
- A computer with working ADB and Fastboot tools that correctly detect your device.
- A USB cable.
- At least 50% battery charge.

**Read the entire installation procedure before proceeding.**

Installing this ROM may erase your device or render it unusable. Back up your data, IMEI, etc., before continuing. Do so at your own risk.

---

## Installation

These instructions are for a **clean installation**. With your mobile device connected to the computer and the ROM ZIP downloaded:

1. Extract the `recovery.img` file inside the zip.
2. Enter Fastboot mode using `adb reboot bootloader` or by pressing the POWER + VOLUME DOWN buttons simultaneously.
3. Install the recovery with `fastboot flash recovery recovery.img`.
4. Boot into Lineage Recovery using `fastboot reboot recovery` or by pressing the POWER + VOLUME UP buttons simultaneously.
5. Format data by selecting the "Factory reset" option and then "Format data/factory reset".
6. Once formatting is complete, select "Apply update" from the Lineage Recovery home screen, then select "Apply from ADB".
7. On your computer, install the downloaded ZIP using `adb -d sideload` followed by the full name of the ZIP file (usually `lineage-XX.X-XXXXXXXX-UNOFFICIAL-cannon.zip`).
8. If you're installing a GApps package, don't reboot yet. Repeat steps 6 and 7, but this time use the filename of your GApps package. If you're not installing GApps, skip this step.
9. Once installation is complete, select "Reboot system now" from the recovery home screen and enjoy your device!

For an **update/dirty installation**, the process is the same, but without flashing recovery or formatting data. Simply repeat steps 4, 6, 7, and 9.

Step 8 may or may not be necessary, depending on your GApps package, but these days, they are reflashed automatically.

---

## Contribute

I do this work for free and share it with everyone so that others can benefit from it, too.

If you enjoy this project and would like to support me, your contributions will be appreciated.

☕ **[Support me on Ko-fi](https://ko-fi.com/jacksedart)**

---

## Support and bugs

Found a bug?

Please report it in the [Telegram community](https://t.me/LineageOS_cannon).

When reporting an issue, include:

- Device variant.
- ROM build.
- Steps to reproduce the issue.
- Screenshots or logs, where applicable.
- Whether the issue happens consistently.

Please search existing discussions before reporting an issue that has already been reported.

Do not report bugs caused by unsupported modifications, kernels, or packages. Only issues that can be reproduced and debugged on a standard configuration will be supported.

---

## Credits and acknowledgements

This project wouldn't be possible without the work of many developers and contributors.

Special thanks to:

- **[LineageOS](https://github.com/LineageOS)** — for the operating system and upstream development.
- **[LinkBoi00](https://github.com/LinkBoi00)** — for the original bring-up and the trees.

---

## Disclaimer

LineageOS is a trademark of its respective owners. This project is an independent, unofficial distribution and is not affiliated with, endorsed by, or supported by the official LineageOS project.

Android is a trademark of Google LLC.

All third-party trademarks belong to their respective owners.
