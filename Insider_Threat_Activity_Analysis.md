# 🚨 Insider Threat Activity Analysis Report

---

## Incident Summary
Suspicious user activity was detected involving access to sensitive files and connection of a USB device within a short time frame, indicating potential data exfiltration behavior.

---

## Log Evidence
[09:00:10] LOGIN SUCCESS - User: umama-PC - IP: 192.168.1.10
[09:05:22] FILE ACCESS - File: report.docx
[09:07:45] FILE ACCESS - File: passwords.xlsx
[09:10:02] USB DEVICE CONNECTED
[09:12:33] FILE ACCESS - File: financial_data.xlsx
[09:15:10] LOGOUT

---

## Timeline of Events
- 09:00:10 – User login successful  
- 09:05:22 – Access to normal file (report.docx)  
- 09:07:45 – Access to sensitive file (passwords.xlsx)  
- 09:10:02 – USB device connected  
- 09:12:33 – Access to sensitive file (financial_data.xlsx)  
- 09:15:10 – User logged out  

---

## Investigation & Analysis
- Initial activity appears normal (login + standard file access).  
- Subsequent access to sensitive files raises concern.  
- USB device connection during session introduces risk of data exfiltration.  
- Rapid access to multiple sensitive files suggests unusual behavior pattern.  

---

## Context Consideration
- If user role requires access, activity may be legitimate  
- If not authorized, activity is highly suspicious  

---

## Indicators of Compromise (IOCs)
- Sensitive files accessed: passwords.xlsx, financial_data.xlsx  
- Activity pattern: Rapid access to sensitive files  
- Device activity: USB device connected  

---

## Security Assessment
- Potential insider threat or unauthorized data handling  
- Risk of:
  - Data exfiltration via removable media  
  - Exposure of sensitive information  
- **Severity:** 🔴 High (Pending user activity validation)

---

## Conclusion
The activity is highly suspicious and may indicate a potential data exfiltration attempt. Further investigation is required to determine whether the behavior is authorized or malicious.

---

## Recommended Actions
- Verify user role and access permissions  
- Check if USB usage was authorized  
- Review file transfer activity  
- Monitor user behavior for recurrence  
- Escalate if unauthorized access is confirmed  
