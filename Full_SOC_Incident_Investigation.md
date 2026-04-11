# 🚨 SOC Incident Report – Phishing Attack with Post-Exploitation Activity

---

## Incident Summary
A security incident was identified involving user **umama-PC**, where a phishing email led to credential compromise, unauthorized access, and execution of a suspicious PowerShell script, indicating potential post-exploitation activity.

---

## Incident Details
- **User:** umama-PC  
- **Malicious Domain:** secure-login-update.net  
- **Source IP:** 198.51.100.23  
- **Command Executed:** powershell.exe -ExecutionPolicy Bypass -File script.ps1  
- **Incident Type:** Phishing → Account Compromise → Post-Exploitation  
- **Severity:** 🔴 High  

---

## Timeline of Events
1. User received phishing email (“Verify your account now”)  
2. User clicked malicious link: secure-login-update.net  
3. DNS request observed for the domain  
4. Login attempt from external IP **198.51.100.23**  
5. Successful login confirmed  
6. PowerShell command executed with execution policy bypass  

---

## Investigation & Analysis
- The phishing email used urgency to trick the user into clicking a malicious link.  
- The domain **secure-login-update.net** is likely a credential harvesting site.  
- The attacker used stolen credentials to gain unauthorized access.  
- The login from an external or unusual IP confirms compromise.  
- Execution of PowerShell with **-ExecutionPolicy Bypass** suggests post-exploitation activity, potentially:
  - Running malicious scripts  
  - Establishing persistence  
  - Downloading additional payloads  

---

## Indicators of Compromise (IOCs)
- **Domain:** secure-login-update.net  
- **IP Address:** 198.51.100.23  
- **Command:** powershell.exe -ExecutionPolicy Bypass -File script.ps1  
- **Script:** script.ps1  

---

## Security Assessment
- Confirmed credential compromise  
- Unauthorized system access  
- Evidence of post-exploitation activity  
- High risk of:
  - Data exfiltration  
  - Malware persistence  
  - Further lateral movement  

---

## Conclusion
This is a confirmed high-severity security incident involving phishing, account compromise, and potential post-exploitation activity. Immediate containment and further investigation are required.

---

## Response Actions Taken
- User credentials reset  
- Malicious IP blocked  
- Active sessions terminated  
- Suspicious script flagged for analysis  
- System monitored for further activity  
- Security team and user notified  


