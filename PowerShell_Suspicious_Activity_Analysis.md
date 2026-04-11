# 🚨 Suspicious PowerShell Activity Investigation Report

## Incident Summary
A suspicious PowerShell command was detected on system **umama-PC**, using execution policy bypass to run a script. The activity requires validation to determine whether it is malicious or a false positive.

---

## Incident Details
- **User/System:** umama-PC  
- **Command Executed:** powershell.exe -ExecutionPolicy Bypass -File update_script.ps1  
- **Incident Type:** Suspicious Script Execution  
- **Severity:** 🟠 Medium  

---

## Investigation & Analysis
- The **-ExecutionPolicy Bypass** flag allows scripts to run without security restrictions.  
- This technique is commonly used by attackers to execute malicious scripts.  
- However, it is also used legitimately by:
  - System administrators  
  - IT automation scripts  
  - Software updates  

---

## Indicators of Compromise (IOCs)
- **Command:** powershell.exe -ExecutionPolicy Bypass -File update_script.ps1  
- **Script Name:** update_script.ps1  

---

## Security Assessment

### Suspicious Indicators
- Execution policy bypass used  
- Script execution from unknown source  

### Possible Legitimate Use
- Internal automation or update script  
- Authorized administrative activity  

---

## Conclusion
This activity is suspicious but not confirmed malicious. It cannot be classified as a false positive without verifying the script content and its origin.

---

## Recommended Actions
- Review contents of **update_script.ps1**  
- Identify script source (internal vs external)  
- Verify if execution was authorized  
- Check for related suspicious activity  
- Monitor system for further anomalies  
