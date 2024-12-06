# Windows XP Service Pack 5

> [!WARNING]
> This project is far from finished, meaning that bugs are to be expected. If you encounter any bugs, please report them in the issue tracker or in the Discord server. Thank you for your understanding.

Windows XP Service Pack 5 is a package consisting of updates, tweaks, backported apps and overall enhancements with the goal of providing an effortless way to have a fully updated Windows XP ISO and enhancing usability on semi-modern machines.

## Service Pack 5 currently includes:

- [x] - All updates released since Service Pack 2, including the latest Windows Server 2003 update
- [x] - Snipping Tool from Windows 10 version 1507 -> Credits: vxiduu
- [ ] - Paint from Windows 10 version 1703
- [x] - Registry Editor from Windows 10 version 1703 -> Credits: [Aurorarion](https://github.com/AurorarionWin/)
- [ ] - In-place service pack installer
- [x] - Native USB 3.0 and NVMe support -> Credits: Unknown user from MyDigitalLife forums
- [x] - TPM 2.0 support
- [ ] - UEFI support in the ISO releases, with EFI GOP support too
- [x] - Inclusion of OneCore API -> Credits: Skulltrail192
- [x] - Windows 7 PE in the ISO
- [x] - Windows 10 setup engine in the ISO release -> Credits: [Aurorarion](https://github.com/AurorarionWin/) (helping out on the 10 setup engine port)
- [x] - Builtin Webp and FLAC codecs
- [ ] - Upscaled graphics in some places
- [x] - Windows XP's boot screen on the ISO
- [ ] - Better DPI support
- [ ] - Integration of Microsoft Visual C++ Redistributable AIO -> Credits: Microsoft Corporation (Visual C++) and [abbodi1406](https://github.com/abbodi1406/) (VC++ AIO repack)

## Installation

> [!CAUTION]
> Failure to follow instructions properly will result in a bricked system! We do not take responsibility for this unless this is a legitimate bug in the installer!

> [!IMPORTANT]
> RAID Storage is not supported. Only NVMe is added. Read below in the FAQ for why we did not add RAID.

> [!WARNING]
> Both versions of the Windows XP Service Pack 5 are x64 only! Don't file issues over the lack of 32-bit hardware support as we do not plan to support 32-bit hardware. Consult the FAQ for more information.

### ISO installation

> [!IMPORTANT]
> The ISO releases are for clean installs only. For in-place installs, please use the installer once we release a working version of it.

1. Pick the UEFI or Legacy Boot version, depending on what your system uses
2. Flash it onto a DVD or a USB flash drive
3. Boot from the Windows XP install media on the machine you wish to install it in
4. Proceed as usual
5. Finish the out of box experience

### In-place intallation

- Download the Windows XP SP5 installer under the releases of this repository
- Follow the steps in the installer as usual

> [!WARNING]
> If the installer is stuck at a certain percentage (during the Upgrading Windows phase), don't turn off your computer! Doing so will brick your system!

## FAQ

### Q: My system is 32-bit in hardware. Why won't the installer and the ISO run?

A: Supporting both 64-bit and 32-bit Windows would be very time consuming, so we chose to support only 64-bit systems. Please don't file any issues regarding the lack of 32-bit support as we have no interests of making any releases targeting 32-bit hardware.

### Q: Why don't you include ESU updates?

A: ESU updates will be rolled out by Microsoft until 2026, and unfortunately adding ESU updates will be time consuming as it requires us to roll out new releases every time a batch of ESU updates gets rolled out.

### Q: Why OneCore API instead of the Windows XP Extended Kernel?

A: OneCore API is safer than the Windows XP Extended Kernel as it relies on external DLLs.

### Q: Does this include custom integrated GPU dri-

A: **NO**

### Q: Does it come with RAID storag-

A: Well to answer your question, how would we add RAID if it's not even supported by intel/other manufacturers?

