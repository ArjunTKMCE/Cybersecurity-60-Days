# Networking Basics

## OSI Model
1. Physical
2. Data Link
3. Network
4. Transport
5. Session
6. Presentation
7. Application

## TCP/IP Model
- Application
- Transport
- Internet
- Network Access

## Important Protocols
- **DNS:** Resolves domain names to IP addresses.
- **HTTP:** Web communication protocol.
- **HTTPS:** HTTP protected using TLS.
- **TCP:** Connection-oriented and reliable.
- **UDP:** Connectionless with lower overhead.

## IP Addressing
IPv4 uses 32 bits. The lab uses `192.168.56.0/24`.

For `/24`:
- Network: `192.168.56.0`
- Usable range: `192.168.56.1`–`192.168.56.254`
- Broadcast: `192.168.56.255`

## NAT
Network Address Translation translates addresses between networks. Kali uses NAT for Internet access and Host-Only networking for the private lab.
