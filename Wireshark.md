# Wireshark

Wireshark captures and analyzes network packets.

## Lab Procedure
1. Select Kali `eth1` Host-Only interface.
2. Start capture.
3. Run:
```bash
ping -c 4 192.168.56.102
```
4. Filter with:
```text
icmp
```

The capture contained 4 Echo Requests and 4 Echo Replies between Kali and Metasploitable2.

Evidence: `../../Screenshots/05-Wireshark-ICMP-capture.txt`
