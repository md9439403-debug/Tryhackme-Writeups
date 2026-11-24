# TryHackme

# TryHackMe: Networking Secure Protocols

**Date:** 24-11-2026
**Room Link:** [https://tryhackme.com/room/networkingsecureprotocols](https://tryhackme.com/room/networkingsecureprotocols)

**Category:** Networking / Network Security & Encryption

---

## 🎯 Summary

Exploring how cryptographic protocols secure network traffic against eavesdropping and tampering, covering TLS encryption, HTTPS web security, encrypted email protocols (SMTPS, POP3S, IMAPS), secure remote access via SSH, encrypted file transfers (SFTP and FTPS), and Virtual Private Networks (VPNs).

---

## 🔑 Key Concepts & Notes

1. **TLS (Transport Layer Security):** A cryptographic protocol designed to provide end-to-end communications security over a network using asymmetric key exchange, symmetric encryption, and digital certificates.
2. **HTTPS:** HTTP layered over TLS (`Port 443`) to ensure confidentiality, integrity, and server authentication during web browsing.
3. **Secure Email Protocols (SMTPS, POP3S, IMAPS):** Standard email protocols wrapped in TLS encryption to protect credentials and message contents from cleartext interception.
4. **SSH (Secure Shell):** A cryptographic network protocol (`Port 22`) for operating network services securely over an unsecured network, replacing legacy cleartext protocols like Telnet.
5. **SFTP vs. FTPS:** SFTP runs over an encrypted SSH channel (`Port 22`), whereas FTPS adds TLS/SSL encryption directly onto traditional FTP (`Port 21` / `990`).
6. **VPN (Virtual Private Network):** Extends a private network across a public network by creating an encrypted tunnel to protect data in transit and mask client IP addresses.

---

## 🛠️ Protocols, Ports & Utilities

| Protocol / Tool | Default Port(s) / Example | Description (কাজের বিবরণ) |
| --- | --- | --- |
| TLS | Handshake & Symmetric Encryption | Secures data in transit and verifies server identity via CA certificates |
| HTTPS | Port `443` (`curl https://...`) | Encrypts HTTP traffic using TLS to prevent MITM sniffing |
| SMTPS | Port `465` / `587` (STARTTLS) | Secures outgoing email transmission between clients and mail servers |
| POP3S / IMAPS | Port `995` / `993` | Encrypts incoming email retrieval and folder synchronization |
| SSH | Port `22` (`ssh user@IP`) | Provides encrypted remote shell access and port forwarding |
| SFTP | Port `22` (`sftp user@IP`) | Transfers files securely over an SSH session |
| FTPS | Port `21` / `990` | Secures traditional FTP connections using SSL/TLS certificates |
| VPN | OpenVPN / WireGuard / IPsec | Creates an encrypted tunnel across public networks for secure remote access |

---

## 🚩 Flag / Lab Solution Notes

- **Task 1 (Introduction):** Read the room overview covering how TLS, SSH, and VPNs protect network traffic.
- **Task 2 (TLS):**
    - Examined the TLS handshake process, cipher suite negotiation, digital certificates, and how asymmetric encryption establishes a shared symmetric session key.
- **Task 3 (HTTPS):**
    - Understood how HTTPS protects web traffic against packet sniffing and Man-in-the-Middle (MITM) attacks compared to plain HTTP.
- **Task 4 (SMTPS, POP3S, and IMAPS):**
    - Reviewed how implicit TLS and explicit `STARTTLS` secure email communications and prevent credential harvesting.
- **Task 5 (SSH):**
    - Practiced connecting securely to a remote host using `ssh`, verifying host key fingerprints, and understanding key-based vs. password authentication.
- **Task 6 (SFTP and FTPS):**
    - Compared SFTP (SSH File Transfer Protocol) and FTPS (FTP Secure), practicing secure file uploads and downloads via `sftp`.
- **Task 7 (VPN):**
    - Explored how VPN tunneling encapsulates and encrypts all device traffic to securely connect remote users to private networks.
- **Task 8 (Closing Notes):** Completed the Networking Secure Protocols room overview.

---

## 💡 What I Learned

- How TLS certificates and handshakes establish trust and encrypt application-layer traffic.
- Why replacing cleartext protocols (`HTTP`, `Telnet`, `FTP`, `SMTP`) with encrypted alternatives (`HTTPS`, `SSH`, `SFTP`, `SMTPS`) is essential for network defense.
- How VPN tunnels protect overall network traffic when operating over untrusted public networks.