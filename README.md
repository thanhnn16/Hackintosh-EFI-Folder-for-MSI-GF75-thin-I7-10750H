# Hackintosh EFI Folder for MSI GF75 thin I7-10750H
Hackintosh EFI Folder for MSI GF75 thin I7-10750H
This README is not complete yet. I will update it later.

# Introduction
This repository contains the EFI folder for MSI GF75 thin I7-10750H Hackintosh. This EFI folder is based on OpenCore 1.0.1 and macOS Sequoia 15.0 Beta. This EFI folder is specifically for MSI GF75 thin I7-10750H, but it can be used for other laptops with similar hardware. This EFI folder is for educational purposes only. I am not responsible for any damage caused to your device. Please read the OpenCore documentation before using this EFI folder.

# OpenCore Version
- **OpenCore**: 1.0.1
- **macOS**: Sequoia 15.0 Beta

# Image
![About This Mac](/assets/ss-1.png)

# System Specification
- **Model**: MSI GF75 thin 10SCXR
- **CPU**: Intel Core i7-10750H
- **GPU**: Intel UHD Graphics 630
- **RAM**: 16 GB 2933 MHz DDR4
- **Storage**: 1TB NVMe SSD (Crucial P3 1TB PCIe M.2 2280 SSD)
- **Audio Codec**: Realtek ALC233
- **Ethernet**: `update later`
- **Wi-Fi/BT**: `update later`
- **BIOS Version**: `latest`
- **macOS Version**: Sequoia 15.0 Beta


# What works
- [x] Intel UHD Graphics 630
- [x] Audio (ALC233)
- [x] Ethernet (RTL8168/8111)
- [x] Wi-Fi (Intel Wireless-AC 9560) using itlwm + HeliPort
- [x] Bluetooth (Intel Wireless-AC 9560)
- [x] USB Ports (USB 3.0 working, not mapped type-C)
- [x] Battery Status
- [x] Sleep/Wake
- [x] Brightness Control
- [x] Trackpad
- [x] Webcam
- [x] Microphone
- [x] iMessage, FaceTime, App Store, iCloud

# What doesn't work
- [ ] HDMI (Fixable later)
- [ ] Type-C (Fixable later)
- [ ] SD Card Reader (Not tested)
- [ ] DRM (Not tested)

# BIOS Settings
- **Disable**:
  - Secure Boot

# Installation
1. Create a bootable USB with [OpenCore](https://dortania.github.io/OpenCore-Install-Guide/installer-guide/)
2. Clone this repository to your EFI folder
3. Generate your own SMBIOS (MacBookPro16,1) using [GenSMBIOS](https://github.com/corpnewt/GenSMBIOS) and replace it in `config.plist` or simply use [OCAT](https://github.com/ic005k/OCAuxiliaryTools) to generate one
4. Boot from the USB and install macOS
5. After installation, mount the EFI partition of the SSD and copy the EFI folder from the USB to the SSD
6. Reboot and enjoy your Hackintosh!

# Kext Used
- [Lilu]()
- [VirtualSMC]()
- [WhateverGreen]()
- [AppleALC]()
- [itlwm]()
- [IntelBluetoothFirmware]()
- [HeliPort]()
- [RealtekRTL8111]()
- [VoodooI2C]()
- [VoodooI2CHID]()
- [VoodooPS2Controller]()

# Credits
- [OpenCore](https://github.com/acidanthera/OpenCorePkg)
- [Acidanthera](https://github.com/acidanthera)
- [Dortania](https://github.com/dortania)
- [OpCore-Simplify](https://github.com/lzhoang2801/OpCore-Simplify)
