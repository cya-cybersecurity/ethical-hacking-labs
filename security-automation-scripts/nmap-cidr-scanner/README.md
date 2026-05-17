

# Nmap CIDR Scanner Automation

## Overview
This Bash script automates network enumeration by reading CIDR ranges from a text file and performing service/version detection scans using Nmap without requiring root privileges.

The script validates CIDR input, skips invalid entries, and stores scan results in organized output files for later analysis.

---

## Features
- Reads multiple CIDR ranges from a file
- Performs automated `nmap -sV` scans
- Runs without sudo/root access
- Validates CIDR notation before scanning
- Skips invalid or malformed entries
- Saves results into individual output files
- Includes basic error handling and logging

---

## Technologies Used
- Bash scripting
- Linux command line
- Nmap

---

## Script Usage

### 1. Make the script executable

```bash
chmod +x scan_cidrs_rootless.sh
````

### 2. Create a CIDR input file

Example `cidrs.txt`:

```text
192.168.1.0/24
10.0.0.0/24
172.16.1.0/24
```

### 3. Run the script

```bash
./scan_cidrs_rootless.sh cidrs.txt
```

---

## Output

Results are stored inside the `results/` directory.

Example:

```text
results/
├── 192.168.1.0_24.nmap
├── 10.0.0.0_24.nmap
└── 172.16.1.0_24.nmap
```

---

## Example Functionality

The script:

1. Reads CIDR ranges line by line
2. Removes comments and whitespace
3. Validates CIDR notation
4. Executes `nmap -sV`
5. Saves scan output to individual files

---

## Skills Demonstrated

* Network enumeration
* Bash scripting
* Input validation
* Security automation
* File handling
* Linux administration

---

## Disclaimer

This project was created for educational purposes and authorized lab environments only.

```
```
