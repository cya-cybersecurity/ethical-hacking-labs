# Network Pivoting & SSH Tunneling Lab

## Overview

This lab focused on advanced network pivoting, SSH tunneling, dynamic port forwarding, and segmented network access within a controlled ethical hacking environment.

The exercises simulated real-world restricted network scenarios where direct access to internal systems was blocked. Using SSH tunneling, Proxychains, SOCKS proxies, firewall rules, and port forwarding techniques, internal systems and web applications were accessed securely from external systems.

This lab strengthened practical understanding of network segmentation, remote administration, tunneling workflows, and internal reconnaissance techniques commonly used in cybersecurity operations and penetration testing environments.

---

## Skills Demonstrated

- SSH tunneling and pivoting
- Dynamic and local port forwarding
- SOCKS proxy configuration
- Proxychains configuration and usage
- NAT and firewall rule management
- Remote Desktop Protocol (RDP)
- Internal network enumeration
- Network segmentation concepts
- Nmap scanning through tunnels
- Web application access through pivots
- Linux and Windows administration
- Troubleshooting remote connectivity issues

---

## Technologies & Tools

### Operating Systems
- Kali Linux
- BackTrack Linux
- Security Onion
- pfSense
- Windows 7
- Windows 8
- Windows Server 2008
- openSUSE
- OWASP Broken Web Applications (BWA)
- Metasploitable

### Networking & Security Tools
- SSH
- Proxychains
- SOCKS Proxy
- Nmap
- Nikto
- WhatWeb
- PuTTY
- RDP / rdesktop
- Netstat

---

## Lab Activities

### Part A – SSH Tunneling & Dynamic Port Forwarding

Configured a segmented lab environment where Kali Linux could only communicate with Security Onion through SSH.

Activities included:
- Configuring pfSense firewall and NAT rules
- Establishing SSH tunnels
- Creating SOCKS proxies
- Configuring Proxychains
- Performing scans through tunnels
- Accessing internal web applications via pivoting
- Running Nikto and WhatWeb through SSH tunnels
- Accessing OWASP BWA through dynamic forwarding

---

### Part B – Port Forwarding & Remote Access

Configured firewall rules and forwarding policies to allow controlled access to internal systems from external networks.

Activities included:
- Configuring Windows firewall port forwarding
- Enabling and testing RDP
- Establishing SSH access to internal Linux systems
- Accessing Windows systems through forwarded RDP ports
- Conducting internal Nmap scans through pivot points
- Using PuTTY tunneling for simultaneous remote access workflows

---

### Part C – Dynamic Proxying & Internal Enumeration

Configured dynamic SOCKS proxying with PuTTY and Firefox to enumerate internal web services across multiple segmented subnets.

Activities included:
- Dynamic port forwarding
- Browser proxy configuration
- Internal subnet reconnaissance
- Web service identification
- Service enumeration with Nmap
- Identifying exposed services on Metasploitable
- Testing FTP and Telnet authentication access in lab systems

---

## Key Concepts Practiced

- Network pivoting
- Defense evasion concepts
- Internal reconnaissance
- Segmented network traversal
- Secure remote administration
- Tunnel-based service access
- Multi-hop connectivity
- Proxy-based scanning

---

## Key Takeaways

This lab significantly improved my understanding of:
- How attackers and defenders traverse segmented networks
- SSH tunneling workflows in restricted environments
- Proxychains and SOCKS proxy configurations
- Firewall and NAT behavior
- Internal service enumeration techniques
- Troubleshooting complex connectivity paths

The exercises also reinforced the importance of proper segmentation, firewall configuration, and monitoring in enterprise environments.

---

## Ethical Use Disclaimer

This project was completed in isolated educational lab environments for authorized cybersecurity training purposes only. All tools and techniques demonstrated were performed within approved systems designed for defensive learning and ethical security testing.

---

## Author

Claudia Arrunategui  
Cybersecurity Student | Security+ Certified | Blue Team & Security Operations Focus
