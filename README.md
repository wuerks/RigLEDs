# Rig LEDs

*A meter bridge for your rig.*

A small desktop window that shows what your computer is doing as columns of glowing LEDs:
processor, graphics, memory, fans, temperatures, disks, network and sound — plus one narrow
column per CPU core. It sounds an alarm when something runs too hot or too busy for too long,
and tells you which program is responsible. Windows 10/11, 64-bit.

## Download

Get the latest **[Release](../../releases/latest)** and download `Rig-LEDs-vX.Y.Z.zip`.

## Install

1. Unzip it, and run **`rig-leds-setup-X.Y.Z.exe`**.
2. Agree to the licence and press **Install**.
3. Windows asks for permission once — say **Yes**. (This lets it read your CPU temperature and
   motherboard fans through a signed driver; nothing else needs it.)

Rig LEDs installs to `Program Files`, adds a Start-menu entry, and starts. To update later, run
a newer setup the same way. To remove it: **Settings → Apps → Rig LEDs → Uninstall**.

## Verify your download (optional but recommended)

Each release lists the ZIP's **SHA-256**. Check the file you downloaded matches before trusting it:

```powershell
Get-FileHash Rig-LEDs-vX.Y.Z.zip -Algorithm SHA256
```

The value it prints should equal the one in the release notes (and in the `.sha256` file beside
the download). Rig LEDs also checks its own SHA-256 when it starts and warns only if it has been
tampered with.

## Licence

Rig LEDs is closed-source freeware, licensed — not sold — under the agreement in `LICENSE.txt`
inside the download. You may install and use it for free; you may not reverse-engineer, modify,
or resell it. It is provided “as is”, with no warranty. It carries the signed PawnIO driver
(GPLv2-with-exception) and the Inter typeface (SIL OFL 1.1) under their own licences.

## Support

Found a problem or have a request? Open an **[issue](../../issues)**. For anything missing a
reading, open **Settings → System** in the app, press **Copy** under **Diagnostics**, and paste
that in — it says exactly what was found and why.
