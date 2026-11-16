# Untitled

# Tryhackme

# TryHackMe: Networking Concepts

**Date:** 16-11-2026
**Room Link:** [https://tryhackme.com/room/networkingconcepts](https://tryhackme.com/room/networkingconcepts)

**Category:** Networking / Core Fundamentals

---

## 🎯 Summary

Learning the fundamental networking architectures and protocols, including the ISO OSI model, TCP/IP protocol suite, IP addressing and subnetting, TCP vs. UDP transport protocols, data encapsulation, and remote connections via Telnet.

---

## 🔑 Key Concepts & Notes

1. **ISO OSI Model:** A 7-layer conceptual framework (Physical, Data Link, Network, Transport, Session, Presentation, Application) standardizing network communication functions.
2. **TCP/IP Model:** A 4-layer practical networking suite (Link, Internet, Transport, Application) that powers modern internet communications.
3. **IP Addresses & Subnets:** Logical numerical labels (IPv4/IPv6) assigned to devices, alongside Subnet Masks used to divide networks into smaller, manageable sub-networks.
4. **TCP vs. UDP:** TCP is connection-oriented and reliable (uses a 3-way handshake), whereas UDP is connectionless, faster, and lightweight without delivery guarantees.
5. **Encapsulation:** The process of wrapping data with protocol headers (and trailers) as it moves down through the network layers before transmission.

---

## 🛠️ Protocols, Layers & Utilities

| Concept / Tool | Layer / Example | Description  |
| --- | --- | --- |
| OSI Model | 7 Layers (L1–L7) | Conceptual standard for how data travels across a network |
| TCP/IP Suite | 4 Layers | Core protocol stack governing internet data routing and delivery |
| IPv4 & Subnetting | `192.168.1.0/24` | Identifies host and network portions of an IP address using CIDR/subnet masks |
| TCP Handshake | `SYN` → `SYN-ACK` → `ACK` | Establishes a reliable, ordered connection before transmitting data |
| UDP | Connectionless Transport | Low-latency protocol used for streaming, DNS, and VoIP |
| Encapsulation | Data → Segment → Packet → Frame → Bits | Adds layer-specific headers as data moves down the stack |
| Telnet | `telnet <IP> <port>` | Cleartext network protocol used for remote terminal access and banner grabbing |

---

## 🚩 Flag / Lab Solution Notes

- **Task 1 (Introduction):** Read the room overview introducing foundational networking concepts.
- **Task 2 (OSI Model):**
    - Reviewed all 7 layers of the ISO OSI model and their respective responsibilities (from Physical bits up to Application protocols).
- **Task 3 (TCP/IP Model):**
    - Mapped the 4 layers of the TCP/IP suite to their corresponding OSI layers.
- **Task 4 (IP Addresses and Subnets):**
    - Practiced identifying network IDs, host ranges, broadcast addresses, and subnet masks using CIDR notation.
- **Task 5 (UDP and TCP):**
    - Compared reliability, overhead, and use cases of TCP (3-way handshake) and UDP.
- **Task 6 (Encapsulation):**
    - Traced how Protocol Data Units (PDUs) transform across layers (Data, Segment, Packet, Frame, Bits).
- **Task 7 (Telnet):**
    - Used `telnet` from the terminal to connect to a remote service over an open port, interact with it in cleartext, and retrieve the flag.
- **Task 8 (Conclusion):** Completed the Networking Concepts room overview.

---

## 💡 What I Learned

- How the 7-layer OSI model and 4-layer TCP/IP suite structure end-to-end network communication.
- Calculating subnets, distinguishing TCP from UDP, and understanding how data encapsulation works across layers.
- Using `telnet` to interact with network services over raw ports and understanding why cleartext protocols pose security risks.