# Rig LEDs

*A meter bridge for your rig.*

[![Latest release](https://img.shields.io/github/v/release/wuerks/RigLEDs)](../../releases/latest)
[![Downloads](https://img.shields.io/github/downloads/wuerks/RigLEDs/total)](../../releases)
[![Support on Ko-fi](https://img.shields.io/badge/Support-Ko--fi-FF5E5B?logo=ko-fi&logoColor=white)](https://ko-fi.com/devWuerks)

Rig LEDs shows what your computer is doing as columns of glowing LEDs: processor and every core,
graphics, memory, fans, temperatures, disks, network and sound, live at a glance. It raises an
alarm when something runs too hot or too busy for too long, and names the program responsible.

## Support this project

Rig LEDs is free, with no ads and no tracking. If it has earned a place on your desktop, you can
buy me a coffee on Ko-fi — card or PayPal, no account needed. It genuinely helps me keep
improving it and build the next one.

Thank you. ☕ &nbsp; <a href="https://ko-fi.com/devWuerks"><img src="donate.svg" alt="Donate" height="36" align="middle"></a>

## Prerequisites

### Software

- **Windows 10 or Windows 11, 64-bit** — desktop or laptop.
- **Administrator rights to install.** The setup adds a small background sensor service and, if
  your PC does not already have it, a Microsoft-signed driver (PawnIO) to read the CPU temperature
  and motherboard fans — both need administrator approval. Windows asks for an administrator once
  during setup. **If your account is not an administrator**, provide administrator credentials when
  prompted, or ask whoever manages the PC to run the setup for you.
- Nothing else to install — everything else is read through Windows.

### Hardware

Rig LEDs runs on any PC and shows only what your machine actually reports, leaving the rest out —
the **System** tab says what is missing and why. What each reading needs:

| Reading | Works on |
|---|---|
| CPU use, **every CPU core**, memory, disk activity, network, sound | Any PC — Intel or AMD |
| CPU temperature | Intel Core, and AMD Ryzen (Zen) |
| Motherboard fan speeds | Most desktop motherboards (many laptops do not expose their fans) |
| Graphics card use, temperature and fan | NVIDIA, AMD or Intel, read through Windows |
| NPU (AI accelerator) use | Shown when Windows lists one (e.g. Intel AI Boost) |

## Download

Get the latest **[Release](../../releases/latest)** and download `rig-leds-setup-<version>.exe`.

## Install

You need **administrator rights** to install (see Prerequisites above).

1. Run **`rig-leds-setup-<version>.exe`**.
2. Agree to the licence and press **Install**.
3. **Approve the administrator prompt** — choose **Yes**, or enter administrator credentials if
   your account is not an administrator. This is required to install the sensor service and the
   signed driver that reads your CPU temperature and motherboard fans; nothing else needs it.

Rig LEDs installs to `Program Files`, adds a Start-menu entry, and starts. To update later, run
a newer setup the same way. To remove it: **Settings → Apps → Rig LEDs → Uninstall**.

## Verify your download

**Download:** `rig-leds-setup-1.1.1.exe`

**SHA-256 Checksum:**

`E2F4B0509ACE5D024FEF89BE13BE49611090F3BB2092B2B400E4A4314FCFAE61`

## Privacy

Rig LEDs runs entirely on your own computer. It collects **no** personal data, usage statistics
or telemetry, and the readings it shows never leave your PC.

- The **only** time it touches the internet is an anonymous check for a newer version: it asks
  GitHub for this repository's latest release number. **Nothing about you or your computer is
  sent** — no identifiers, no system details. You can turn the check off in **Settings → Display**.
- If you **report an issue**, only what you choose to paste is shared. The **Diagnostics** text
  lists your hardware and what was or wasn't read — handy for support, but review it before posting.

## Licence

Rig LEDs is closed-source freeware, licensed — not sold — under the agreement in `LICENSE.txt`
inside the download. You may install and use it for free; you may not reverse-engineer, modify,
or resell it. It is provided “as is”, with no warranty. It carries the signed PawnIO driver
(GPLv2-with-exception) and the Inter typeface (SIL OFL 1.1) under their own licences.

## Support

Found a problem or have an idea? Open a **[new issue](../../issues/new/choose)** and pick
**Bug report** or **Feature request**. For anything missing a reading, open **Settings → System**
in the app, press **Copy** under **Diagnostics**, and paste that into the bug report — it says
exactly what was found and why.
