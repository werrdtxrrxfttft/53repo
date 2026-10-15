<!-- ASTER_XFCE_DOWNLOAD_BEGIN -->
# Aster Linux 0.2.1 XFCE desktop

[Download aster-linux-xfce.iso](https://github.com/werrdtxrrxfttft/53repo/raw/refs/heads/aster-iso-download/aster-linux-xfce.iso) ·
[SHA-256 checksum](https://github.com/werrdtxrrxfttft/53repo/raw/refs/heads/aster-iso-download/aster-linux-xfce.iso.sha256) ·
[Package manifest](https://github.com/werrdtxrrxfttft/53repo/raw/refs/heads/aster-iso-download/desktop-manifest.json)

This x86-64 live ISO includes Debian 13, XFCE, graphical login, networking,
and the `apt` package manager. The desktop logs in automatically as **aster**;
the password is **aster**. Open Terminal to run `sudo apt update` or install
packages with `sudo apt install PACKAGE`.

For VirtualBox, choose Linux / Debian (64-bit), **2 GB RAM**, **2 CPUs**,
**128 MB video memory**, and **3D acceleration off**. Attach the ISO as the
virtual optical disk. NAT provides networking.

For a black desktop screen, power off the VM, **disable EFI**, and select
**VBoxSVGA** or **VMSVGA** graphics. Boot the ISO and choose **Aster Linux
0.2.1 - XFCE desktop (legacy graphics, BIOS only)**. This adds a VESA graphics
path for BIOS boot; its behavior still needs confirmation in VirtualBox.
The **native graphics** and **safe graphics** menu entries remain available.
Those entries support BIOS or x86-64 UEFI; disable Secure Boot when using UEFI.

The boot menu waits **10 seconds**. Press an arrow key to keep it open while
choosing an entry. Boot now displays loading messages and local system startup
progress instead of hiding it with `quiet`.

If graphics still fail, choose **Aster Linux 0.2.1 - text recovery and
diagnostics**. The local console logs in automatically as **aster**. Run
`aster diagnose` to collect graphics, display-manager, and boot diagnostics.

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
