# Tryhackme

# TryHackMe: Windows Fundamentals Part 2

**Date:** 27-10-2026
**Room Link:** [https://tryhackme.com/room/windowsfundamentals2x0x](https://tryhackme.com/room/windowsfundamentals2x0x)

**Category:** Windows / Operating System Basics

---

## 🎯 Summary

Exploring advanced Windows system administration utilities, including System Configuration, UAC settings adjustment, Computer Management, System Information, Resource Monitor, Command Prompt basics, and Registry Editor.

---

## 🔑 Key Concepts & Notes

1. **System Configuration (`msconfig`):** A tool used to troubleshoot the Windows startup process, enable/disable services, and manage boot options.
2. **UAC Settings:** Adjusting User Account Control notification levels to balance system security and user convenience.
3. **Computer Management (`compmgmt.msc`):** A collection of administrative tools (Task Scheduler, Device Manager, Disk Management, Event Viewer, Services).
4. **Windows Registry (`regedit`):** A hierarchical database that stores low-level settings for the operating system and installed applications.

---

## 🛠️ Tools & System Components

| Component / Utility | Usage / Command | Description  |
| --- | --- | --- |
| System Configuration | `msconfig` | Configures startup options, system services, and boot flags |
| Change UAC Settings | `UserAccountControlSettings.exe` | Adjusts slider for security elevation notifications |
| Computer Management | `compmgmt.msc` | Central console for managing local services, disks, and events |
| System Information | `msinfo32` | Displays comprehensive hardware and OS software environment specs |
| Resource Monitor | `resmon` | Offers detailed real-time monitoring of CPU, Disk, Network, and Memory |
| Command Prompt | `cmd` | Command-line interface for executing system commands and scripts |
| Registry Editor | `regedit` | Hierarchical database editor for system configurations and keys |

---

## 🚩 Flag / Lab Solution Notes

- **Task 1 (Introduction):** Read the room overview regarding Windows Fundamentals Part 2.
- **Task 2 (System Configuration and Advanced System Settings):**
    - Used `msconfig` to view system boot configuration, services, and startup tools.
    - Explored Advanced System Settings for environment variables and performance options.
- **Task 3 (Change UAC Settings):**
    - Examined different UAC notification levels ranging from "Always Notify" to "Never Notify".
- **Task 4 (Computer Management):**
    - Explored tools inside `compmgmt.msc` including Event Viewer, Local Users and Groups, and Disk Management.
- **Task 5 (System Information):**
    - Ran `msinfo32` to inspect hardware resources, components, and software environment configuration.
- **Task 6 (Resource Monitor):**[
    - Used `resmon` to analyze process network connections, active disk read/write operations, and memory usage.
- **Task 7 (Command Prompt):**
    - Practiced basic utility commands inside the `cmd` terminal interface.
- **Task 8 (Registry Editor):**
    - Navigated through main hives like `HKEY_LOCAL_MACHINE` and `HKEY_CURRENT_USER` using `regedit`.
- **Task 9 (Conclusion):** Completed the Windows Fundamentals 2 module overview

---

## 💡 What I Learned

- How to inspect and edit system configuration hives using the Windows Registry Editor (`regedit`).
- Monitoring real-time hardware resources, network traffic, and disk activity via Resource Monitor (`resmon`).
- Utilizing built-in administrative utilities like `compmgmt.msc` and `msconfig` for OS management and security analysis.