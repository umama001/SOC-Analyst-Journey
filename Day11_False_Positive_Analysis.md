# Day 11 – False Positive Analysis

## Scenario
User: umama-PC  
Alert Type: Suspicious PowerShell Activity  
Command Executed: powershell.exe -ExecutionPolicy Bypass -File update_script.ps1  

---

## Initial Analysis
The command uses PowerShell with the -ExecutionPolicy Bypass option, which allows scripts to run without security restrictions. This can be suspicious because attackers often use it to execute malicious scripts.

---

## Investigation
To verify this activity, the following should be checked:
- Review the contents of update_script.ps1  
- Identify the source of the script  
- Confirm if this action was authorized or part of normal operations  
- Check for any additional suspicious activity on the system  

---

## Decision
Needs Further Investigation

---

## Reason
Although the use of PowerShell with ExecutionPolicy Bypass is suspicious, there is no additional evidence confirming malicious activity. At the same time, it cannot be considered a false positive without verifying the script and its origin. Therefore, further investigation is required before making a final determination.
