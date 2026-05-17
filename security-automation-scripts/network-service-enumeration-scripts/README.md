# Network Service Enumeration Scripts

## Overview

This project contains Bash scripts developed to automate network service enumeration across multiple CIDR ranges using Nmap.

The scripts scan network ranges provided in a CIDR input file and identify hosts exposing commonly targeted services such as:
- HTTP
- FTP
- SSH
- SMTP
- RDP
- SNMP

The project was created as part of cybersecurity and ethical hacking lab exercises focused on reconnaissance automation, service discovery, and Bash scripting.

---

## Skills Demonstrated

- Bash scripting
- Nmap automation
- Network reconnaissance
- Service enumeration
- CIDR-based scanning
- Parsing grepable Nmap output
- File handling and validation
- Error handling
- Temporary file management
- Linux command-line operations
- Network automation workflows

---

## Scripts Included

### HTTP Enumeration

```bash
scan_cidrs_port80.sh
```

Scans CIDR ranges for systems with TCP port 80 open.

---

### FTP Enumeration

```bash
ftp_script.sh
```

Scans CIDR ranges for systems exposing FTP services on port 21.

---

### SSH Enumeration

```bash
ssh_script.sh
```

Scans CIDR ranges for systems exposing SSH services on port 22.

---

### SMTP Enumeration

```bash
smtp_script.sh
```

Scans CIDR ranges for systems exposing SMTP services on port 25.

---

### RDP Enumeration

```bash
rdp_script.sh
```

Scans CIDR ranges for systems exposing Remote Desktop Protocol (RDP) services on port 3389.

---

### SNMP Enumeration

```bash
snmp_script.sh
```

Scans CIDR ranges for systems exposing SNMP services on UDP port 161.

This script includes:
- Root-aware execution logic
- UDP scanning support
- Netcat fallback functionality
- Best-effort non-root scanning

---

## CIDR Input File

The scripts utilize a shared CIDR input file:

```text
cidrs.txt
```

Example:

```text
172.16.99.0/24
10.6.6.0/24
10.5.5.0/24
192.168.0.0/24
```

---

## Example Usage

```bash
./scan_cidrs_port80.sh cidrs.txt results.txt
```

```bash
./ssh_script.sh
```

```bash
./rdp_script.sh
```

---

## How the Scripts Work

The scripts:

1. Read CIDR ranges from an input file
2. Execute targeted Nmap scans
3. Parse grepable output
4. Extract IP addresses exposing specific services
5. Save discovered hosts into output files
6. Deduplicate results automatically

---

## Features

- Non-root compatible scanning
- Fast TCP connect scans
- Grepable output parsing
- Temporary file cleanup
- Duplicate removal
- Input validation
- Comment support inside CIDR files
- Error handling for missing dependencies

---

## Requirements

- Linux environment
- Bash shell
- Nmap installed
- Netcat (optional for SNMP fallback mode)

Install Nmap:

```bash
sudo apt install nmap
```

Install Netcat:

```bash
sudo apt install netcat
```

---

## Example Output

```text
Scanning: 172.16.99.0/24
Scanning: 10.6.6.0/24

Done. IPs with port 22 open saved to: open_ssh_ips.txt
Total found: 12
```

---

## Educational Purpose

These scripts were created for educational cybersecurity lab environments to practice:
- Service discovery
- Network enumeration
- Bash scripting
- Reconnaissance automation
- Output parsing
- Nmap usage

---

## Ethical Use Disclaimer

These scripts are intended strictly for authorized cybersecurity testing and educational lab environments. Do not scan systems or networks without explicit authorization.

---

## Repository Structure

```text
.
├── cidrs.txt
├── ftp_script.sh
├── ssh_script.sh
├── smtp_script.sh
├── rdp_script.sh
├── snmp_script.sh
├── scan_cidrs_port80.sh
└── README.md
```

---

## Author

Claudia Arrunategui  
Cybersecurity Student | Security+ Certified | Blue Team & Security Operations Focus
