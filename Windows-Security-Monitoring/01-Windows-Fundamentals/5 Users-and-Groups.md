# Windows Users and Groups

## Overview

Windows uses user accounts, groups, security identifiers,
access tokens, permissions, and privileges to control access
to system resources.

## User Types

- Local User
- Domain User

## Important Local Groups

- Administrators
- Users
- Guests
- Remote Desktop Users

## Security Identifier (SID)

A SID uniquely identifies a Windows security principal.

Example format:

S-1-5-21-...

## Access Token

An access token represents the security context of a user or
process and contains information such as SIDs and privileges.

## UAC

User Account Control helps prevent unauthorized elevation
to administrative privileges.

## Integrity Levels

- Low
- Medium
- High
- System

## Permissions vs Privileges

Permissions control access to resources such as files and
folders.

Privileges represent specific rights granted to a security
principal.

## Hands-on Commands

whoami
whoami /user
whoami /groups
whoami /priv
Get-LocalUser
Get-LocalGroup
Get-LocalGroupMember -Group "Administrators"

## Investigation Example

Alert:
A user was added to the local Administrators group.

Investigation:

User
→ SID
→ Group Membership
→ Privileges
→ Login Activity
→ Process Activity
→ PowerShell/CMD
→ Network Activity
→ Windows Logs

## Security Relevance

User and group information provides important context when
investigating authentication, privilege escalation, suspicious
processes, and account-related security alerts.
