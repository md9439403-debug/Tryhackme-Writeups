# Tryhackme

# 🐧 TryHackMe: Linux Fundamentals Part 2

**Date:** 24-10-2026
**Room Link:** [https://tryhackme.com/room/linuxfundpart2](https://tryhackme.com/room/linuxfundpart2)

**Category:** Linux / Basics

---

## 🎯 Summary

Learning about file permissions, operator symbols, common directories and how to access Linux using SSH.

---

## 🔑 Key Concepts & Notes

1. **Access Control (Permissions):** Linux uses user, group, and others permissions with Read (r), Write (w), and Execute (x) access.
2. **SSH (Secure Shell):** Used to securely connect and manage a remote Linux system over a network.
3. Common directories: The root file system 

---

## 🛠️ Commands Learned

| Command | Full Form / Meaning | Usage / Example | Description  |
| --- | --- | --- | --- |
| `ssh` | Secure shell | `ssh tryhackme@10.80.184.24` | Open securely remote access |
| `ping` | Packet internet groper | `ping -c` | Send ICMP ECHO_REQUEST to network hosts
 |
| `ls` | List | `ls-a`  and `ls -lh` | Show list directory content |
| `man` | Manual | `man ls` | Manual of content |
| `touch` | — | `touch recipe.txt` | Create file |
| `mkdir` | Make directory | `mkdir myfile` | Makes directory |
| `cp` | Copy | `cp racipe racipe2` | Copy one file to another file |
| `mv`  | Move | `mv racipe racipe2` | Move  one file to another file |
| `rm` | Remove | `rm - R mydirectory` | Remove files |
| `su` | Switch user | `su user2` | Switch one user to  another user |

---

## 🚩 Flag / Lab Solution Notes

- **Task 1 :**
    - Connected to the target machine using: `ssh machine_ip` with the provided credentials.
- **Task 2 :**
    - I used `ls - a` to  found hidden folder .
    - I used `man ls` to read manual of ls command .
    - I used `ls -lh` to saw much more details of file and directories.
- **Task 3:**
    - I used `touch recipe.txt` to create text file.
    - I used `mkdir Myfile` to create a directory .
    - I used `rm -R Myfile` to remove directory .
    - I used `cp recipe recipe2` to copy recipe file to recipe2 .
    - I used `mv myfile` Jihad to move file .
    - I ran `cp note Ducuments` to the flag `THM{COPY_Master}`.
- **Task 4 :**
    - I’m learned the Linux root file system . Exp.  /etc , /var , /root , /tmp .
- **Task 5 :**
    - I’m learned file and group permissions.
    - I ran `su user2`  to switch the user.

---

## 💡 What I Learned

- How file permissions (Read, Write, Execute) protect Linux systems from unauthorized access.
- How to connect and manage remote servers securely using SSH.
