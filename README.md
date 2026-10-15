<!-- ASTER_XFCE_DOWNLOAD_BEGIN -->
# Aster Linux XFCE desktop

[Download aster-linux-xfce.iso](https://github.com/werrdtxrrxfttft/53repo/raw/refs/heads/aster-iso-download/aster-linux-xfce.iso) ·
[SHA-256 checksum](https://github.com/werrdtxrrxfttft/53repo/raw/refs/heads/aster-iso-download/aster-linux-xfce.iso.sha256) ·
[Package manifest](https://github.com/werrdtxrrxfttft/53repo/raw/refs/heads/aster-iso-download/desktop-manifest.json)

This x86-64 live ISO includes Debian 13, XFCE, graphical login, networking,
and the `apt` package manager. The desktop logs in automatically as **aster**;
the password is **aster**. Open Terminal to run `sudo apt update` or install
packages with `sudo apt install PACKAGE`.

For VirtualBox, choose Linux / Debian (64-bit), **2 GB RAM**, **2 CPUs**,
**VMSVGA** graphics, **128 MB video memory**, and **3D acceleration off**.
Attach the ISO as the virtual optical disk and boot it. BIOS and x86-64 UEFI
are supported; disable Secure Boot when using UEFI. NAT provides networking.
If the desktop stays black, select **Aster Linux 0.2 - XFCE desktop (safe
graphics)** in the boot menu. Press an arrow key during the two-second menu
countdown to keep the menu open while choosing the entry.

This is a live desktop with no disk installer. Files, settings, and packages
installed in the running VM reset after shutdown.

Verify the downloaded ISO with `sha256sum -c aster-linux-xfce.iso.sha256`.
The desktop ISO is stored using Git LFS; use the download link above or
GitHub's **Download raw file** button to obtain the complete image.
<!-- ASTER_XFCE_DOWNLOAD_END -->

## Original console ISO

Bootable x86-64 live CD, tested in QEMU using BIOS and UEFI.

Download `aster-linux.iso` using GitHub's Download raw file button.
For UEFI, disable Secure Boot. The system opens a root text console and runs
entirely in RAM; files disappear at shutdown. Type `aster help` to explore
and `poweroff` to shut down.

Use `sha256sum -c aster-linux.iso.sha256` to verify the download.
Package versions and hashes are recorded in `iso-manifest.json`.

