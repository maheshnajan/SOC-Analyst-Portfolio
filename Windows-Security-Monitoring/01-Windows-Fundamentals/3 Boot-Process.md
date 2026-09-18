# Windows Boot Process

## Overview

The Windows boot process is the sequence through which the system
initializes firmware, boot components, the kernel, drivers, system
processes, services, and finally the user session.

## Boot Sequence

Power On
→ UEFI
→ Secure Boot
→ Windows Boot Manager
→ BCD
→ Windows OS Loader
→ Windows Kernel
→ Boot Drivers
→ smss.exe
→ System Initialization
→ Services
→ Login
→ Windows Desktop

## Important Components

- UEFI
- Secure Boot
- Windows Boot Manager
- BCD
- bootmgfw.efi
- winload.efi
- ntoskrnl.exe
- Boot-start drivers
- smss.exe

## Security Relevance

The boot process is important for security because attackers may
attempt to establish persistence or execute malicious code at
early stages of system startup.

## Hands-on

Commands:

msinfo32
Confirm-SecureBootUEFI
bcdedit /enum

## Observations

- BIOS Mode:
- Secure Boot:
- Boot Manager:
- Windows Loader:
- Windows System Root:

## SOC Relevance

Understanding the boot process helps analysts investigate
boot-level persistence, suspicious drivers, and system integrity issues.
