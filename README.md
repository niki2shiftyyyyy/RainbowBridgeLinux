# 🌈 Rainbow Bridge OS

A privacy-focused Linux distribution based on Debian Bookworm, designed for people who want privacy out of the box without the complexity.

Sits between Tails OS and a normal desktop distro — persistent, usable, and private by default.

## Features

- Boots straight into GNOME
- Privacy defaults baked in (MAC randomization, encrypted DNS, firewall)
- Simple installer — just run `sudo rbi` from the terminal
- Clean base — install what you want, nothing you don't
- USB watchdog shutdown protection
- Built on Debian Bookworm with systemd

## Usage

Boot the ISO from USB. You'll be dropped into a live GNOME session.

To install to disk, open a terminal and run:

```bash
sudo rbi
```

Follow the prompts. That's it.

## Building

Requirements: `live-build`, `systemd-nspawn`, Debian Bookworm chroot

```bash
sudo systemd-nspawn -D ~/debian-chroot
cd ~/rainbowbridge
lb clean && lb build
```

## Philosophy

Privacy should be the default, not an afterthought. Rainbow Bridge OS is for people who want a system that works — with strong privacy built in — without having to configure everything themselves.

## License

GNU General Public License v3.0
