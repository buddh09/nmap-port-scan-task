# nmap-port-scan-task
Scanning local network for open ports using Nmap

## Objective
To discover open ports and services on local network devices using Nmap, and understand exposure risks.

##  Tools Used
- Nmap (`-sS` TCP SYN scan)

## 🧪 Steps Performed
1. Identified my local IP range as `192.168.1.0/24`
2. Ran the following command:
   ```bash
   nmap -sS 192.168.1.0/24
