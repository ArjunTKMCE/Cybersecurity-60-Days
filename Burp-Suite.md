# Burp Suite

Burp Suite was used to inspect HTTP traffic in the isolated lab.

## Procedure
1. Open Burp Suite Community Edition.
2. Start a temporary project.
3. Open Burp's built-in browser.
4. Visit:
```text
http://192.168.56.102
```
5. Open **Proxy → HTTP history**.

Observed:
- Host: `192.168.56.102`
- Method: `GET`
- URL: `/`
- Status: `200`
- Title: `Metasploitable2 - Linux`

Evidence: `../../Screenshots/07-Burp-HTTP-history.png`
