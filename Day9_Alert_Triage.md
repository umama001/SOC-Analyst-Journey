# Day 9 – Alert Triage
*Note: This is a simulated SOC triage scenario for training purposes.*
## Scenario
You are an L1 SOC Analyst. You receive three alerts at the same time:

🔴 Alert 1: Multiple failed login attempts detected on an admin account  
🟡 Alert 2: User visited domain: free-movie-download123.xyz  
🟢 Alert 3: Normal DNS traffic to google.com detected  

---

## Alert 1 – Failed Logins
Priority: High  
Reason: Multiple failed login attempts on an admin account may indicate a brute-force attack. If successful, it could lead to unauthorized access with high privileges, making it a critical risk.

## Alert 2 – Suspicious Domain
Priority: Medium  
Reason: The domain appears suspicious and may be associated with phishing, scams, or malware delivery. However, there is no confirmation of compromise yet.

## Alert 3 – Normal Traffic
Priority: Low  
Reason: DNS traffic to google.com is expected and represents normal user activity.

---

## Investigation Order
1. Alert 1 – Failed Logins  
2. Alert 2 – Suspicious Domain  
3. Alert 3 – Normal Traffic  

---

## Final Decision
Alerts are prioritized based on potential impact and risk. The failed login attempts on an admin account pose the highest risk due to possible unauthorized access. The suspicious domain requires investigation but has lower immediate impact. Normal traffic is low priority and does not require investigation.
