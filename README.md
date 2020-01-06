# EFI for Catalina 10.15.1

## working
- everything (maybe not audio because i use external AUDIO interface)

## Specs
- CPU: **i7-7700k**
- GPU: **AMD 580 4Gb**
- MOAB: **msi Z270-A PRO**
- DISK: **samsung 850 EVO**
- network: **TP-Link WDN4800**
- bluetooth: **logitech dongle**
- display: **LG ultrawide 16:9**

# Instructions:
- follow a generic guide to create the usb installer
- copy this repository EFI in the installer EFI partition
- install catalina
- copy this EFI in the new catalina disk
- boot inside catalina disk and
  - make the disk writable with `sudo mount -uw /` to be able to follow the below steps
  - to make TP-Link WDN4800 work use [Atheros patch](https://www.insanelymac.com/forum/files/file/956-atheros-installer-for-macos-mojave-and-catalina/)
  - if you use different CPU change the ig-platform-id and smbios
  - if using a non standard display (ultrawide, 4k) use [mac-pixel-clock-patch-V2](https://github.com/Floris497/mac-pixel-clock-patch-V2)
