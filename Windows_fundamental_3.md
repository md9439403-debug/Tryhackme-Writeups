# Untitled

# Tryhackme

# TryHackMe: Windows Fundamentals Part 3

**Date:** 30-10-2026
**Room Link:** [https://tryhackme.com/room/windowsfundamentals3xzx](https://tryhackme.com/room/windowsfundamentals3xzx)

**Category:** Windows / Operating System Security

---

## 🎯 Summary

Learning about built-in Microsoft security features and tools designed to protect Windows devices, including Windows Updates, Windows Security, Virus & threat protection, Firewall & network protection, App & browser control, Device security, BitLocker drive encryption, and Volume Shadow Copy Service (VSS).

---

## 🔑 Key Concepts & Notes

1. **Windows Security:** A built-in centralized hub providing real-time protection against viruses, malware, and network threats.
2. **BitLocker:** A full-disk encryption feature included with Windows that protects data by encrypting entire volumes.
3. **Volume Shadow Copy Service (VSS):** A Windows service that creates backup copies or snapshots of computer files or volumes, even when they are in use.
4. **Windows Firewall:** Filters network traffic entering and leaving the system to block unauthorized access.

---

## 🛠️ Tools & Security Components

| Component / Utility | Usage / Command | Description  |
| --- | --- | --- |
| Windows Updates | Settings > Update & Security | Keeps OS patched against known vulnerabilities and security flaws |
| Virus & Threat Protection | Defender Antivirus | Performs real-time scans, quick scans, and updates threat definitions |
| Firewall & Network Protection | `wf.msc` | Controls network profiles (Domain, Private, Public) and rules |
| App & Browser Control | SmartScreen Filter | Protects against dangerous apps, files, sites, and downloads |
| BitLocker Drive Encryption | `manage-bde` / Control Panel | Encrypts drive volumes using AES to protect sensitive data |
| Volume Shadow Copy Service | `vssadmin` | Manages volume shadow copies used for system restore and backups |

---

## 🚩 Flag / Lab Solution Notes

- **Task 1 (Introduction):** Read the room overview regarding Windows security utilities[cite: 15].
- **Task 2 (Windows Updates):**[cite: 15]
    - Reviewed patch management and automatic update configurations.
- **Task 3 (Windows Security):**[cite: 15]
    - Navigated the Windows Security dashboard interface and health reports.
- **Task 4 (Virus & threat protection):**[cite: 15]
    - Examined Microsoft Defender options, real-time protection toggles, and exclusion settings.
- **Task 5 (Firewall & network protection):**[cite: 15]
    - Checked domain, private, and public network firewall rules and inbound/outbound traffic behaviors.
- **Task 6 (App & browser control):**[cite: 15]
    - Explored SmartScreen settings and exploit protection configurations.
- **Task 7 (Device security):**[cite: 15]
    - Checked hardware-level security features including Core Isolation and TPM (Trusted Platform Module).
- **Task 8 (BitLocker):**[cite: 15]
    - Explored BitLocker drive encryption setup, key recovery options, and volume locking mechanisms.
- **Task 9 (Volume Shadow Copy Service):**[cite: 15]
    - Inspected shadow copies created by Windows using `vssadmin` and learned its importance in recovery and forensics.
- **Task 10 (Conclusion):** Completed the Windows Fundamentals 3 module and finalized the Windows Fundamentals path[cite: 15].

---

## 💡 What I Learned

- How Windows Defender, SmartScreen, and Windows Firewall interact to form a multi-layered defense.
- Protecting data at rest using BitLocker full-disk encryption.
- The mechanics of Volume Shadow Copies (`vssadmin`) for system recovery and threat investigation.