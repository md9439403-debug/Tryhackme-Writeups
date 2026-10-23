
# 🐧 TryHackMe: Linux Fundamentals Part 1

**Date:** 21-10-2026
**Room Link:** [https://tryhackme.com/room/linuxfundpart1](https://tryhackme.com/room/linuxfundpart1)**Category:** Linux / Basics

---

## 🎯 Summary

Getting familiar with the Linux operating system, learning basic terminal commands, and navigating through the file system.

---

## 🔑 Key Concepts & Notes

1. **Linux System:** Linux is an open-source operating system. It is available in various distributions (such as Ubuntu, Kali, and Debian).
2. **Terminal:** A means of controlling the Linux system via the command line.
3. **Shell:** A medium that accepts user commands and relays them to the operating system (e.g., Bash).

---

## 🛠️ Commands Learned

| Command | Full Form / Meaning | Usage / Example | Description (কাজের বিবরণ) |
| --- | --- | --- | --- |
| `echo` | Echo | `echo "Hello"` | Display line of text |
| `whoami` | Who am I | `whoami` | Print effective user name |
| `ls` | List | `ls` or `ls -la` | List directory content |
| `cd` | Change Directory | `cd /var/www` | To move from one folder to another folder |
| `pwd` | Print Working Directory | `pwd` | To print current working directory |
| `cat` | Concatenate | `cat flag.txt` | concatenate files and print on standard output |
| `find` | Find | `find -name flag.txt` | Search for files in a directory hierarchy |
| `grep` | **Global Regular Expression Print** | `grep "password123" passwords.txt` | print lines that match patterns |

---

## 🚩 Flag / Lab Solution Notes

- **Task 1 :**  What is Linux and where is it  used ?
- **Task 2 (Interacting with the System):**
    - I ran `whoami` and  found the username :  `tryhackme`
    - I ran `echo “Hello world”` and printed the text
- Task 3 :
    - I ran `ls` to see what is my home folder .
    - I used `cd` to change the folder.
    - I used `cat` to output the content of any files .
    - I used `pwd` to see where I am within the system .
    - Command to read the flag : `cat passwords.txt`
    - The flag is password123
- **Task 5 :**
    - I used `find -name passwords.txt` to search for a file by its name.
    - I ran `cd /home/tryhackme` to return my home folder.
    - I ran `grep "THM" access.log` to search the log file with grep. Then I found the flag `THM{ACCESS}`

---

## 💡 What I Learned

- How powerful the grep and find commands are when searching  for files .
- The difference between a relative path and absolute path.
