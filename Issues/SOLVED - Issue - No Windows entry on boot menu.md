---
tag: issue, Windows, dual boot, grub
is_solved: true
date: 2022-12-15
solve_date: 2022-12-15
---
Description: Dual booting Pop!\_OS with Windows 11. After fresh installation of Pop!\_OS, automatically boots to Linux, without GRUB menu and Windows entry.
Device: ![[Device - Asus Vivobook Pro 14 OLED]]
OS: ![[OS - Pop!_OS 22.04 LTS]]

Solution: 
1. Open terminal
2. Run `lsblk`.\
    If Windows is installed first, probably the first entry/partition.
3. Copy the Microsoft EFI\
    `sudo cp -ax /dev/<Windows' partition>/EFI/Microsoft /boot/efi/EFI`

Reference: https://github.com/spxak1/weywot/blob/main/Pop_OS_Dual_Boot.md#4-tldr-dual-boot-from-the-same-drive-with-windows-and-pop_os-already-installed

