+++
date = '2025-01-06T01:13:15-03:00'
draft = false
title = 'How to Properly Dual Boot Windows and Linux'
+++


Windows monopoly your hardware, so it doesn't facilitates the user to use the system in a multi operational systems.  
So Windows doesn't give a damn to break other operational systems boot.  
A solution for many year was the GRUB bootloader it can easily detect Windows and Linux Systems, however GRUB is not a solid solution, unfortunately many GRUB default configuration has a anoying behavior:
* Timeout: a delay before boot to the default system, grub has no good way to change this behavior making really anoying booting your system, you can configure the timeout with the minimum of 1 second, yes, 1 second delay, and that's solve another problem, when you don't want to boot to your default system your got time to press any button and select another system.
* No easy way to change the default boot systems, every GRUB update happily overrite your configuration and your default system boot entry.
* Ugly: GRUB GUI is outdated.


Well, now the modern systems use UEFI and it has a bootloader stardard removing the need of a intermediate, GRUB.  
If possible use the EFI stub standard to configure your UEFI boot entry.

I use Ubuntu 22.04 witch automatically installs the EFI boot entry and GRUB, but GRUB doesn't show, it just boot without showing any screen, I don't know if GRUB still loads or not, the only instances where I see it is when Ubuntu updates itself GRUB shows but only once, the subsequent boots it disappers do I don't know.
