# **Lenovo ThinkPad L380 — macOS Sequoia Hackintosh (OpenCore 1.0.7)**

This repository contains my fully working **macOS Sequoia (15.x)** Hackintosh configuration for the **Lenovo ThinkPad L380**.
The system runs smoothly with **native Intel Wi-Fi support via AirportItlwm** and excellent stability on **OpenCore 1.0.7**.

---

## 🖥️ **System Overview**

| Component               | Details                            |
| ----------------------- | ---------------------------------- |
| **Model**               | Lenovo ThinkPad L380               |
| **CPU**                 | Intel Core i3 (8th Gen)            |
| **iGPU**                | Intel UHD Graphics 620             |
| **RAM**                 | 20GB DDR4                          |
| **Storage**             | *Western Digital* 512GB NVMe SSD   |
| **macOS Version**       | macOS Sequoia (15.x)               |
| **Bootloader**          | OpenCore **1.0.7**                 |
| **Wi-Fi**               | Fully working via **AirportItlwm** |
| **Bluetooth**           | Fully working                      |
| **Audio**               | Working via AppleALC               |
| **Webcam**              | Working                            |
| **Trackpad**            | Working                            |

---

## ✅ **What Works**

Everything listed below has been tested and verified:

* **Native Intel Wi-Fi** via AirportItlwm
* **Bluetooth**
* **Intel UHD 620 Graphics Acceleration (QE/CI)**
* **USB Ports** (custom mapped)
* **Audio**: speakers, headphones, microphone
* **Webcam**
* **Trackpad + Precision Gestures (VoodooI2C)**
* **Sleep / Wake**
* **Battery Percentage**
* **Power Management & CPU scaling**
* **iMessage / FaceTime / App Store / iCloud**
* **FileVault** — *works out of the box without additional configuration*
* **SMBIOS compatibility** (MacBookPro15,2 recommended)

---

## ⚠️ **What Doesn’t Work**

You tell me.

Everything else functions reliably.

---

## 🔧 **BIOS Settings**

This ThinkPad works with minimal BIOS modifications.

### **Disable**

* **Secure Boot** (required)

### **Everything else**

Default settings work properly.

---

## 🚀 **Installation Steps**

1. Create a macOS Sequoia USB installer using macOS or `gibMacOS`.
2. Copy this repository’s `EFI` folder into the EFI partition of your USB installer.
3. Generate your own SMBIOS (recommended: `MacBookPro15,2`) using **GenSMBIOS**.
4. Boot from USB and proceed with installation.
5. After installation, mount the internal drive’s EFI and copy over the OpenCore EFI.

---

## 🛠️ **Post-Install Notes**

* Very stable sleep/wake behavior
* Smooth Intel UHD 620 graphics acceleration
* Native Wi-Fi menu integration with AirportItlwm
* Reliable Bluetooth
* Accurate battery reporting
* Custom USB mapping for proper port behavior

---

## 🙏 **Credits**

* **OpenCore Team**
* **acidanthera** (Lilu, WhateverGreen, VirtualSMC, AppleALC)
* **OpenIntelWireless** (AirportItlwm, Intel Bluetooth)
* **Dortania** documentation
* **OCsimplify** for easy open core config making
* Hackintosh community


