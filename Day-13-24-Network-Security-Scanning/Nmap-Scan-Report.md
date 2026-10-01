# Task 2 — Nmap Scan Report

## Scope
- Target: Metasploitable2
- Target IP: `192.168.56.102`
- Environment: isolated VirtualBox Host-Only lab network
- Purpose: reconnaissance, port discovery and service enumeration for the assigned training target.

## Scan Evidence / Results
A TCP service scan of the lab target identified **23 open TCP services/ports**:

| Port | Service |
|---|---|
| 21/tcp | FTP |
| 22/tcp | SSH |
| 23/tcp | Telnet |
| 25/tcp | SMTP |
| 53/tcp | DNS |
| 80/tcp | HTTP |
| 111/tcp | RPCbind |
| 139/tcp | NetBIOS-SSN |
| 445/tcp | Microsoft-DS/SMB |
| 512/tcp | exec |
| 513/tcp | login |
| 514/tcp | shell |
| 1099/tcp | Java RMI |
| 1524/tcp | Ingreslock |
| 2049/tcp | NFS |
| 2121/tcp | FTP proxy |
| 3306/tcp | MySQL |
| 5432/tcp | PostgreSQL |
| 5900/tcp | VNC |
| 6000/tcp | X11 |
| 6667/tcp | IRC |
| 8009/tcp | AJP13 |
| 8180/tcp | HTTP/unknown |

The baseline service scan demonstrates that the intentionally vulnerable training VM exposes a broad service surface.

## Required Nmap Activities
The Task 2 brief asks for:
- TCP SYN scanning (`-sS`)
- UDP scanning (`-sU`)
- Service/version detection (`-sV`)
- OS detection (`-O`)
- A written scan report

Use the following commands only against the isolated lab target:

```bash
sudo nmap -sS 192.168.56.102
sudo nmap -sU 192.168.56.102
sudo nmap -sV 192.168.56.102
sudo nmap -O 192.168.56.102
```

## Analysis
The exposed services include legacy protocols such as Telnet, FTP, r-services, SMB, and several application/database services. On a deliberately vulnerable VM such as Metasploitable2, this large exposed surface is expected and is useful for defensive learning.

Important security observations:
1. **Unencrypted/legacy protocols** such as FTP and Telnet can expose sensitive information if used in real environments.
2. **Multiple application and database services** increase the number of components that require hardening and patch management.
3. **Network exposure should be minimized** by disabling unnecessary services and restricting access with firewall rules.
4. Nmap findings should be correlated with the OpenVAS results rather than treated as proof that a service is exploitable.

## Limitations
The screenshots supplied for this report contain OpenVAS evidence but do not include screenshots of each individual Nmap command requested in the Task 2 brief. The port list above records the verified lab service-scan results; add the corresponding `-sS`, `-sU`, `-sV`, and `-O` screenshots to the GitHub repository if the evaluator requires command-level visual evidence.
