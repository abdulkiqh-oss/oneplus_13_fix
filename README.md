# OnePlus 13 Fix & OnePlus/OPPO EDL Firehose Collection

A comprehensive collection of Qualcomm Emergency Download (EDL) Firehose programmers, signatures, and tools specifically structured for OnePlus and OPPO devices, including support for Snapdragon chips and the `oneplus_13_fix` toolset.

---

## 📂 Repository Structure

### 1. `Firehose/`
Contains Qualcomm EDL programmers (`.elf`, `.melf`), signatures (`.bin`), and digests categorized by SoC models:
* **SM8750 / Snapdragon 8 Elite (8E):** Firehose loaders and boot images for flagship platforms.
* **SM8650 / Snapdragon 8 Gen 3:** Firehose loaders (`V1.0.21.melf`) with corresponding Digest and Sign files.
* **SM8475 / SM8450 (8+ Gen 1 / 8 Gen 1 / 8 Gen 2 / 7+ Gen 2):** Complete Firehose sets.
* **Mid-Range SoCs:** Loaders for SM6375 (695), SM6115 (460), 710/670/712, 765G series, SDM845, and legacy models.

### 2. `op13_firehose/`
Dedicated Firehose package for **OnePlus 13 / SM8475 platform variant**, containing:
* `SM8475_V3.0.melf`
* `Digest.bin`
* `Sign.bin`

### 3. `OplusEdlTool/`
A CLI toolset based on .NET 8 for flashing and communicating with OPPO/OnePlus devices in Qualcomm EDL (9008) mode:
* **Executables:** `OplusEdlTool.exe`
* **Qualcomm Tools:** `QSaharaServer.exe`, `fh_loader.exe`
* **Image Utilities:** `simg2img.exe`, `lpmake.exe`, `lsusb.exe`

---

## 🛠️ Usage

1. Put your device into **Qualcomm EDL Mode (9008)**.
2. Navigate to `OplusEdlTool/` or use `QSaharaServer.exe` / `fh_loader.exe`.
3. Select the appropriate Firehose loader (`.elf` / `.melf`) along with its matching `Digest.bin` and `Sign.bin` files from the `Firehose/` folder corresponding to your device's SoC.

---

## ⚠️ Disclaimer

* These files are intended for advanced developers, repair technicians, and researchers.
* Flashing incorrect Firehose files or modifying partitions can cause permanent bricking.
* Use at your own risk.
