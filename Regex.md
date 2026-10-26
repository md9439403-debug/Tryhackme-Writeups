# Tryhackme

# TryHackMe: Regular Expressions

**Date:** 25-10-2026
**Room Link:** [https://tryhackme.com/room/catregex](https://tryhackme.com/room/catregex)

**Category:** Linux / Text Processing & Regex

---

## 🎯 Summary

Learning the fundamentals of Regular Expressions (Regex) to match patterns, search specific text strings, handle wildcards, use character sets, metacharacters, and apply logical operators in log analysis and security tasks.

---

## 🔑 Key Concepts & Notes

1. **Regular Expressions (Regex):** A sequence of characters that specifies a search pattern in text.
2. **Character Sets (`[...]`):** Used to match any single character contained within square brackets.
3. **Wildcards (`.`):** Matches any single character except newline characters.
4. **Metacharacters & Repetitions (, `+`, `{n,m}`):** Used to control how many times a character or group should be repeated.
5. **Anchors (`^`, `$`):** Spells out where matching should start (`^` for line start) or end (`$` for line end).

---

## 🛠️ Syntax & Symbols Learned

| Symbol / Concept | Syntax / Example | Description  |
| --- | --- | --- |
| Character Set | `[a-z]`, `[0-9]` | Matches any lowercase letter or digit |
| Negated Set | `[^abc]` | Matches any character except a, b, or c |
| Wildcard | `c.t` | Matches cat, cot, cut, etc. |
| Optional | `colou?r` | The `?` makes the preceding character optional |
| Kleene Star | `a*` | Matches zero or more occurrences of 'a' |
| Plus Operator | `a+` | Matches one or more occurrences of 'a' |
| Repetitions | `a{2,4}` | Matches 'a' between 2 to 4 times |
| Line Start / End | `^admin`, `end$` | Matches pattern at start (`^`) or end (`$`) of line |
| Alternation / Or | `(cat|dog)` | Matches either 'cat' or 'dog' |

---

## 🚩 Flag / Lab Solution Notes

- **Task 1 (Introduction):** Read the room overview regarding Regular Expressions fundamentals[cite: 7].
- **Task 2 (Charsets):**[cite: 7]
    - Learned how to construct basic character sets using `[a-z]`, `[A-Z]`, and `[0-9]`.
    - Practiced matching specific characters or ranges of characters.
- **Task 3 (Wildcards and optional characters):**[cite: 7]
    - Used the dot (`.`) wildcard to match arbitrary single characters.
    - Applied the question mark (`?`) to specify optional preceding characters.
- **Task 4 (Metacharacters and repetitions):**[cite: 7]
    - Used  for zero-or-more matches and `+` for one-or-more matches.
    - Utilized curly braces `{}` to set exact minimum and maximum repetition limits.
- **Task 5 (Starts with/ ends with, groups, and either/ or):**[cite: 7]
    - Used caret (`^`) and dollar (`$`) anchors to pin search patterns to line boundaries.
    - Applied parentheses `()` for grouping expressions and pipe (`|`) for OR logical operations.
- **Task 6 (Conclusion):** Completed the Regular Expressions room and reviewed practical CLI usage with tools like `grep`[cite: 7].

---

## 💡 What I Learned

- How to build flexible text matching patterns using Regex syntax.
- Efficiently parsing and filtering log files using anchors, character sets, and repetition flags.
- Combining regex patterns with security utilities like `grep` for log analysis and VAPT tasks.