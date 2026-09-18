# Linux Cheat-Sheet

| Command | Purpose | Example |
|---|---|---|
| `pwd` | Show current directory | `pwd` |
| `ls` | List files | `ls` |
| `cd` | Change directory | `cd Desktop` |
| `touch` | Create file | `touch testfile` |
| `chmod` | Change permissions | `chmod 644 testfile` |
| `chown` | Change owner/group | `sudo chown kali:kali testfile` |
| `apt` | Package management | `apt -v` |
| `dpkg` | Debian package management | `dpkg -l` |
| `ifconfig` | Show interfaces | `ifconfig` |
| `ping` | Test connectivity | `ping -c 4 192.168.56.102` |
| `netstat` | Show connections/ports | `netstat -tuln` |
| `traceroute` | Show network path | `traceroute google.com` |

## Lab IPs
```text
Kali eth0 (NAT):        10.0.2.15
Kali eth1 (Host-Only):  192.168.56.101
Metasploitable2 eth0:   192.168.56.102
Host-Only network:      192.168.56.0/24
```
