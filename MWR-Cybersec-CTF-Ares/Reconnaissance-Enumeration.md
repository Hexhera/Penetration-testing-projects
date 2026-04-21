# 🔍 Reconnaissance & Enumeration

Reconnaissance and enumeration was performed to acquire detailed information about the target.


## Techniques Used
- Nmap scanning (`-sV`, `-sC`)
- Full port scanning (`-p-`)
- Service identification


To perform an extensive examination of the Ares Mainframe, a full port scan was conducted with nmap. 

<img width="650" height="311" alt="image" src="https://github.com/user-attachments/assets/abe1bba5-7a65-47a9-892a-9dd0eaab829f" />


---

## Findings
- Port 80: HTTP service (Apache)
- Port 8080: Secondary web service
- Additional open ports discovered via full scan
- The scan results revealed 3 open ports with port 33333 TCP being the highest port running.


---

## Summary
📌 The system exposed multiple web services that increased the attack surface and allowed further enumeration.
