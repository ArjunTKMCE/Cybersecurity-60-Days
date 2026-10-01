# Cybersecurity 60-Day Challenge — Task 2

## Network Security & Scanning (Days 13–24)

### Target
Metasploitable2 in an isolated VirtualBox Host-Only network.

### Task Areas
- Reconnaissance
- Nmap port and service scanning
- OpenVAS vulnerability scanning
- Wireshark packet analysis
- Firewall basics

### Reports
- `Nmap-Scan-Report.md`
- `OpenVAS-Vulnerability-Report.md`
- `Task-2-Network-Security-Scanning-Report.pdf`
- `Task-2-Network-Security-Scanning-Report.docx`

### Evidence
The `Evidence/` directory contains the supplied OpenVAS evidence screenshots and the Task 2 requirements screenshot.

### Nmap Target
`192.168.56.102`

### Verified TCP Service Surface
The lab service scan identified 23 open TCP ports, including FTP, SSH, Telnet, SMTP, DNS, HTTP, SMB, MySQL, PostgreSQL, VNC, IRC and other services.

### OpenVAS Summary
- Hosts: 1
- Ports: 20/23
- Applications: 20/20
- CVEs: 36/36
- Results: 69
- Critical: 13
- High: 10
- Medium: 40
- Low: 6
- Highest reported CVSS: 10.0 Critical

### Safety
All testing was performed against the intentionally vulnerable Metasploitable2 VM in the isolated lab network. No external systems were targeted.
