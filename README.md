# withsudo_arch
proxy utility for running yay/yaourt/etc under root

## Example of usage:

`withsudo yay -Syu --noconfirm`
or
`withsudo yaourt -Syua --noconfirm`

## Problem:

Generally utilities for updating AUR packages do not work under root account. I mean those `yay` or `yaourt`. So far it's impossible to call them by cron to auto update OS.

This proxy utility solves this problem. Just copy this script somewhere to your PATH and prepend your command which updates your system with `withsudo` and then magic happens.

## Requirements:

You should install `sudo` before you can use this script:
- `pacman -S sudo`
