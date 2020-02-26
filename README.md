# MSI-GF63-Thin-9SC-257
MSI GF63 Thin 9SC-257 Laptop
i5-9300H
GeForce GTX 1650 Max-Q

MacOS Catalina 10.15.3
Kingston NVMe 512gb (Windows 10)
Samsung 860 Evo 1tb SSD (MacOS Catalina 10.15.3)

Clover 5103 is the current Clover boot loader.

This took a bit to setup. Tried various USB installers (Tonymac, Olarila, Niresh) to get this up. Only one that seemed to work was Niresh Mojave (which was version 10.14.1). Had to install as Legacy. UEFI would not work. Could not get the Samsung 860 Evo  SSD to recognize to boot up without the USB installer in the USB drive. In order to get Catalina installed I had to manually update each Mojave update (10.14.2 and then 10.14.3 and then 10.14.4). After each install it would go to black screen. Had to reboot after each one and use the USB installer to get into Clover and choose MacOS Install on (computer name). Once that got setup updated to Catalina 10.15.3 from the System Preferences, Update pane.

Clover was setup with Legacy install. Was too much going on to remember the settings for it so that is why the EFI is attached here.

Have to go into BIOS and set it to Legacy on boot up and then save and reboot. Reboots perfectly fine without USB installer attached.

Have to go into BIOS and set it to UEFI with CSM in order to boot into Windows 10 with the Kingston NVMe 512gb SSD.


What is working:
Audio (installed VoodooHDA 2.9.1 to System/Library/Extensions with Kext Utility
Installed AppleHDADisabler.kext to System/Library/Extensions with Kext Utility
Audio layout in Clover is set to ID 2

Ethernet
Camera (using Function + F6 keys)
Facetime (Through Ethernet until wifi card arrives. Will update then.)
iMessage (Through Ethernet until wifi card arrives. Will update then.)
All USB ports seem to be working fine. They are listed using Hackintool as: HS02 (USB 3.2 Gen 1 Type-C), HS03 (USB 3.2 (Gen 1 Type-A), HS04 (USB 3.2 (Gen 1 Type-A), HS05 (USB 3.2 Gen 1 Type-A). Don't think full speeds are there though but not really sure that is an issue either. Would be nice to have full speed on them.
Brightness functions in Display settings works fine. Can't figure out how to work them with keyboard though.


Not working:
Intel HD 630 Graphics. Doesn't show up in System Information and listed as Intel HD 630 CFL CRB 1536 MB. Graphics seems to work fine. No lag noticed. Youtube videos play fine with no lag.

Still get the black screen which takes about 3-4 minutes to get past once it passes the verbose screen. Can't figure out how to get rid of that.

Also need to why the Intel HD 630 doesn't show up in the System Information and need to verify if the Nvidia 1650 is disabled or not.
