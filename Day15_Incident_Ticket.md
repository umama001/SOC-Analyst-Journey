# Day 15 – SOC Incident Ticket

## Alert Summary
A phishing email was received by the user "umama-PC" containing a malicious link. The user clicked the link, followed by a DNS request to a suspicious domain. Shortly after, an external IP (203.0.113.77) was observed logging into the account successfully. A PowerShell script was then executed using ExecutionPolicy Bypass.

---

## Key Evidence
- Email received: "Important Security Update"
- Malicious link clicked: http://account-security-update.net
- DNS request to suspicious domain detected
- Login from external IP: 203.0.113.77
- Successful login after external access
- PowerShell execution: powershell.exe -ExecutionPolicy Bypass -File update.ps1

---

## Analysis
The sequence of events suggests a likely phishing attack leading to credential compromise. The user interacted with a malicious domain which likely resulted in credential theft. This was followed by a successful login from an external IP, indicating unauthorized access. The execution of a PowerShell script using ExecutionPolicy Bypass suggests post-compromise activity, likely used to execute malicious commands or scripts.

---

## Risk Level
High

---

## Decision
Real Threat – Confirmed Security Incident (Requires Immediate Response)

---

## Recommended Actions
- Reset user credentials immediately
- Terminate all active sessions
- Block IP address 203.0.113.77
- Investigate PowerShell script (update.ps1)
- Perform endpoint scan for further compromise
- Check for lateral movement or additional accounts affected
- Notify security team and user

---

## Reason
Multiple correlated indicators confirm malicious activity: phishing interaction, external unauthorized login, and execution of a PowerShell script with bypassed execution policy. This strongly indicates a successful phishing-based compromise requiring immediate containment.

---

## MITRE ATT&CK Mapping

- Initial Access: Phishing (T1566)
- Credential Access: Valid Accounts (T1078)
- Execution: PowerShell (T1059.001)

---

## Severity Justification
This incident is classified as High severity due to confirmed unauthorized access, execution of a suspicious script, and potential system compromise. The attacker has already gained access and executed commands, increasing the risk of further damage.
