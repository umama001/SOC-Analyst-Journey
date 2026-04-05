# Day 13 – Log Analysis

## Evidence – Log Data

[10:15:23] LOGIN FAILED - User: umama-PC - IP: 198.51.100.23  
[10:15:30] LOGIN FAILED - User: umama-PC - IP: 198.51.100.23  
[10:15:45] LOGIN SUCCESS - User: umama-PC - IP: 198.51.100.23  
[10:16:10] PowerShell Executed - File: script.ps1  
[10:17:05] DNS Request - secure-login-update.net  

---

## Log Summary
The logs show multiple failed login attempts followed by a successful login from the same external IP (198.51.100.23). After the successful login, a PowerShell script (script.ps1) was executed, followed by a DNS request to a suspicious domain (secure-login-update.net). This indicates possible unauthorized access and post-compromise activity.

---

## Timeline of Events
10:15:23 – Login failed for user umama-PC from IP 198.51.100.23  
10:15:30 – Another login attempt from the same IP failed  
10:15:45 – Login from IP 198.51.100.23 was successful  
10:16:10 – PowerShell script script.ps1 was executed  
10:17:05 – DNS request made to secure-login-update.net  

---

## Analysis
The sequence of events suggests a possible account compromise. After multiple failed login attempts, a successful login occurred from the same external IP. Following this, a PowerShell script was executed, which may indicate malicious activity. The DNS request to a suspicious domain suggests that the script may have attempted communication with an external server.

---

## Suspicious Indicators
- External IP: 198.51.100.23  
- Suspicious domain: secure-login-update.net  
- PowerShell execution: script.ps1  
- Multiple failed logins followed by a successful login  

---

## Possible Attack
Account compromise followed by post-exploitation activity  

---

## Decision
Yes, this is a real threat  

---

## Reason
The logs show a clear sequence of suspicious behavior, including repeated login attempts, successful access from an external IP, execution of a PowerShell script, and communication with a suspicious domain. This strongly indicates unauthorized access and potential malicious activity on the system.
