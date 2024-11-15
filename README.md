# Arch Linux Install Script

Automates Arch install with LUKS encryption, LVM, Systemd-boot, and user setup.

## Features
- **Encryption & LVM**: Sets up secure root with LUKS and LVM.
- **System Install**: Base system, hardened kernel, essential packages.
- **User & Security**: Adds sudo user, configures TODO Firejail, security modules.
- **Bootloader**: Systemd-boot setup.
- **Custom Packages**: Installs from `packages.cfg` and AUR via Yay.

## Manual Partitioning
Before running the script, create two partitions manually:
1. **Boot Partition**: 512 MB (EFI, type `ef00`).
2. **Root Partition**: Remaining space (for LUKS encryption).

## Usage
1. Edit variables
2. Run as root in a live Arch environment.
3. Ensure `packages.cfg` is present in the same directory.
