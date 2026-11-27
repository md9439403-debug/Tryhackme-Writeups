# TryHackme

# TryHackMe: Nmap: The Basics

**Date:** 27-11-2026
**Room Link:** [https://tryhackme.com/room/nmap](https://tryhackme.com/room/nmap)

**Category:** Networking / Network Scanning & Enumeration

---

## 🎯 Summary

Learning the fundamentals of Nmap (Network Mapper) to discover live hosts on a network, scan for open TCP and UDP ports, enumerate running service versions and OS details, control scan timing templates, and save scan results in multiple output formats.

---

## 🔑 Key Concepts & Notes

1. **Nmap (Network Mapper):** An industry-standard open-source utility for network discovery, port scanning, service enumeration, and security auditing.
2. **Host Discovery:** Identifying active hosts on a network using ping sweeps (`sn`), ARP scans, ICMP echo requests, or skipping host discovery (`Pn`) when firewalls block ping probes.
3. **Port Scanning Types:** Understanding TCP SYN (Stealth) scans (`sS`), TCP Connect scans (`sT`), and UDP scans (`sU`), as well as port states (`open`, `closed`, `filtered`).
4. **Service & OS Detection:** Probing open ports to fingerprint exact software versions (`sV`) and operating systems (`O`), or running aggressive enumeration (`A`).
5. **Timing & Output Control:** Adjusting scan speed via timing templates (`T0` to `T5`) to balance stealth vs. speed, and saving scan outputs in normal, XML, or grepable formats (`oN`, `oX`, `oG`, `oA`).

---

## 🛠️ Commands, Flags & Scan Types

| Flag / Scan Type | Syntax / Example | Description (কাজের বিবরণ) |
| --- | --- | --- |
| Ping Sweep (Host Discovery) | `nmap -sn 192.168.1.0/24` | Discovers live hosts on a subnet without performing a port scan |
| Skip Ping (No Discovery) | `nmap -Pn <IP>` | Treats target host as online and skips initial host discovery |
| TCP SYN (Stealth) Scan | `sudo nmap -sS <IP>` | Sends SYN packets without completing the 3-way handshake (fast & stealthy) |
| TCP Connect Scan | `nmap -sT <IP>` | Completes full TCP 3-way handshake (used when raw socket privileges aren't available) |
| UDP Scan | `sudo nmap -sU <IP>` | Scans open UDP ports (DNS, SNMP, DHCP) |
| Port Specification | `nmap -p 22,80,443 <IP>` / `-p-` | Scans specific ports, port ranges (`-p 1-1000`), or all 65,535 ports (`-p-`) |
| Service Version Detection | `nmap -sV <IP>` | Probes open ports to determine running service names and versions |
| OS & Aggressive Scan | `sudo nmap -O <IP>` / `-A` | Detects target OS (`-O`) or enables OS, version, script, and traceroute (`-A`) |
| Timing Templates | `nmap -T4 <IP>` | Controls scan speed from Paranoid (`-T0`) to Insane (`-T5`); `-T4` is standard for fast networks |
| Output Formats | `nmap -oN out.txt` / `-oA scan` | Saves results in Normal (`-oN`), XML (`-oX`), Grepable (`-oG`), or All formats (`-oA`) |

---

## 🚩 Flag / Lab Solution Notes

- **Task 1 (Introduction):** Read the room overview introducing Nmap for network reconnaissance.
- **Task 2 (Host Discovery: Who Is Online):**
    - Practiced scanning subnets with `sn` to identify live IP addresses and MAC vendors without port scanning.
- **Task 3 (Port Scanning: Who Is Listening):**
    - Compared TCP SYN (`sS`), TCP Connect (`sT`), and UDP (`sU`) scans, and practiced scanning all ports using `p-`.
- **Task 4 (Version Detection: Extract More Information):**
    - Used `sV` to enumerate exact service banners/versions and `O` / `A` to gather operating system details.
- **Task 5 (Timing: How Fast Is Fast):**
    - Explored timing templates (`T0` through `T5`) and rate-limiting flags (`-min-rate`) to optimize scan performance.
- **Task 6 (Output: Controlling What You See):**
    - Controlled verbosity (`v`, `vv`) and saved scan reports using `oN`, `oX`, `oG`, and `oA`.
- **Task 7 (Conclusion and Summary):** Completed the Nmap: The Basics room overview.

---

## 💡 What I Learned

- How to map active devices on a network using Nmap host discovery techniques.
- The differences between SYN, Connect, and UDP scans, and how to enumerate service versions (`sV`) and OS fingerprints (`O`).
- Balancing scan speed and stealth with timing templates (`T0`–`T5`) and exporting structured reports (`oN`, `oX`, `oG`, `oA`).