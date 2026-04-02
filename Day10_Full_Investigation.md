# Day 10 – Full SOC Investigation

## Scenario
User: umama-PC  
Event:
- User visited domain: secure-update-login.net  
- Shortly after, multiple failed login attempts detected  
- Followed by a successful login  

Source IP: 203.0.113.45  

---

## Initial Observations
- User visited a suspicious domain  
- Multiple failed login attempts occurred  
- A successful login was recorded from the same external IP  

---

## Analysis
The sequence of events suggests a possible attack chain. The user first visited a suspicious domain, which may have been a phishing site. Shortly after, multiple failed login attempts were detected, followed by a successful login from the same IP address. This indicates that the attacker may have obtained the user's credentials and successfully accessed the account.

---

## Possible Attack
Phishing attack leading to account compromise

---

## Decision
Yes, this is a real security threat

---

## Action
- Reset the user’s password immediately  
- Block the suspicious IP address (203.0.113.45)  
- Terminate active sessions  
- Monitor the account for further suspicious activity  
- Notify the user and security team  

---

## Reason
The user visited a suspicious domain that may have been used for credential harvesting. The timing of failed and successful login attempts strongly suggests that the attacker obtained valid credentials and accessed the account. This indicates a likely account compromise through phishing, requiring immediate response and containment.
