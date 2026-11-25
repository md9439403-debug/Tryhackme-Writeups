# TryHackme

# TryHackMe: Wireshark: The Basics

**Date:** 25-11-2026
**Room Link:** [https://tryhackme.com/room/wiresharkthebasics](https://tryhackme.com/room/wiresharkthebasics)

**Category:** Networking / Packet Analysis & Traffic Inspection

---

## 🎯 Summary

Learning the fundamentals of Wireshark to capture, inspect, dissect, navigate, and filter network traffic and PCAP files for protocol analysis and security investigations.

---

## 🔑 Key Concepts & Notes

1. **Wireshark:** An open-source packet analyzer used for network troubleshooting, protocol analysis, and inspecting captured network traffic (`.pcap` / `.pcapng`).
2. **Packet Dissection:** Breaking down captured network packets layer by layer (Frame, Ethernet, IPv4/IPv6, TCP/UDP, Application Layer) to inspect headers and payloads.
3. **Packet Navigation:** Moving efficiently through large capture files using packet numbers, timestamps, Go To Packet (`Ctrl + G`), Find Packet (`Ctrl + F`), and following TCP/UDP/HTTP streams.
4. **Packet Filtering:** Narrowing down traffic using **Capture Filters** (applied before capturing) and **Display Filters** (applied on already captured packets to isolate specific protocols, IPs, or ports).

---

## 🛠️ Filters, Features & Shortcuts

| Feature / Filter | Syntax / Shortcut | Description (কাজের বিবরণ) |
| --- | --- | --- |
| Find Packet | `Ctrl + F` | Searches for specific strings, hex values, or packet details inside a PCAP |
| Go To Packet | `Ctrl + G` | Jumps directly to a specific packet frame number |
| Follow Stream | Right-click → Follow → TCP/HTTP Stream | Reconstructs full human-readable conversations between client and server |
| Filter by IP | `ip.addr == 192.168.1.10` | Displays packets where the source or destination IP matches |
| Filter by Protocol | `http` / `dns` / `tcp` / `icmp` | Isolates traffic belonging to a specific network protocol |
| Filter by Port | `tcp.port == 80` | Filters TCP traffic communicating over a specific port |
| Logical Operators | `and` (`&&`), `or` (`||`), `not` (`!`) | Combines multiple display filter conditions for precise traffic isolation |

---

## 🚩 Flag / Lab Solution Notes

- **Task 1 (Introduction):** Read the room overview introducing Wireshark and PCAP analysis.
- **Task 2 (Tool Overview):**
    - Explored the Wireshark GUI layout: Packet List Pane, Packet Details Pane, and Packet Bytes Pane.
    - Checked capture file statistics, protocol hierarchy, and resolved addresses.
- **Task 3 (Packet Dissection):**
    - Inspected individual packet layers from physical frame metadata up to application-layer payloads.
    - Analyzed Ethernet MAC addresses, IP headers, TCP flags, and HTTP request/response structures.
- **Task 4 (Packet Navigation):**
    - Practiced locating specific packets using `Ctrl + F` (Find Packet) and `Ctrl + G` (Go To Packet).
    - Used **Follow TCP/HTTP Stream** to reconstruct cleartext communications and extract hidden flags.
- **Task 5 (Packet Filtering):**
    - Applied display filters (`ip.addr`, `tcp.port`, `http.request`, etc.) to isolate suspicious traffic from noisy captures.
- **Task 6 (Conclusion):** Completed the Wireshark: The Basics room overview.

---

## 💡 What I Learned

- How to navigate the three core panes of Wireshark to dissect packets across OSI layers.
- Reconstructing full client-server conversations using Follow Stream and locating artifacts with packet search tools.
- Writing accurate display filters to isolate specific IPs, ports, and protocols during traffic analysis.