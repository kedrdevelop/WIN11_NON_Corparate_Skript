# Windows 11 Unattended Setup

Universal unattended setup configuration (`autounattend.xml`) for automated Windows 11 installation.

## Features

- **Automated Setup:** Locale and keyboard configured to `de-DE`.
- **Storage:** Automatically formats and partitions Disk 0 (GPT: EFI, MSR, Primary NTFS).
- **Account:** Creates a local administrator account (`User`) with passwordless auto-logon.
- **OOBE Bypass:** Skips all OOBE setup and online account requirements.
- **Native Drivers:** Supports automatic driver injection via the `$WinPEDriver$` root directory on the installation media.

## Usage

1. Place `autounattend.xml` in the root of your bootable Windows 11 USB drive.
2. (Optional) Place extracted driver folders (`.inf` files) into a `$WinPEDriver$` directory at the root of the USB drive.
3. Boot the system from the USB drive. The installation will proceed automatically.
