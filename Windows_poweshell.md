# Tryhackme

# TryHackMe: Windows PowerShell

**Date:** 10-11-2026
**Room Link:** [https://tryhackme.com/room/windowspowershell](https://tryhackme.com/room/windowspowershell)

**Category:** Windows / Command Line & Automation

---

## 🎯 Summary

Exploring the core fundamentals of Windows PowerShell, including cmdlet architecture, navigation, pipeline filtering and sorting, real-time system/network analysis, and basic scripting.

---

## 🔑 Key Concepts & Notes

1. **PowerShell Architecture:** An object-oriented command-line shell and scripting language built on the .NET framework using standard `Verb-Noun` cmdlets.
2. **Object Pipeline:** Passing whole structured objects between cmdlets using the `|` operator rather than plain raw text strings.
3. **Filtering & Sorting:** Utilizing `Where-Object` and `Sort-Object` to parse and extract relevant log data or system processes.
4. **Automation & Scripting:** Writing executable `.ps1` scripts using loops, variables, and execution policies.

---

## 🛠️ Cmdlets & System Components

| Cmdlet / Utility | Usage / Example | Description  |
| --- | --- | --- |
| `Get-Help` | `Get-Help Get-Process -Detailed` | Displays detailed usage and help documentation for any cmdlet |
| `Get-Command` | `Get-Command *service*` | Lists available cmdlets matching specified search terms |
| `Get-ChildItem` | `Get-ChildItem -Path C:\ -Recurse` | Navigates and lists files/directories (similar to `ls` or `dir`) |
| `Where-Object` | `Get-Process | Where-Object`  | Filters pipeline objects based on evaluation criteria |
| `Sort-Object` | `Get-Process | Sort-Object CPU -Descending` | Sorts output objects alphabetically or numerically |
| `Get-NetIPAddress` | `Get-NetIPAddress -AddressFamily IPv4` | Retrieves detailed network IP address configurations |
| `Get-Process` | `Get-Process | Select-Object -First 10` | Obtains real-time status of running background processes |
| `Set-ExecutionPolicy` | `Set-ExecutionPolicy RemoteSigned` | Manages permissions for executing custom `.ps1` PowerShell scripts |

---

## 🚩 Flag / Lab Solution Notes

- **Task 1 (Introduction):** Read the room overview regarding Windows PowerShell capability and features.
- **Task 2 (What Is PowerShell):**
    - Examined the difference between traditional CMD text outputs and PowerShell object-oriented pipelines.
- **Task 3 (PowerShell Basics):**
    - Practiced retrieving cmdlet structures using `Get-Command` and reading help manuals with `Get-Help`.
- **Task 4 (Navigating the File System and Working with Files):**
    - Used `Get-ChildItem` (alias `dir`/`ls`), `Set-Location` (alias `cd`), and file creation cmdlets (`New-Item`, `Get-Content`).
- **Task 5 (Piping, Filtering, and Sorting Data):**
    - Piped pipeline output into `Where-Object` and `Sort-Object` to extract specific process parameters.
- **Task 6 (System and Network Information):**
    - Evaluated network properties and hardware profiles using `Get-NetIPAddress`, `Get-NetTCPConnection`, and `Get-HotFix`.
- **Task 7 (Real-Time System Analysis):**
    - Performed real-time tracking of process CPU usage, service status (`Get-Service`), and event logs (`Get-EventLog`).
- **Task 8 (Scripting):**
    - Created a basic `.ps1` script, set execution policy limits via `Set-ExecutionPolicy`, and ran it in PowerShell.
- **Task 9 (Conclusion):** Completed the Windows PowerShell fundamental module overview.

---

## 💡 What I Learned

- How `Verb-Noun` structured cmdlets and object-oriented pipelines make data manipulation far more powerful than traditional text parsing.
- Filtering system logs, network sockets, and running services in real-time using `Where-Object` and `Select-Object`.
- Fundamentals of PowerShell scripting, Execution Policies, and administrative system analysis.