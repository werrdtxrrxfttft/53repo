# Aster Linux ISO

Bootable x86-64 live CD, tested in QEMU using BIOS and UEFI.

Download `aster-linux.iso` using GitHub's Download raw file button.
For UEFI, disable Secure Boot. The system opens a root text console and runs
entirely in RAM; files disappear at shutdown. Type `aster help` to explore
and `poweroff` to shut down.

Use `sha256sum -c aster-linux.iso.sha256` to verify the download.
Package versions and hashes are recorded in `iso-manifest.json`.
