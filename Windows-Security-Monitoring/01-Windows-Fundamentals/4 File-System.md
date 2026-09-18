# Windows File System

## Overview

Windows uses a file system to organize and manage files,
directories, and storage volumes.

## Important File System

- NTFS

## Important Directories

- C:\Windows
- C:\Windows\System32
- C:\Users
- C:\Program Files
- C:\Program Files (x86)
- C:\ProgramData
- C:\Users\<User>\AppData
- C:\Users\<User>\Downloads
- C:\Users\<User>\AppData\Local\Temp

## NTFS Security

- Security Descriptors
- DACL
- SACL
- Ownership
- Permission Inheritance

## NTFS Metadata

- File timestamps
- File attributes
- MFT
- File metadata

## File Hashing

Command used:

Get-FileHash "<file>" -Algorithm SHA256

Purpose:

SHA256 can be used as a file identifier and IOC during
security investigations.

## Hands-on Labs

### Lab 1 — File System Exploration

Commands:

Get-Location
Get-ChildItem
Get-ChildItem C:\Windows
Get-ChildItem C:\Windows\System32

### Lab 2 — File Metadata

Command:

Get-Item "<file>"

### Lab 3 — File Hash

Command:

Get-FileHash "<file>" -Algorithm SHA256

### Lab 4 — File Permissions

Command:

Get-Acl "<file>"

## Investigation Mindset

Suspicious File
→ Path
→ Metadata
→ Hash
→ Signature
→ Owner
→ Permissions
→ Process
→ Parent Process
→ Network Activity
→ Logs
→ Threat Intelligence
