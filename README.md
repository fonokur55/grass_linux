# GRASS Linux

A custom Arch based Linux distribution with a green Hyprland desktop, a full gaming stack, and its own terminal installer.

GRASS Linux is a ready to use system for people who want a modern tiling desktop without spending days setting everything up. It boots into a themed Hyprland rice, comes with useful apps preconfigured, and can be installed to disk with a simple terminal installer that supports encryption and dual boot. Under the hood it is still plain Arch, so you can change anything you want.

## Download

Latest ISO (3.4 GB): **[grass-linux.iso](https://archive.org/download/grass-linux/grass-linux.iso)**

Torrent: **[grass-linux.iso.torrent](https://archive.org/download/grass-linux/grass-linux_archive.torrent)**

Item page: [archive.org/details/grass-linux](https://archive.org/details/grass-linux)

Write the ISO to a USB stick (Ventoy is the easiest: just copy the .iso onto a Ventoy drive), boot from it, and you get a live session you can try before installing.

## Features

### Desktop
* Hyprland tiling window manager with a green rice (waybar, rofi, swaync, wlogout)
* Dynamic theme colors: the whole desktop recolors itself to match your wallpaper (matugen)
* kitty terminal, nemo file manager, int_clay glassy icons, macOS style cursor
* Wallpaper picker, keyboard layout switcher (hu / us), and a built in WiFi menu
* Screenshot tool (grim + slurp + swappy) with region select and annotation

### Gaming and apps
* Steam, Lutris, GameMode, MangoHud, Gamescope, multilib enabled
* Wine with double click .exe support
* LibreOffice, VLC with codecs, qBittorrent, Wireshark
* Fun extras: cbonsai, cmatrix, tty-clock, lavat, pacseek

### Installer
GRASS Linux ships with its own terminal based installer (grass-install). It supports:
* Automatic whole disk install
* Manual partitioning (via cfdisk) and dual boot alongside an existing OS
* Full disk encryption with LUKS2
* Automatic GPU driver detection and install (NVIDIA and AMD)
* A real non root user with sudo, zram swap, NetworkManager, firewall, and NTP

## Installation

1. Boot the ISO from your USB stick (the live desktop starts automatically).
2. Open a terminal with SUPER + ENTER and run:

   ```
   grass-install
   ```

3. Follow the steps. Use the arrow keys to move, Tab to switch buttons, and Enter to confirm.
   You will choose a disk, a partition mode (auto, manual, or dual boot), optional LUKS encryption,
   a hostname, and a user account.
4. When it finishes, reboot and remove the USB stick.

If you chose encryption, you will be asked for your passphrase at every boot.

## Keyboard shortcuts

| Shortcut | Action |
| --- | --- |
| SUPER + ENTER | Terminal (kitty) |
| SUPER + E | File manager |
| SUPER + F | Fullscreen |
| SUPER + W | Wallpaper picker (recolors the theme) |
| SUPER + B | Browser |
| SUPER + L | Lock screen |
| SUPER + SHIFT + S or Print | Screenshot (region) |
| SUPER + Print | Screenshot (full screen) |

To connect to WiFi, click the network icon in the top bar, pick your network, and enter the password.

## Built on Arch

GRASS Linux is a curated Arch Linux setup. Nothing is locked down. You get the rolling release,
pacman, the AUR, and full control to modify or extend the system however you like.

## Notes

* Tested on real hardware and in virtual machines across all installer modes.
* This is a personal project shared for anyone who likes this setup.
* Always back up important data before installing any operating system.
