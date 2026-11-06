# Rig LEDs

*A meter bridge for your rig.*

[![Latest release](https://img.shields.io/github/v/release/wuerks/RigLEDs)](../../releases/latest)
[![Downloads](https://img.shields.io/github/downloads/wuerks/RigLEDs/total)](../../releases)
[![Support on Ko-fi](https://img.shields.io/badge/Support-Ko--fi-FF5E5B?logo=ko-fi&logoColor=white)](https://ko-fi.com/devWuerks)

Rig LEDs shows what your computer is doing as columns of glowing LEDs. Processor and every core,
graphics, memory, fans, temperatures, disks, network and sound, all at a glance. It raises an
alarm when something runs too hot or too busy for too long, and names the program causing it.

## Support this project

Rig LEDs is free, with no ads and no tracking. If you like it, you can buy me a coffee on Ko-fi.
You can pay by card or PayPal, and you do not need an account. It helps me keep improving Rig LEDs
and build the next app.

Thank you. ☕ &nbsp; <a href="https://ko-fi.com/devWuerks"><img src="donate.svg" alt="Donate" height="36" align="middle"></a>

## Prerequisites

### Software

1. **Windows 10 or Windows 11, 64-bit**, on a desktop or laptop.
2. **Administrator rights to install.** The setup adds a small sensor service that runs in the
   background. If your PC does not have it yet, it also adds PawnIO, a Microsoft-signed driver
   that reads the CPU temperature and the motherboard fans. Both need administrator approval, so
   Windows asks once during setup. If your account is not an administrator, enter administrator
   details when asked, or ask whoever manages the PC to run the setup.
3. Nothing else. Everything else is read through Windows.

### Hardware

Rig LEDs runs on any PC. It shows only what your PC reports and leaves the rest out. The
**System** tab in Settings lists what is missing and why. What each reading needs:

| Reading | Works on |
|---|---|
| CPU use, **every CPU core**, memory, disk activity, network, sound | Any PC, Intel or AMD |
| CPU temperature | Intel Core, and AMD Ryzen (Zen) |
| Motherboard fan speeds | Most desktop motherboards. Many laptops do not report their fans. |
| Graphics card use, temperature and fan | NVIDIA, AMD or Intel, read through Windows |
| NPU (AI accelerator) use | Shown when Windows lists one, such as Intel AI Boost |

## Download

Open the latest **[Release](../../releases/latest)** and download `rig-leds-setup-<version>.exe`.

## Install

You need **administrator rights** to install. See Prerequisites above.

1. Run **`rig-leds-setup-<version>.exe`**.
2. Agree to the licence and press **Install**.
3. **Approve the administrator prompt.** Choose **Yes**, or enter administrator details if your
   account is not an administrator. Only the sensor service and the driver need this.

Rig LEDs installs to Program Files, adds a Start menu entry and starts. To update later, run a
newer setup the same way. To remove it, open Windows **Settings > Apps**, find Rig LEDs and choose
**Uninstall**.

## Verify your download

**Download:** `rig-leds-setup-1.1.3.exe`

**SHA-256 Checksum:**

`8768E212259FB333174907B0CF1B1ADE2E061099D9CCD607C6780B307601031A`

## Privacy

Rig LEDs runs only on your own computer. It collects **no** personal data, usage statistics or
telemetry. The readings it shows never leave your PC.

1. It goes online **only** to check for a newer version. It asks GitHub for the number of the
   latest release here. **Nothing about you or your computer is sent.** You can turn the check
   off in Rig LEDs Settings, on the **Help** tab under Updates.
2. If you **report an issue**, only what you paste is shared. The **Diagnostics** text lists your
   hardware and what could or could not be read. It helps with support, but read it before you
   post it.

## Licence

Rig LEDs is closed-source freeware. It is licensed, not sold, under the agreement in
`LICENSE.txt`, which comes with the download. You may install and use it for free. You may not
reverse-engineer, modify or resell it. It is provided "as is", with no warranty. It includes the
signed PawnIO driver (GPLv2 with exception) and the Inter typeface (SIL OFL 1.1) under their own
licences.

## Support

Found a problem or have an idea? Open a **[new issue](../../issues/new/choose)** and choose
**Bug report** or **Feature request**. If a reading is missing, open **Settings > System** in
Rig LEDs, press **Copy** under **Diagnostics**, and paste the text into the bug report. It shows
what was found and why.
