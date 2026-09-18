# Nmap

## Host Discovery
```bash
nmap -sn 192.168.56.0/24
```

Identified lab hosts including Kali `192.168.56.101` and Metasploitable2 `192.168.56.102`.

## Service Scan
```bash
nmap 192.168.56.102
```

The scan identified numerous open services on the intentionally vulnerable target, including FTP, SSH, Telnet, HTTP, SMB, MySQL, PostgreSQL, VNC, IRC, and others.

Evidence: `../../Screenshots/03-Nmap-host-discovery.png` and `../../Screenshots/04-Nmap-service-scan.png`
