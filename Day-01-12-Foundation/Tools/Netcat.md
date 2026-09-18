# Netcat

Netcat is a simple networking utility useful for basic TCP/UDP connectivity testing.

## Lab TCP Test

On Metasploitable2:
```bash
nc -l -p 4444
```

On Kali:
```bash
nc -v 192.168.56.102 4444
```

A test message was sent from Kali and received by Metasploitable2.

The practical was completed. Add the Netcat screenshot to the `Screenshots` folder before final submission.
