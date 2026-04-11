# 🚨 SOC Incident Ticket – Phishing Attack & Account Compromise

## Incident Summary
A phishing email was received by user **umama-PC** containing a malicious link. The user interacted with the link, leading to suspicious DNS activity, unauthorized external login, and execution of a PowerShell script using execution policy bypass. The sequence of events indicates a confirmed phishing-based account compromise with post-exploitation activity.

---

## Timeline of Events
- 10:00 – Phishing email received (“Important Security Update”)  
- 10:02 – User clicked malicious link: http://account-security-update.net  
- 10:03 – DNS request observed for suspicious domain  
- 10:05 – External IP 203.0.113.77 logged into account successfully  
- 10:07 – PowerShell executed: update.ps1 with ExecutionPolicy Bypass  

---

## Key Evidence (IOCs)
- **Malicious Domain:** account-security-update.net  
- **IP Address:** 203.0.113.77  
- **PowerShell Command:** powershell.exe -ExecutionPolicy Bypass -File update.ps1  
- **Script File:** update.ps1  

---

## Investigation Summary
- The phishing email used urgency (“Important Security Update”) to trick the user into clicking a malicious link.  
- The domain is non-legitimate and likely designed for credential harvesting.  
- DNS activity confirms interaction with the malicious domain.  
- A successful login from an external IP indicates credential compromise.  
- Execution of PowerShell with bypassed execution policy strongly suggests post-exploitation activity, possibly for running malicious scripts or maintaining access.  

---

## Security Assessment
- **Attack Type:** Phishing → Credential Compromise → Post-Exploitation  
- **Severity:** 🔴 High  
- **Status:** Confirmed Security Incident  

### Risk Impact:
- Unauthorized account access  
- Potential data exposure  
- Possible malware execution  
- Risk of lateral movement  

---

## Conclusion
This incident is a confirmed phishing-based attack that led to full account compromise and execution of a suspicious PowerShell script. Immediate containment and investigation are required to prevent further damage.

---

## Recommended Response Actions
- Reset user credentials immediately  
- Terminate all active sessions  
- Block malicious domain account-security-update.net  
- Block IP 203.0.113.77  
- Investigate PowerShell script (update.ps1)  
- Perform endpoint scan for malware or persistence  
- Check for lateral movement across other accounts  
- Notify SOC team and affected user  

---

## MITRE ATT&CK Mapping
- **T1566** – Phishing (Initial Access)  
- **T1078** – Valid Accounts (Credential Access / Use)  
- **T1059.001** – PowerShell (Execution)  

