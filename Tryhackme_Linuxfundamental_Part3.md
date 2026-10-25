# Tryhackme

# 🐧 TryHackMe: Linux Fundamentals Part 3

**Date:** 25-10-2026
**Room Link:** [https://tryhackme.com/room/linuxfundamentalspart3](https://tryhackme.com/room/linuxfundamentalspart3)

**Category:** Linux / Advanced Basics

---

## 🎯 Summary

Learning advanced Linux utilities, managing terminal text editors, managing background/foreground processes, automation using cronjobs, managing software packages, and reviewing system logs.

---

## 🔑 Key Concepts & Notes

1. **Terminal Text Editors:** Editing files directly inside the command line using terminal-based editors like Nano or Vim.
2. **Processes:** Programs or tasks running on the Linux operating system, each assigned a unique Process ID (PID).
3. **Cron / Automation:** A time-based job scheduler in Linux used to run scripts or commands automatically at specified intervals.
4. **Package Management:** Installing, updating, and removing software packages using tools like `apt`.

---

## 🛠️ Commands Learned

| Command | Full Form / Meaning | Usage / Example | Description (কাজের বিবরণ) |
| --- | --- | --- | --- |
| `nano` | Nano Text Editor | `nano filename.txt` | Easy-to-use terminal text editor to edit files |
| `vim` | Vi Improved | `vim filename.txt` | Advanced modal text editor for the terminal |
| `wget` | Web Get | `wget <http://IP/file`> | Download files from the web via command line |
| `scp` | Secure Copy Protocol | `scp file.txt user@IP:/dir` | Securely transfer files between hosts over SSH |
| `ps` | Process Status | `ps aux` | Display information about active processes |
| `top` | Table of Processes | `top` | Real-time display of running system processes |
| `kill` | Kill Process | `kill -9 <PID>` | Terminate running processes by PID |
| `crontab` | Cron Table | `crontab -e` | Maintain and edit cron schedules for automation |
| `apt` | Advanced Package Tool | `sudo apt install <pkg>` | Command-line tool for handling software packages |

---

## 🚩 Flag / Lab Solution Notes

- **Task 1 (Introduction):** Read the room overview.
- **Task 2 (Deploy Your Linux Machine):** Started the target machine and established connection via SSH/In-Browser terminal.
- **Task 3 (Terminal Text Editors):**
    - Created and edited a text file using `nano`.
    - Practiced saving files using `Ctrl + O` and exiting with `Ctrl + X`.
- **Task 4 (General/Useful Utilities):**
    - Used `wget` to download remote files directly into the target machine.
    - Used python HTTP server and `scp` to move files across systems.
- **Task 5 (Processes 101):**
    - Ran `ps aux` to view all running processes.
    - Identified process IDs (PID) and killed unwanted process using `kill <PID>`.
- **Task 6 (Maintaining Your System: Automation):**
    - Inspected scheduled tasks located in `/etc/crontab` and edited user cronjobs with `crontab -e`.
- **Task 7 (Maintaining Your System: Package Management):**
    - Updated repository list using `sudo apt update`.
    - Installed missing packages using `sudo apt install`.
- **Task 8 (Maintaining Your System: Logs):**
    - Checked system log files located under `/var/log` (e.g., `/var/log/syslog`, `/var/log/auth.log`).
- **Task 9 (Conclusions & Summaries):** Completed the Linux Fundamentals module series!

---

## 💡 What I Learned

- How to edit files directly in the terminal without a GUI using `nano`.
- How to track, inspect, and kill system processes using `ps`, `top`, and `kill`.
- The basics of system automation via `crontab` and reviewing security logs in `/var/log`.