# Network Host Enumeration Scripts

## Overview

This project contains Bash scripts designed to automate basic network host enumeration and operating system identification using Nmap.

The scripts perform OS detection scans against a specified CIDR subnet and parse the results to count the number of Linux or Windows hosts discovered on the network.

These scripts were created as part of ethical hacking and cybersecurity lab exercises focused on network reconnaissance, automation, and Bash scripting.

---

## Skills Demonstrated

- Bash scripting
- Nmap automation
- Network reconnaissance
- OS fingerprinting
- Command-line argument handling
- Output parsing with grep and wc
- Linux command-line operations
- Basic scripting troubleshooting

---

## Scripts Included

### count_linux_hosts.sh

Scans a subnet using Nmap OS detection and counts the number of hosts identified as Linux systems.

Example:

```bash
./count_linux_hosts.sh 172.16.99.0/24
```

---

### count_windows_hosts.sh

Scans a subnet using Nmap OS detection and counts the number of hosts identified as Windows systems.

Example:

```bash
./count_windows_hosts.sh 172.16.99.0/24
```

---

## How It Works

Both scripts:

1. Accept a CIDR subnet as input
2. Execute an Nmap OS detection scan
3. Parse Nmap output using grep
4. Count matching operating system results
5. Display the total number of detected hosts

Example workflow:

```text
User Input → Nmap Scan → Output Parsing → Host Count
```

---

## Requirements

- Linux environment
- Bash shell
- Nmap installed
- Sudo privileges (recommended for accurate OS detection)

Install Nmap on Debian/Ubuntu:

```bash
sudo apt install nmap
```

---

## Example Output

```text
[*] Scanning network: 172.16.99.0/24 with OS detection...
[*] Number of Linux boxes found: 5
```

---

## Educational Purpose

These scripts were developed for educational cybersecurity lab environments to practice:
- Network enumeration
- Bash scripting
- OS fingerprinting
- Automation concepts

---

## Ethical Use Disclaimer

These scripts are intended strictly for authorized security testing and educational lab environments. Do not scan networks or systems without explicit permission.

---

## Author

Claudia Arrunategui  
Cybersecurity Student | Security+ Certified | Blue Team & Security Operations Focus
