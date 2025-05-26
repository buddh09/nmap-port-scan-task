# Nmap Port Scan Task

## Objective:
Perform a TCP SYN scan on your local network using Nmap to discover open ports and understand potential security risks.

---

## Tools Used:
- Nmap
---

## Steps Performed:
1. Installed Nmap on the system.
2. Identified local IP range: `192.168.1.0/24`.
3. Ran a TCP SYN scan using the command:

nmap -sS 192.168.1.0/24


4. Collected and saved scan results to `scan_results.txt`.

---

## Observations:
- **192.168.1.1** had open ports: 21 (FTP), 53 (DNS), 80 (HTTP), 443 (HTTPS), etc.
- **192.168.1.5** had port 7070 open (realserver).
- **192.168.1.23** had all ports closed or reset.

---

## Potential Risks:
- Open ports like FTP (21) or HTTP (80) can expose services to attackers.
- Filtered SSH (22) shows limited access but should still be monitored.
- Realserver on 7070 may expose internal application servers.

---

## Conclusion:
This task helped me understand how attackers or admins can discover services running on devices in a local network. I practiced using Nmap to run a TCP SYN scan, interpreted the results, and learned to evaluate security risks based on open ports.
