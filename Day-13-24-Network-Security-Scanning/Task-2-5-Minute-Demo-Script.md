# Task 2 — 5-Minute Demo Video Script

## 0:00–0:25 — Introduction
Hello, this is my walkthrough for Task 2, Network Security and Scanning, of the ApexPlanet 60-Day Cybersecurity Internship. I used an isolated VirtualBox lab with Kali Linux as the testing machine and Metasploitable2 as the intentionally vulnerable target.

## 0:25–1:15 — Reconnaissance and Nmap
First, I performed reconnaissance and network scanning against the lab target. The target IP is 192.168.56.102. I used Nmap to identify hosts, ports and services. The service scan identified multiple exposed services including FTP, SSH, Telnet, HTTP, SMB, MySQL, PostgreSQL, VNC and IRC.

## 1:15–2:00 — Nmap Analysis
The purpose of port and service scanning is to understand the attack surface. Legacy and unencrypted services such as FTP and Telnet require particular attention in real environments. I also performed the required Nmap scan variations for TCP, UDP, service detection and OS detection within the isolated lab.

## 2:00–3:20 — OpenVAS
Next, I used OpenVAS to perform a vulnerability scan of Metasploitable2. The completed scan used the OpenVAS Default scanner with the Full and fast configuration. The report covered one host and identified 69 results.

The severity distribution was 13 Critical, 10 High, 40 Medium and 6 Low. The report also showed a highest CVSS score of 10.0, classified as Critical.

## 3:20–4:15 — Findings and Defensive Meaning
These results demonstrate why vulnerability scanning is useful after port and service discovery. Nmap shows what is exposed, while OpenVAS helps identify known security issues associated with the discovered attack surface. In a real environment, the next steps would be validation, patching, service hardening, firewall restrictions and a follow-up scan.

## 4:15–5:00 — Conclusion
This completes my Task 2 practical work. I performed network reconnaissance, port and service scanning and vulnerability assessment against the isolated Metasploitable2 training target. The results were documented for analysis and defensive learning.
