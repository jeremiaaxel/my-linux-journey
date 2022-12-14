---
tag: issue, audio, microphone, driver
is_solved: true
date: 2022-12-14
solve_date: 2022-12-14
---
Description: After fresh install of Linux, headphone's microphone is not showing up on sound settings.
Device: ![[Device - Asus Vivobook Pro 14 OLED]]
OS: ![[OS - Pop!_OS 22.04 LTS]]

Solution: 
1. Edit `/etc/modprobe.d/alsa-base.conf`.
2. Add `options snd-hda-intel index=1,0 model=auto,dell-headset-multi`.
3. Reboot
Reference: https://bbs.archlinux.org/viewtopic.php?id=279083

