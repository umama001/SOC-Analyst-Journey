# 🚨 Security Log Analysis Report

## Incident Summary
Log analysis revealed suspicious activity involving multiple failed login attempts, a successful login from an external IP, execution of a PowerShell script, and a DNS request to a suspicious domain, indicating a likely account compromise with post-exploitation activity.

---

## Log Evidence
[10:15:23] LOGIN FAILED - User: umama-PC - IP: 198.51.100.23
[10:15:30] LOGIN FAILED - User: umama-PC - IP: 198.51.100.23
[10:15:45] LOGIN SUCCESS - User: umama-PC - IP: 198.51.100.23
[10:16:10] PowerShell Executed - File: script.ps1
[10:17:05] DNS Request - secure-login-update.net


---

## Timeline of Events
- 10:15:23 – Failed login attempt from IP 198.51.100.23  
- 10:15:30 – Second failed login attempt from same IP  
- 10:15:45 – Successful login from same external IP  
- 10:16:10 – PowerShell script **script.ps1** executed  
- 10:17:05 – DNS request to suspicious domain **secure-login-update.net**  

---

## Investigation & Analysis
- Multiple failed login attempts followed by a success indicate a brute-force or credential-based attack.  
- Successful login from an external IP suggests unauthorized access.  
- Execution of a PowerShell script with unknown origin indicates potential post-exploitation activity.  
- DNS request to a suspicious domain suggests possible command-and-control communication or payload retrieval.  

---

## Indicators of Compromise (IOCs)
- **IP Address:** 198.51.100.23  
- **Domain:** secure-login-update.net  
- **Script:** script.ps1  
- **Activity Pattern:** Multiple failed logins → successful login  

---

## Security Assessment
- Confirmed account compromise  
- Evidence of post-exploitation activity  
- High risk of:
  - Malware execution  
  - Data exfiltration  
  - Persistence mechanisms  
- **Severity:** 🔴 High  

---

## Conclusion
The log data confirms a security incident involving unauthorized access and malicious activity execution. The attack likely involved credential compromise followed by post-exploitation actions.

---

## Recommended Actions
- Reset user credentials immediately  
- Block IP address 198.51.100.23  
- Terminate active sessions  
- Investigate **script.ps1** for malicious behavior  
- Monitor for further suspicious activity  
- Escalate to incident response team  
