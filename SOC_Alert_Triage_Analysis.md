# 🚨 SOC Alert Triage Report

## Incident Summary
Multiple security alerts were received simultaneously and triaged based on risk level, potential impact, and urgency to determine the appropriate investigation order.

---

## Alert Overview

### 🔴 Alert 1: Multiple Failed Login Attempts (Admin Account)
- **Priority:** High  
- **Type:** Potential Brute-Force Attack  

### 🟡 Alert 2: Suspicious Domain Access
- **Domain:** free-movie-download123.xyz  
- **Priority:** Medium  
- **Type:** Potential Phishing / Malware  

### 🟢 Alert 3: Normal DNS Traffic
- **Domain:** google.com  
- **Priority:** Low  
- **Type:** Normal Activity  

---

## Indicators of Compromise (IOCs)
- **Domain:** free-movie-download123.xyz  
- **Target Account:** Admin account (failed login attempts)

---

## Triage Analysis

### 🔴 Alert 1 – Failed Logins (High Priority)
- Multiple failed login attempts detected on a privileged account  
- High risk of brute-force attack  
- If successful, attacker could gain full administrative access  

### 🟡 Alert 2 – Suspicious Domain (Medium Priority)
- Domain contains suspicious keywords (“free”, “download”)  
- Possible phishing or malware distribution site  
- No confirmed compromise yet  

### 🟢 Alert 3 – Normal Traffic (Low Priority)
- DNS request to trusted domain (google.com)  
- Expected user activity  
- No security concern  

---

## Investigation Priority Order
1. 🔴 Failed Login Attempts (Admin Account)  
2. 🟡 Suspicious Domain Access  
3. 🟢 Normal DNS Traffic  

---

## Recommended Actions

### 🔴 High Priority Alert
- Investigate login logs immediately  
- Check source IPs  
- Lock or protect admin account if needed  
- Escalate to L2 if attack confirmed  

### 🟡 Medium Priority Alert
- Analyze domain reputation  
- Check if user accessed the domain  
- Monitor for further activity  

### 🟢 Low Priority Alert
- No action required  
- Mark as normal activity  

---

## Conclusion
Alerts were triaged based on risk and impact. The admin account login attempts represent the highest threat and require immediate attention, while the suspicious domain requires monitoring. Normal DNS activity does not pose a risk.
