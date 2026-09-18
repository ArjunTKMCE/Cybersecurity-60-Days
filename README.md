# Cybersecurity 60-Day Challenge

## Task 1 — Foundation & Environment Setup (Days 1–12)

This repository contains my Task 1 lab report, study notes, Linux cheat-sheet, tool notes, and practical evidence.

### Lab Environment
- VirtualBox 7.2.16
- Kali Linux 2026.2
- Metasploitable2
- Kali Host-Only IP: `192.168.56.101`
- Metasploitable2 Host-Only IP: `192.168.56.102`
- Host-Only network: `192.168.56.0/24`

### Network
```text
Internet
   |
  NAT
   |
Kali Linux
eth0: 10.0.2.15
eth1: 192.168.56.101
   |
   | Host-Only 192.168.56.0/24
   |
Metasploitable2
eth0: 192.168.56.102
```

### Practical Evidence
1. Metasploitable2 `ifconfig`
2. Kali → Metasploitable2 `ping`
3. Nmap host discovery
4. Nmap service scan
5. Wireshark ICMP capture
6. Netcat TCP connection
7. Burp Suite HTTP history

> The Netcat practical was completed, but its screenshot still needs to be added.

### Contents
- [Lab Setup Report](Day-01-12-Foundation/Lab-Setup-Report.pdf)
- [Linux Cheat-Sheet](Day-01-12-Foundation/Linux-Cheat-Sheet.md)
- [Cybersecurity Basics](Day-01-12-Foundation/Cybersecurity-Basics.md)
- [Networking Basics](Day-01-12-Foundation/Networking-Basics.md)
- [Cryptography](Day-01-12-Foundation/Cryptography.md)
- [Nmap](Day-01-12-Foundation/Tools/Nmap.md)
- [Wireshark](Day-01-12-Foundation/Tools/Wireshark.md)
- [Burp Suite](Day-01-12-Foundation/Tools/Burp-Suite.md)
- [Netcat](Day-01-12-Foundation/Tools/Netcat.md)

### Safety
All testing was performed in my own isolated training environment using Kali Linux and the intentionally vulnerable Metasploitable2 VM.
