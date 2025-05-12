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
