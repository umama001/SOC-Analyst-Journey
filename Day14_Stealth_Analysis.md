# Day 14 – Stealth Activity Analysis

## Evidence – Logs
[09:00:10] LOGIN SUCCESS - User: umama-PC - IP: 192.168.1.10  
[09:05:22] FILE ACCESS - User: umama-PC - File: report.docx  
[09:07:45] FILE ACCESS - User: umama-PC - File: passwords.xlsx  
[09:10:02] USB DEVICE CONNECTED  
[09:12:33] FILE ACCESS - User: umama-PC - File: financial_data.xlsx  
[09:15:10] LOGOUT - User: umama-PC  

---

## Observations

### Normal Activity
- User successfully logged in  
- Accessed a standard document (report.docx)  
- Session ended with logout  

### Suspicious Activity
- Access to sensitive file passwords.xlsx  
- Access to financial_data.xlsx  
- USB device connected during active session  
- Multiple sensitive files accessed within a short timeframe  

---

## Analysis
The user performed normal login activity followed by access to a standard document. However, shortly after, the user accessed sensitive files including passwords.xlsx and financial_data.xlsx. During the same session, a USB device was connected, which could allow data transfer outside the system. The combination of sensitive file access and removable media usage suggests potential unauthorized data handling.

---

## Suspicious Indicators
- Access to passwords.xlsx  
- Access to financial_data.xlsx  
- USB device connection  
- Rapid access to multiple sensitive files  

---

## Possible Threat
Potential insider threat or data exfiltration attempt

---

## Decision
Suspicious activity – High risk, requires investigation

---

## Reason
Although no malware or failed authentication is observed, the user accessed multiple sensitive files and connected a USB device within a short timeframe. This pattern is consistent with possible data exfiltration behavior and should be investigated further to confirm intent.
