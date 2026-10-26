# Tryhackme

# TryHackMe: Bash Scripting

**Date:** 25-10-2026
**Room Link:** [https://tryhackme.com/room/bashscripting](https://tryhackme.com/room/bashscripting)

**Category:** Scripting / Linux Basics

---

## 🎯 Summary

Learning the fundamentals of Bash scripting to automate repetitive tasks in Linux, use variables, accept positional parameters, manage arrays, and implement conditional logic.

---

## 🔑 Key Concepts & Notes

1. **Shebang (`#!/bin/bash`):** Placed at the very top of a script to tell the operating system to use the Bash interpreter.
2. **Variables:** Used to store data dynamically within a script (e.g., `NAME="User"`).
3. **Parameters (Arguments):** Command-line arguments passed into a script, accessed using `$1`, `$2`, `$@`, etc.
4. **Arrays:** Used to store multiple values in a single variable list.
5. **Conditionals (`if/else`):** Used to perform different actions based on whether a condition is true or false.

---

## 🛠️ Commands & Syntax Learned

| Command / Concept | Syntax / Example | Description  |
| --- | --- | --- |
| Shebang | `#!/bin/bash` | Defines script interpreter |
| Execution Permission | `chmod +x script.sh` | Makes the script executable |
| Run Script | `./script.sh` or `bash script.sh` | Executes the bash script |
| Variable Declaration | `NAME="Cyber"` | Assigns value to a variable |
| Use Variable | `echo $NAME` | Outputs the variable content |
| User Input | `read -p "Enter name: " variable` | Takes input from user |
| Positional Arguments | `$1`, `$2`, `$#` | Accesses arguments passed via terminal |
| Arrays | `cars=('Toyota' 'Honda')` | Declares an array of elements |
| Conditionals | `if [ $num -gt 10 ]; then ... fi` | Evaluates numeric or string comparisons |

---

## 🚩 Flag / Lab Solution Notes

- **Task 1 (Introduction):** Read the room overview regarding Bash scripting fundamentals.
- **Task 2 (Our first simple bash scripts):**[cite: 5]
    - Created a `.sh` file using `nano script.sh`.
    - Added `#!/bin/bash` at the top and used `echo` to output text.
    - Granted execution rights using `chmod +x script.sh` and ran it with `./script.sh`.
- **Task 3 (Variables):**[cite: 5]
    - Declared custom variables and referenced them using `$` notation.
    - Used `read` command to interactively capture user inputs.
- **Task 4 (Parameters):**[cite: 5]
    - Passed command-line arguments to the script (e.g., `./script.sh arg1 arg2`).
    - Accessed parameters using `$1` for first argument and `$#` for total argument count.
- **Task 5 (Arrays):**[cite: 5]
    - Created an array list and printed specific elements using `${array[0]}`.
    - Printed all elements using `${array[@]}`.
- **Task 6 (Conditionals):**[cite: 5]
    - Used `if`, `elif`, and `else` statements alongside operators like `eq`, `ne`, `gt`, `lt`.
    - Tested file existence using `if [ -f filename ]; then`.
- **Task 7 (Further reading):** Completed the room and reviewed resources for advanced automation[cite: 5].

---

## 💡 What I Learned

- How to write clean and executable Bash scripts for system automation.
- How to accept command-line input dynamically using parameters.
- Using array data structures and conditional checks to make decisions in Linux automation tasks.
