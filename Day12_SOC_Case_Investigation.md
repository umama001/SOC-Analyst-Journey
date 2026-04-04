# Day 12 – SOC Case Investigation

## Scenario
User: umama-PC  

The user received an email with the subject "Verify your account now" and clicked the link http://secure-login-update.net. A DNS request for this domain was observed. Shortly after, a login attempt from IP 198.51.100.23 occurred, followed by a successful login. After login, a PowerShell command was executed:
powershell.exe -ExecutionPolicy Bypass -File script.ps1

---

## Key Events
- Phishing email received  
- User clicked suspicious link  
- DNS request for malicious domain  
- External login attempt detected  
- Successful login from unknown IP  
- PowerShell command execution  

---

## Analysis
The sequence of events indicates a phishing attack. The user likely entered credentials on a malicious site, leading to credential theft. The attacker then used these credentials to log in from an external IP. After gaining access, the attacker executed a PowerShell command with ExecutionPolicy Bypass, which may indicate post-exploitation activity such as running a malicious script.

---

## Attack Type
Phishing attack leading to account compromise and possible post-exploitation

---

## Indicators of Compromise (IOCs)
- Domain: http://secure-login-update.net  
- IP Address: 198.51.100.23  
- Command: powershell.exe -ExecutionPolicy Bypass -File script.ps1  
- Script: script.ps1  

---

## Decision
Confirmed security incident (High severity)

---

## Response Actions
- Reset user credentials immediately  
- Block the suspicious IP address (198.51.100.23)  
- Terminate all active sessions  
- Investigate the script (script.ps1)  
- Monitor the system for further suspicious activity  
- Notify the security team and affected user  

---

## Reason
This is a confirmed phishing attack that resulted in account compromise. The user interacted with a malicious domain, followed by unauthorized access from an external IP. The execution of a PowerShell script suggests potential post-exploitation activity. Immediate response is required to contain the threat and prevent further damage.
