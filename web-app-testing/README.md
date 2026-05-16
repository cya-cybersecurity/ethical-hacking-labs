# Web Application Penetration Testing Lab

## Overview
In this lab, I performed web application penetration testing against the OWASP Broken Web Applications (BWA) environment using Kali Linux. The objective was to explore common web vulnerabilities including Local File Inclusion (LFI), Remote File Inclusion (RFI), file upload exploitation, MySQL enumeration, and SQL injection attacks using Burp Suite and sqlmap.

---

## Tools & Technologies
- Kali Linux
- OWASP BWA / DVWA / bWAPP
- Burp Suite
- sqlmap
- MySQL
- Linux CLI
- Netcat

---

## Key Activities

### Local File Inclusion (LFI)
- Exploited Local File Inclusion vulnerabilities to access sensitive Linux system files such as:
  - `/etc/passwd`
  - `/etc/group`
  - SSH configuration files
  - filesystem and host mapping information

### File Upload Exploitation
- Demonstrated file upload exploitation by uploading a text file to DVWA.
- Tested a bash reverse shell connection between Kali Linux and the OWASP VM.

### MySQL Enumeration
- Connected to the OWASP MySQL server via SSH.
- Enumerated databases, tables, usernames, and password hashes from vulnerable applications such as bWAPP and DVWA.

### SQL Injection Testing
- Configured Burp Suite as a proxy to intercept HTTP requests.
- Used sqlmap to automate SQL injection testing against bWAPP.
- Used sqlmap to:
  - Identify the backend DBMS (MySQL)
  - Enumerate databases and tables
  - Identify database columns
  - Dump credential data from vulnerable tables

---

## Skills Demonstrated
- Web application security testing
- Vulnerability exploitation
- Linux system enumeration
- SQL injection testing
- HTTP proxy interception
- Database enumeration
- Reverse shell concepts
- Offensive security tooling

---

## Key Takeaway
This lab strengthened my understanding of how insecure web applications can expose sensitive system and database information when proper input validation and security controls are missing. It also provided hands-on experience using industry-recognized penetration testing tools in a controlled lab environment.
