# gey gay gsi 

This document contains the list of repositories for building a Realme-based Treble ROM.

## Clone All Repositories

Use the following commands to clone all required repositories for your project.

```bash
git clone https://github.com/TrebleDroid/vendor_interfaces -b android-15.0 vendor/interfaces
git clone https://github.com/TrebleDroid/device_phh_treble -b android-15.0 device/phh/treble
git clone https://github.com/TrebleDroid/treble_app -b master treble_app
git clone https://github.com/AndyCGYan/android_packages_apps_QcRilAm -b master packages/apps/QcRilAm
git clone https://github.com/TrebleDroid/vendor_hardware_overlay -b pie vendor/hardware_overlay
git clone https://android.googlesource.com/platform/prebuilts/vndk/v28 prebuilts/vndk/v28
git clone https://android.googlesource.com/platform/prebuilts/vndk/v29 prebuilts/vndk/v29
git clone https://github.com/ponces/treble_adapter -b master treble_adapter
```


# Apply Patches Script

This repository contains a script for applying TrebleDroid and personal patches to a custom Android ROM. It automates the process of applying patches to specific directories within the ROM's source tree, ensuring a smoother integration of custom modifications.

## Overview

The `apply-patches.sh` script performs the following tasks:

1. **Apply TrebleDroid Patches:**
   - Checks and applies patches located in the `patches/trebledroid` directory.
   - Skips patches that have already been applied.
   
2. **Apply Personal Patches:**
   - Checks and applies patches located in the `patches/personal` directory.
   - Skips patches that have already been applied.

The script supports patching various directories in the source tree, such as `build`, `vendor/hardware/overlay`, and more.

## Prerequisites

To run this script, you must have the following installed:

- A Git environment (e.g., Git CLI)
- Patch utility (`patch` command)
- A local copy of the Android ROM source code

## Usage

### Steps to Apply Patches:

1. Clone this repository to your local machine.
2. Place your TrebleDroid patches in the `patches/trebledroid` directory.
3. Place your personal patches in the `patches/personal` directory.
4. Run the `apply-patches.sh` script from the root of your Android ROM source code:

   ```bash
   Bash apply-patches.sh ~/gsi
  ``
  #
