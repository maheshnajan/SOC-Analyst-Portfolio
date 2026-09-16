# Windows Security Monitoring & Investigation

## 📌 Project Overview

This project documents my practical learning and hands-on work in **Windows Security, Windows Internals, Security Monitoring, Threat Detection, and SOC Investigation**.

The goal is to understand how Windows systems work, how attackers abuse Windows features, how those activities appear in logs and telemetry, and how a SOC Analyst can investigate and respond to suspicious activity.

This repository is being built as a **practical cybersecurity portfolio project**, not just as a collection of theoretical notes.

---

## 🎯 Objectives

* Understand Windows operating system fundamentals
* Understand Windows security architecture
* Learn Windows users, groups, permissions, processes, and services
* Understand Windows authentication
* Learn NTLM and Kerberos fundamentals
* Understand Windows networking
* Learn Windows Event Viewer and security logs
* Analyze important Windows Event IDs
* Learn Sysmon and endpoint telemetry
* Investigate suspicious processes and process trees
* Understand Windows persistence techniques
* Investigate PowerShell activity
* Understand common Windows attack techniques
* Detect suspicious Windows behaviour
* Perform SOC-style Windows investigations
* Create professional investigation reports

---

## 🧠 Learning Areas

### 1. Windows Fundamentals

* Windows Architecture
* Windows Boot Process
* File System
* Users and Groups
* Local Accounts
* Domain Accounts
* Permissions
* NTFS Permissions
* Processes
* PIDs
* Parent/Child Processes
* Services
* Registry

### 2. Windows Administration & Command Line

* CMD
* PowerShell
* Task Manager
* Services
* Event Viewer
* Windows networking commands
* Process investigation commands
* File and permission commands

### 3. Windows Authentication

* Windows Authentication
* NTLM
* Kerberos
* Logon Types
* Authentication Events
* Failed Authentication
* Successful Authentication
* Account Lockouts

### 4. Windows Security Monitoring

* Windows Event Viewer
* Security Logs
* System Logs
* Application Logs
* PowerShell Logs
* Sysmon
* Process Creation
* Network Connections
* File Creation
* Service Creation
* Scheduled Tasks

### 5. Important Security Events

Examples include:

* Event ID 4624 — Successful Logon
* Event ID 4625 — Failed Logon
* Event ID 4688 — Process Creation
* Event ID 4672 — Special Privileges Assigned
* Event ID 4720 — User Account Created
* Event ID 4728 — Member Added to Security-Enabled Global Group
* Event ID 4732 — Member Added to Security-Enabled Local Group
* Event ID 7045 — New Service Installed

Event IDs will be studied with their context, fields, limitations, and investigation value rather than memorized alone.

---

## 🔍 Investigation Methodology

The investigation process used in this project:

```text
Alert
  ↓
Identify Host
  ↓
Identify User
  ↓
Identify Process
  ↓
Check Parent Process
  ↓
Review Windows Logs
  ↓
Check Network Activity
  ↓
Identify IOC
  ↓
Threat Intelligence
  ↓
Build Timeline
  ↓
Map MITRE ATT&CK
  ↓
Determine Severity
  ↓
Contain / Escalate
  ↓
Document Findings
```

---

## 🧪 Practical Labs

Practical work will include:

* Windows local lab
* TryHackMe Windows security labs
* Windows Event Viewer investigations
* Sysmon investigations
* Process analysis
* PowerShell investigations
* Authentication investigations
* Suspicious network connection analysis
* Persistence investigations
* Malware behaviour analysis

---

## 🛠️ Tools

### Windows Tools

* Event Viewer
* Task Manager
* CMD
* PowerShell
* Windows Defender
* Services
* Registry Editor
* Resource Monitor
* Performance Monitor
* Sysmon

### Security Tools

* Wireshark
* Nmap
* VirusTotal
* CyberChef
* Splunk
* Microsoft Sentinel
* MITRE ATT&CK

---

## 📂 Repository Structure

```text
Windows-Security-Monitoring/
│
├── README.md
│
├── 01-Windows-Fundamentals/
│   ├── Windows-Architecture.md
│   ├── Boot-Process.md
│   ├── File-System.md
│   ├── Users-and-Groups.md
│   └── Permissions.md
│
├── 02-Processes-Services-Registry/
│   ├── Processes.md
│   ├── Process-Trees.md
│   ├── Services.md
│   └── Registry.md
│
├── 03-CMD-PowerShell/
│   ├── CMD-Commands.md
│   ├── PowerShell-Basics.md
│   └── PowerShell-Security.md
│
├── 04-Windows-Authentication/
│   ├── Authentication.md
│   ├── NTLM.md
│   ├── Kerberos.md
│   └── Logon-Types.md
│
├── 05-Windows-Event-Logs/
│   ├── Event-Viewer.md
│   ├── Security-Logs.md
│   ├── Important-Event-IDs.md
│   └── PowerShell-Logs.md
│
├── 06-Sysmon/
│   ├── Sysmon-Overview.md
│   ├── Sysmon-Event-IDs.md
│   └── Sysmon-Investigations.md
│
├── 07-Windows-Attacks/
│   ├── Credential-Attacks.md
│   ├── Privilege-Escalation.md
│   ├── Persistence.md
│   ├── PowerShell-Attacks.md
│   └── RDP-SMB-Attacks.md
│
├── 08-Investigations/
│   ├── Authentication-Investigation.md
│   ├── Process-Investigation.md
│   ├── PowerShell-Investigation.md
│   ├── Persistence-Investigation.md
│   └── Malware-Investigation.md
│
├── 09-TryHackMe/
│   ├── room-01.md
│   ├── room-02.md
│   └── ...
│
├── 10-Reports/
│   ├── Windows-Incident-Report-01.md
│   ├── Windows-Incident-Report-02.md
│   └── ...
│
└── screenshots/
```

---

## 📊 Investigation Documentation Format

Every investigation will document:

### Alert

What triggered the investigation?

### Host

Which Windows machine was involved?

### User

Which account was involved?

### Process

Which process executed?

### Parent Process

Which process launched it?

### Command Line

What command was executed?

### Network Activity

Was there an external connection?

### IOC

Were any suspicious:

* IP addresses
* Domains
* URLs
* Hashes
* Files

identified?

### Timeline

What happened first, second, and third?

### MITRE ATT&CK

Which tactic/technique may be relevant?

### Verdict

* Benign
* Suspicious
* Malicious
* Inconclusive

### Recommended Action

What should the SOC Analyst do next?

---

## 🧪 Example Investigation

```text
User receives suspicious document
        ↓
WINWORD.EXE starts
        ↓
PowerShell starts
        ↓
Suspicious command executed
        ↓
External network connection
        ↓
Suspicious executable downloaded
        ↓
Persistence created
```

The investigation will use Windows logs, process information, network evidence, and threat intelligence to determine whether the activity is malicious.

---

## 📚 Learning Sources

Primary learning sources will include:

* Microsoft Learn
* TryHackMe
* Official Windows documentation
* MITRE ATT&CK
* Security research and trusted cybersecurity resources
* Curated cybersecurity training videos

YouTube videos will be used selectively for difficult concepts and demonstrations.

---

## 🏆 Skills Demonstrated

By completing this project, I aim to demonstrate practical knowledge of:

* Windows Security
* Windows Administration
* Windows Event Logs
* Sysmon
* PowerShell
* Process Investigation
* Authentication Investigation
* Endpoint Monitoring
* Threat Detection
* IOC Analysis
* MITRE ATT&CK
* SOC Investigation
* Incident Documentation

---

## ⚠️ Disclaimer

All security testing and attack simulations in this repository are performed in authorized lab environments for educational and defensive cybersecurity purposes.

---

## 👨‍💻 Author

**Mahesh Najan**

Cybersecurity | SOC Analyst | VAPT

GitHub: https://github.com/maheshnajan

