# VAPT Report — testphp.vulnweb.com

**Target:** testphp.vulnweb.com (public practice site).  
**Objective:** Non-destructive external vulnerability assessment focused on server configuration, component disclosure, and HTTP security headers.  
**Authorization:** Public practice target; testing performed in lab environment.

## Tools
- Nmap, Nikto, Gobuster, Burp Suite (Proxy & Repeater)

## Commands & Key Output (examples)
```bash
# Nmap service detection and default scripts
nmap -sC -sV -oN nmap_scan.txt testphp.vulnweb.com

# Directory enumeration (example)
gobuster dir -u http://testphp.vulnweb.com -w /usr/share/wordlists/dirb/common.txt -o gobuster.txt

# Nikto web server scan
nikto -host http://testphp.vulnweb.com -o nikto_report.txt
