# postmarketOS Device Package for Xiaomi Redmi Note 10 (mojito)

This repository contains the main device package configuration (`device-xiaomi-mojito`) for porting **postmarketOS** to the **Xiaomi Redmi Note 10** (codename: `mojito`).

It is used by `pmbootstrap` to handle core device dependencies, kernel requirements, and initramfs modules.

---

## 📂 Repository Contents

* **`APKBUILD`**: The Alpine Linux package recipe defining primary dependencies such as `linux-xiaomi-mojito`, `mkbootimg`, and `postmarketos-base`.
* **`deviceinfo`**: Configuration file specifying architecture (`aarch64`), flash offsets, boot parameters, and screen properties.
* **`modules-initfs`**: List of essential kernel modules loaded during early boot in the initramfs stage.

---

## 🛠️ How to Build

1. Place this directory in your local `pmaports` tree under `device/testing/device-xiaomi-mojito`.
2. Build the device package and generate the installation image using `pmbootstrap`:
   ```bash
   pmbootstrap build device-xiaomi-mojito
   pmbootstrap install
