# Lenovo Ideapad 330 Linux kernel configuration
This config file is for Lenovo Ideapad 330 laptop (Specifically 15ICH model).

## What is working
Everything, including webcam, touchpad, battery status, Wi-Fi (If adapter is Intel Dual-Band Wireless AC 3165 or similar), Bluetooth, sound, etc...

## Notes
**DO NOT UPGRADE TO KERNEL >= 4.18 UNTIL ACPI BUG GETS FIXED!**, I recommend 
using **4.14.101**.

## How to use
1. Rename "config" file to ".config"
2. Move it to Linux source tree directory.
3. Build the kernel.
5. Copy xorg.conf to /etc/X11 to enable external GPU (Nvidia).
6. (OPTIONAL) If you want to enable "Double tap to click" on touchpad, copy 
"40-libinput.conf" to /etc/X11/xorg.conf.d.

linux-firmware package is required for Wi-Fi to work.
