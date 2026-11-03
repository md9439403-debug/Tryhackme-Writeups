# Tryhackme

TryHackMe: Windows Command Line

**Date:** 03-11-2026
**Room Link:** [https://tryhackme.com/room/windowscommandline](https://tryhackme.com/room/windowscommandline)

**Category:** Windows / Command Line & System Utilities

---

## 🎯 Summary

Learning the essential Windows command-line utilities for system information retrieval, network troubleshooting, file and disk management, as well as task and process management via CMD.

---

## 🔑 Key Concepts & Notes

1. **Command Prompt (CMD):** The default command-line interpreter for Windows operating systems used to execute administrative commands and scripts.
2. **System Information Utilities:** Built-in commands like `systeminfo` and `hostname` used to gather hardware, OS, and computer identity data.
3. **Network Troubleshooting Tools:** Essential tools (`ipconfig`, `ping`, `tracert`, `netstat`) used to diagnose connectivity issues and inspect network interfaces.
4. **Process & Service Management:** Utilizing CLI commands like `tasklist` and `taskkill` to monitor and terminate active system processes.

---

## 🛠️ Commands & System Utilities

| Command | Usage / Example | Description  |
| --- | --- | --- |
| `hostname` | `hostname` | Displays the current computer name |
| `systeminfo` | `systeminfo` | Fetches detailed system hardware, OS version, and patch details |
| `ipconfig` | `ipconfig /all` | Displays network interface configurations, IP addresses, and DNS details |
| `ping` | `ping 8.8.8.8` | Checks network connectivity between hosts |
| `tracert` | `tracert tryhackme.com` | Traces the path/route packets take to reach a destination host |
| `netstat` | `netstat -ano` | Displays active network connections, listening ports, and associated PIDs |
| `dir` | `dir /a` | Lists directory files and folders (including hidden files) |
| `tree` | `tree /F` | Graphically displays the directory structure of a path or drive |
| `tasklist` | `tasklist` | Displays all currently running processes and their PIDs |
| `taskkill` | `taskkill /PID <pid> /F` | Forcefully terminates a running process by its Process ID |

---

## 🚩 Flag / Lab Solution Notes

- **Task 1 (Introduction):** Read the room overview regarding Windows Command Line tools.
- **Task 2 (Basic System Information)**
    - Used `hostname` to display the machine name.
    - Executed `systeminfo` to inspect OS configuration, hotfixes, and system architecture.
- **Task 3 (Network Troubleshooting):**
    - Used `ipconfig` to verify network interface settings and default gateway IPs.
    - Practiced testing host reachability with `ping` and tracing routing hops using `tracert`.
    - Inspected listening ports and network sockets with `netstat`.
- **Task 4 (File and Disk Management):**
    - Navigated directories using `cd` and listed contents with `dir`.
    - Viewed file structures using `tree` and checked file attributes/permissions.
- **Task 5 (Task and Process Management):**
    - Listed running background processes using `tasklist`.
    - Identified process IDs (PIDs) and practiced killing unwanted tasks using `taskkill`.
- **Task 6 (Conclusion):** Completed the Windows Command Line module overview.

---

## 💡 What I Learned

- How to quickly gather host and OS information using native CLI utilities (`systeminfo`, `hostname`).
- Diagnosing network issues and port activity directly through `ipconfig`, `tracert`, and `netstat`.
- Managing disk files, viewing directory trees, and handling active system processes via `tasklist` and `taskkill`.