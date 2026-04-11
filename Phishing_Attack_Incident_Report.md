# 🚨 SOC Incident Report – Phishing Attack Leading to Account Compromise

## Incident Summary
A security incident was identified involving user **umama-PC**, where access to a suspicious domain was followed by failed login attempts and a successful login from an external IP, indicating a likely account compromise.

---

## Incident Details
- **User:** umama-PC  
- **Suspicious Domain:** secure-update-login.net  
- **Source IP:** 203.0.113.45  
- **Incident Type:** Phishing → Account Compromise  
- **Severity:** High  

---

## Timeline of Events
1. User accessed suspicious domain **secure-update-login.net**  
2. Multiple failed login attempts detected  
3. Successful login from external IP **203.0.113.45**

---

## Investigation & Analysis
- The domain **secure-update-login.net** appears to be a phishing site designed to harvest user credentials.  
- The timing suggests the user may have entered credentials on the malicious site.  
- Multiple failed login attempts indicate the attacker was attempting to use stolen credentials.  
- The successful login confirms that valid credentials were obtained.  
- Login from an external or unusual IP further supports unauthorized access.

---

## Indicators of Compromise (IOCs)
- **Domain:** secure-update-login.net  
- **IP Address:** 203.0.113.45  

---

## Security Assessment
- Confirmed credential compromise  
- Unauthorized access to user account  
- High risk of further malicious activity (data access, lateral movement)

---

## Conclusion
This incident is a confirmed phishing attack leading to account compromise. The attacker successfully obtained user credentials and accessed the account from an external IP address.

---

## Response Actions Taken
- Password reset enforced  
- Malicious IP blocked  
- Active sessions terminated  
- User notified  
- Security team alerted  

---

## Recommendations
- Enable Multi-Factor Authentication (MFA)  
- Conduct phishing awareness training  
- Block known malicious domains  
- Monitor for similar activity across other accounts  
