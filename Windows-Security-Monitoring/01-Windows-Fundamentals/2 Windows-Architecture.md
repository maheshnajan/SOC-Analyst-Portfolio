# Windows Architecture

## Overview

Windows operates using user-mode and kernel-mode components.

## User Mode

- Applications
- Processes
- PowerShell
- CMD
- User-mode services

## Kernel Mode

- Windows Kernel
- Drivers
- Memory management
- I/O management
- Process/thread management

## Process

A process is a running instance of a program.

## PID

Every running process has a unique Process ID.

## Thread

A thread is an execution unit within a process.

## Process Tree

Parent processes can create child processes.

Example:

WINWORD.EXE
    |
    └── powershell.exe

## Security Relevance

Process trees help SOC analysts understand how suspicious processes were launched.

## Hands-on

Commands used:

Get-Process
Get-Process | Select-Object ProcessName, Id, CPU
Get-Process powershell

## Investigation Mindset

Process
→ PID
→ Parent Process
→ Child Process
→ Command Line
→ File Activity
→ Network Activity
→ Logs
→ Verdict
