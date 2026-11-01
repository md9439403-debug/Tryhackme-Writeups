# Untitled

# Tryhackme

# TryHackMe: Active Directory Basics

**Date:** 01-11-2026
**Room Link:** [https://tryhackme.com/room/winadbasics](https://tryhackme.com/room/winadbasics)

**Category:** Windows / Active Directory Basics

---

## 🎯 Summary

Learning the core concepts and fundamental functionality provided by Active Directory (AD), including Windows Domains, Domain Controllers, AD user and computer object management, Group Policy Objects (GPOs), authentication protocols, and AD infrastructure hierarchy (Trees, Forests, and Trusts).

---

## 🔑 Key Concepts & Notes

1. **Active Directory (AD):** A directory service developed by Microsoft for Windows domain networks to centralize identity and access management.
2. **Domain Controller (DC):** A server running Active Directory Domain Services (AD DS) that responds to security authentication requests and controls domain access.
3. **Group Policy Objects (GPO):** A feature of Active Directory that allows administrators to manage operating system environments, security settings, and software for users and computers across a domain.
4. **Trees, Forests & Trusts:** Structural components of AD where Trees group related domains, Forests group multiple trees, and Trusts define access relationships between domains.

---

## 🛠️ Components & Administration Utilities

| Component / Utility | Management Tool / Concept | Description |
| --- | --- | --- |
| Domain Controller (DC) | Active Directory Domain Services (AD DS) | Central server validating user credentials and enforcing security policies |
| Active Directory Users & Computers | `dsa.msc` | GUI console used to manage users, groups, Organizational Units (OUs), and machines |
| Group Policy Management | `gpmc.msc` | Centralized management of system, security, and script policies applied to domain devices |
| Kerberos / NTLM | Authentication Protocols | Security protocols used to verify identities and enable single sign-on (SSO) |
| Organizational Units (OU) | Logical Containers | Containers within a domain used to organize objects and scope Group Policies |

---

## 🚩 Flag / Lab Solution Notes

- **Task 1 (Introduction):** Read the room overview introducing Active Directory architecture and usage.
- **Task 2 (Windows Domains):**
    - Understood domain concepts, central authority management, and client-server network models.
- **Task 3 (Active Directory):**
    - Explored the core roles of Active Directory Domain Services (AD DS) and central database functionality.
- **Task 4 (Managing Users in AD):**
    - Practiced viewing, creating, and modifying user accounts, administrative rights, and user attributes using `dsa.msc`.
- **Task 5 (Managing Computers in AD):**
    - Examined domain-joined computer objects and machine account properties.
- **Task 6 (Group Policies):**
    - Explored GPO deployment, policy linking to OUs, and setting enforcement across domain machines.
- **Task 7 (Authentication Methods):**
    - Reviewed authentication mechanisms such as Kerberos tickets (TGT/TGS) and legacy NTLM challenge-response.
- **Task 8 (Trees, Forests and Trusts):**
    - Analyzed forest root domains, child domains, and transitive/non-transitive trust relationships.
- **Task 9 (Conclusion):** Completed the Active Directory Basics room overview.

---

## 💡 What I Learned

- The architecture of Active Directory and how Domain Controllers manage enterprise authentication.
- How to manage users, computers, and Organizational Units (OUs) using AD management utilities.
- How Group Policies (GPOs) enforce security configurations and how Kerberos powers domain authentication.