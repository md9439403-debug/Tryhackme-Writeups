# Untitled

# Tryhackme

TryHackMe: Linux Shells

**Date:** 12-11-2026
**Room Link:** [https://tryhackme.com/room/linuxshells](https://tryhackme.com/room/linuxshells)

**Category:** Linux / Command Line & Scripting

---

## 🎯 Summary

Exploring how Linux shells act as an interface between the user and the operating system kernel, comparing different shell types (Bash, Sh, Zsh, Fish), and practicing shell scripting components like variables, loops, and conditional logic.

---

## 🔑 Key Concepts & Notes

1. **Linux Shell:** A command-line interpreter that translates user commands into instructions the Linux kernel can execute.
2. **Types of Shells:** Different shell environments offer unique features — e.g., `sh` (Bourne Shell), `bash` (Bourne Again Shell), `zsh` (Z Shell), and `fish` (Friendly Interactive Shell).
3. **Environment & Shell Variables:** Storing temporary or persistent session data (like `$SHELL`, `$PATH`, `$USER`) to control script and terminal behavior.
4. **Control Flow & Loops:** Using `if/else` conditions and `for`/`while` loops to automate repetitive tasks and logic inside shell scripts.

---

## 🛠️ Commands & Syntax Learned

| Command / Concept | Syntax / Example | Description  |
| --- | --- | --- |
| Check Current Shell | `echo $SHELL` or `echo $0` | Displays the active default shell path |
| List Available Shells | `cat /etc/shells` | Shows all valid login shells installed on the system |
| Switch Shell | `zsh` or `bash` | Temporarily switches to another installed shell |
| Shebang | `#!/bin/bash` | Specifies the interpreter used to execute the script |
| Execution Permission | `chmod +x script.sh` | Grants executable permissions to a shell script |
| For Loop | `for i in {1..5}; do echo $i; done` | Iterates over a range or list of items |
| Conditionals | `if [ "$var" == "val" ]; then ... fi` | Evaluates conditions to control script flow |
| Grep / Piping | `cat file.txt | grep "flag"` | Filters output streams to find specific patterns |

---

## 🚩 Flag / Lab Solution Notes

- **Task 1 (Introduction to Linux Shells):** Read the room overview regarding the role of shells in Linux systems.
- **Task 2 (How To Interact With a Shell?):**
    - Explored terminal interaction, command execution, standard input/output redirection (`>`, `>>`), and piping (`|`).
- **Task 3 (Types of Linux Shells):**
    - Checked active shells using `echo $SHELL` and inspected installed shells in `/etc/shells`.
    - Compared features of `sh`, `bash`, `zsh`, and `fish`.
- **Task 4 (Shell Scripting and Components):**
    - Reviewed core building blocks of shell scripts: Shebang (`#!/bin/bash`), variables, user input (`read`), loops, and conditionals.
- **Task 5 (The Locker Script):**
    - Analyzed and debugged a script implementing variables, user input prompts, and `if-elif-else` conditional authentication logic.
- **Task 6 (Practical Exercise):**
    - Applied shell commands, piping, and scripting logic to search through files and extract the hidden flag.
- **Task 7 (Conclusion):** Completed the Linux Shells room overview.

---

## 💡 What I Learned

- How different Linux shells (`bash`, `zsh`, `sh`, `fish`) operate and how to switch between them.
- Writing structured shell scripts using loops, conditional statements, and user input handling.
- Combining command-line utilities, piping, and scripting logic to automate tasks and solve practical challenges.