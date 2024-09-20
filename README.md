
# Hackintosh EFI Folder for MSI GF75 thin I7-10750H
Hackintosh EFI Folder for MSI GF75 thin I7-10750H.

This README is not complete yet. I will update it later.

Please give a star if this EFI has helped you.

# Introduction
This repository contains the EFI folder for MSI GF75 thin I7-10750H Hackintosh. This EFI folder is based on OpenCore 1.0.1 and macOS Sequoia 15.0 Beta. This EFI folder is specifically for MSI GF75 thin I7-10750H, but it can be used for other laptops with similar hardware. This EFI folder is for educational purposes only. I am not responsible for any damage caused to your device. Please read the OpenCore documentation before using this EFI folder.

# OpenCore Version
- **OpenCore**: 1.0.1
- **macOS**: Sequoia 15.0 Beta

# Image
![About This Mac](/assets/ss-1.png)
![System Update](/assets/ss-2.png)

# System Specification
- **Model**: MSI GF75 thin 10SCXR
- **CPU**: Intel Core i7-10750H
- **GPU**: Intel UHD Graphics 630
- **RAM**: 16 GB 2933 MHz DDR4
- **Storage**: 1TB NVMe SSD (Crucial P3 1TB PCIe M.2 2280 SSD)
- **Audio Codec**: Realtek ALC233
- **Ethernet**: Realtek RealtekRTL8111
- **Wi-Fi/BT**: Intel(R) Wi-Fi 6 AX201 160MHz
- **BIOS Version**: `latest`
- **macOS Version**: Sequoia 15.0 Beta


# What works
- [x] Intel UHD Graphics 630
- [x] Audio (ALC233)
- [x] Ethernet (RTL8168/8111)
- [x] Wi-Fi: using itlwm + HeliPort
- [x] Bluetooth
- [x] USB Ports (Mapped All Ports)
- [x] Battery Status
- [x] Sleep/Wake
- [x] Brightness Control
- [x] Trackpad (can't disable via fn, will fix later)
- [x] Webcam
- [x] Microphone
- [x] iMessage, FaceTime, App Store, iCloud

# What doesn't work
- [ ] HDMI (Fixable later)
- [x] ~~Type-C (Fixable later)~~ `Now working`
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
