# Tryhackme

# TryHackMe: Networking Core Protocols

**Date:** 22-11-2026
**Room Link:** [https://tryhackme.com/room/networkingcoreprotocols](https://tryhackme.com/room/networkingcoreprotocols)

**Category:** Networking / Application Layer Protocols

---

## 🎯 Summary

Exploring the core TCP/IP application-layer protocols that drive everyday internet usage, including domain resolution via DNS, domain registration lookups with WHOIS, web communication over HTTP(S), file transfers via FTP, and email protocols (SMTP, POP3, and IMAP).

---

## 🔑 Key Concepts & Notes

1. **DNS (Domain Name System):** Translates human-readable domain names (like `tryhackme.com`) into machine-readable IP addresses using hierarchical DNS servers and record types (`A`, `AAAA`, `CNAME`, `MX`, `TXT`).
2. **WHOIS:** A query and response protocol used for querying databases that store registered users or assignees of an Internet resource, such as a domain name or an IP address block.
3. **HTTP(S) (Hypertext Transfer Protocol Secure):** The foundational protocol for transmitting web pages and data over the internet, with HTTPS adding TLS encryption for confidentiality and integrity.
4. **FTP (File Transfer Protocol):** A standard network protocol used for transferring files between a client and a server over a TCP connection (Port 21 for control, Port 20 for data).
5. **Email Protocols (SMTP, POP3, IMAP):** SMTP handles sending/routing emails, POP3 downloads emails locally (typically removing them from the server), and IMAP synchronizes emails across multiple devices while keeping them on the server.

---

## 🛠️ Protocols, Ports & Utilities

| Protocol / Tool | Default Port(s) / Example | Description (কাজের বিবরণ) |
| --- | --- | --- |
| DNS | Port `53` (`nslookup`, `dig`) | Resolves domain names to IP addresses via A, MX, and TXT records |
| WHOIS | Port `43` (`whois example.com`) | Retrieves domain ownership, registrar, and registration date details |
| HTTP / HTTPS | Port `80` / `443` (`curl`) | Transfers web resources; HTTPS encrypts traffic using TLS |
| FTP | Port `20` (Data) & `21` (Control) | Transfers files between remote hosts (`ftp <IP>`) |
| SMTP | Port `25`, `465`, `587` | Pushes and relays outgoing emails between mail servers |
| POP3 | Port `110` / `995` (SSL) | Downloads email messages from a mail server to a single local client |
| IMAP | Port `143` / `993` (SSL) | Syncs and manages emails directly on the mail server across multiple devices |

---

## 🚩 Flag / Lab Solution Notes

- **Task 1 (Introduction):** Read the room overview introducing core TCP/IP application protocols.
- **Task 2 (DNS: Remembering Addresses):**
    - Explored DNS hierarchy (Root, TLD, Authoritative servers) and queried records (`A`, `AAAA`, `CNAME`, `MX`, `TXT`) using tools like `nslookup` and `dig`.
- **Task 3 (WHOIS):**
    - Ran `whois` lookups to inspect domain registration details, registrant info, and name servers.
- **Task 4 (HTTP(S): Accessing the Web):**
    - Examined HTTP request methods (`GET`, `POST`), status codes (`200`, `301`, `404`), headers, and how HTTPS secures web traffic.
- **Task 5 (FTP: Transferring Files):**
    - Practiced connecting to an FTP server, navigating remote directories, and downloading files using basic FTP commands (`ls`, `get`).
- **Task 6 (SMTP: Sending Email):**
    - Reviewed how SMTP pushes mail from client to server and relays messages between mail transfer agents.
- **Task 7 (POP3: Receiving Email):**
    - Understood how POP3 retrieves messages from a mail server and stores them locally.
- **Task 8 (IMAP: Synchronizing Email):**
    - Compared IMAP with POP3, focusing on multi-device folder synchronization and server-side storage.
- **Task 9 (Conclusion):** Completed the Networking Core Protocols room overview.

---

## 💡 What I Learned

- How DNS resolves domain names and how `whois` provides valuable OSINT on domain registrations.
- The mechanics of web communication via HTTP(S) and cleartext file transfers using FTP.
- The distinct roles and default ports of email protocols (`SMTP` for sending, `POP3` for downloading, and `IMAP` for syncing).

---