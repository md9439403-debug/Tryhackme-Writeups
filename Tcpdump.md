# TryHackme

# TryHackMe: Tcpdump: The Basics

**Date:** 26-11-2026
**Room Link:** [https://tryhackme.com/room/tcpdump](https://tryhackme.com/room/tcpdump)

**Category:** Networking / CLI Packet Capture & Analysis

---

## 🎯 Summary

Learning the fundamentals of Tcpdump to capture live network traffic from the command line, save and read PCAP files, apply basic and advanced Berkeley Packet Filter (BPF) expressions, and customize packet output displays.

---

## 🔑 Key Concepts & Notes

1. **Tcpdump:** A lightweight, command-line packet analyzer used on Linux/Unix systems to intercept and display TCP/IP and other packets being transmitted or received over a network.
2. **Basic Packet Capture:** Specifying network interfaces (`i`), limiting captured packet counts (`c`), disabling name resolution (`n` / `nn`), saving captures to disk (`w`), and reading existing PCAP files (`r`).
3. **Filtering Expressions (BPF):** Using Berkeley Packet Filter syntax to isolate specific hosts, networks, ports, or protocols (`host`, `net`, `port`, `src`, `dst`).
4. **Advanced Filtering & Display Options:** Combining logical operators (`and`, `or`, `not`), inspecting TCP flags, and controlling verbosity (`v`, `vv`, `vvv`) or packet payload formats (`X`, `A`, `e`).

---

## 🛠️ Commands, Flags & Filters

| Flag / Filter | Syntax / Example | Description (কাজের বিবরণ) |
| --- | --- | --- |
| Select Interface | `tcpdump -i eth0` | Captures packets on a specific network interface (`any` for all) |
| Disable Resolution | `tcpdump -nn` | Prevents DNS and port name lookups for faster, raw numeric output |
| Limit Packet Count | `tcpdump -c 10` | Stops capturing automatically after receiving 10 packets |
| Write / Read PCAP | `tcpdump -w out.pcap` / `-r in.pcap` | Saves captured packets to a file or reads from an existing PCAP |
| Filter by Host / Net | `tcpdump host 192.168.1.10` | Isolates traffic to or from a specific IP address or subnet (`net`) |
| Filter by Port / Proto | `tcpdump tcp port 80` | Captures traffic matching a specific protocol and port number |
| Direction Filters | `src host <IP>` / `dst port 443` | Filters packets based on source (`src`) or destination (`dst`) |
| Display Payloads | `tcpdump -A` / `tcpdump -X` | Prints packet contents in ASCII (`-A`) or both Hex and ASCII (`-X`) |
| Verbosity & Headers | `tcpdump -vvv -e` | Shows maximum packet detail (`-vvv`) and link-layer Ethernet MAC headers (`-e`) |

---

## 🚩 Flag / Lab Solution Notes

- **Task 1 (Introduction):** Read the room overview introducing Tcpdump as a CLI packet capture utility.
- **Task 2 (Basic Packet Capture):**
    - Practiced selecting interfaces with `i`, limiting captures using `c`, and reading saved `.pcap` files with `r`.
    - Used `n` and `nn` flags to inspect raw IP addresses and port numbers without DNS resolution delays.
- **Task 3 (Filtering Expressions):**
    - Applied BPF expressions (`host`, `src`, `dst`, `port`, `icmp`, `tcp`, `udp`) to extract targeted traffic from PCAP files.
- **Task 4 (Advanced Filtering):**
    - Combined multiple filter conditions using logical operators (`and`, `or`, `not`) and inspected packet length/header filters to pinpoint specific anomalies.
- **Task 5 (Displaying Packets):**
    - Used `e` to view MAC addresses, `v`/`vvv` for deeper protocol inspection, and `A`/`X` to read cleartext payloads and locate hidden flags.
- **Task 6 (Conclusion):** Completed the Tcpdump: The Basics room overview.

---

## 💡 What I Learned

- How to capture, save, and inspect network packets directly from a Linux terminal without needing a GUI.
- Writing precise Berkeley Packet Filter (BPF) expressions to isolate specific hosts, ports, and protocols.
- Customizing Tcpdump verbosity and payload display modes (`A`, `X`, `e`, `nn`) to analyze headers and uncover cleartext data.