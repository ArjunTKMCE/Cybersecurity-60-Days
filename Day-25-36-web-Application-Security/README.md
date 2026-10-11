\# Task 3: Web Application Security Testing



\## Overview

This folder contains the documentation and evidence for Task 3 of my

ApexPlanet Cybersecurity Internship.



The practical exercises used DVWA (Damn Vulnerable Web Application)

on Kali Linux in a controlled local lab.



\## Tools Used

\- Kali Linux

\- DVWA

\- Burp Suite Community Edition

\- Apache

\- MariaDB

\- PHP

\- curl



\## Experiments



\### 1. SQL Injection

Tested SQL injection against the DVWA SQL Injection module and observed

multiple database records returned by a controlled test input.



\### 2. SQL Injection Mitigation

Created a separate local demonstration using a MySQLi prepared statement.

The tested injection input did not return all user records.



\### 3. Cross-Site Scripting (XSS)

Tested:

\- Stored XSS

\- Reflected XSS

\- DOM-based XSS



The controlled test payloads displayed browser alerts in DVWA.



\### 4. File Inclusion

Tested the DVWA File Inclusion module. The attempted local file disclosure

did not succeed. This limitation is documented in the report.



\### 5. Burp Suite

Used Burp Proxy and HTTP history to inspect requests to the local DVWA app.



\### 6. Cryptography

Tested the DVWA encode/decode functionality with a sample value.



\### 7. API Module

Opened the DVWA API page and recorded the displayed setup warnings.

A complete API security assessment was not performed.



\### 8. HTTP Security Headers

Inspected HTTP response headers using curl and recorded the observed results.



\## Mitigation Recommendations

\- Use parameterized SQL queries.

\- Encode untrusted output to prevent XSS.

\- Use allowlisted file identifiers instead of user-controlled include paths.

\- Protect state-changing requests against CSRF.

\- Configure and verify appropriate HTTP security headers.



\## Evidence

The `Evidence` folder contains screenshots captured during the practical.

The screenshots should be interpreted together with the report.



\## Report

See:

\- `Task-3-Web-Application-Security-Testing-Report.pdf`

\- `Task-3-Web-Application-Security-Testing-Report.docx`



\## Scope and Ethics

All testing was performed against a deliberately vulnerable application

in a local lab. No external systems were targeted.



Some tests remain incomplete; the report records these limitations honestly.

