# nmap-port-scan-task
Scanning local network for open ports using Nmap

## Objective
To discover open ports and services on local network devices using Nmap, and understand exposure risks.

##  Tools Used
- Nmap (`-sS` TCP SYN scan)

##  Steps Performed
1. Identified my local IP range as `192.168.1.0/24`
2. Ran the following command:
   ```bash
   nmap -sS 192.168.1.0/24

3.Noted IPs that were active and identified open ports on them

4.Saved the scan results in scan_results.txt

## Key Findings
A .192.168.1.1:

Open ports: 21 (FTP), 53 (DNS), 80 (HTTP), 443 (HTTPS)

Port 22 is filtered (possible firewall or IDS)

B .192.168.1.5:

Open port: 7070 (often used by streaming or management services)

C .192.168.1.23:

All ports closed (host is up but no services exposed)

## Risk Assessment
FTP (Port 21): Insecure, may expose login credentials if not encrypted.

HTTP (Port 80): Web service may leak sensitive data if not secured.

SSH (Port 22): Filtered — may be protected by firewall but still detected.

Open ports may expose services vulnerable to attacks if outdated or misconfigured.

## Conclusion
This task helped me understand how attackers or admins can discover services running on devices in a local network. I practiced using Nmap to run a TCP SYN scan, interpreted the results, and learned to evaluate security risks based on open ports.
