# 🚨 Phishing Email Investigation Report

## Incident Summary
A suspicious email was analyzed and identified as a phishing attempt designed to trick users into revealing sensitive information through a fake login page.

---

## Email Details
- **Subject:** Urgent! Your account will be suspended  
- **Sender:** support@paypaI.com  
- **Link:** http://secure-paypal-login123.com  
- **Incident Type:** Phishing Email  
- **Severity:** 🔴 High  

---

## Investigation & Analysis

### Email Content Analysis
- The message creates urgency (“verify immediately”)  
- Uses fear tactics (“account will be suspended”)  
- Encourages immediate action without verification  

### Sender Analysis
- **Sender Domain:** paypaI.com  
- Uses lookalike technique (capital “I” instead of “l”)  
- Common phishing method used to impersonate trusted brands  

### Link Analysis
- **URL:** secure-paypal-login123.com  
- Not an official PayPal domain  
- Uses brand name with random words (“login123”)  
- Likely designed for credential harvesting  

---

## Indicators of Compromise (IOCs)
- **Sender Email:** support@paypaI.com  
- **Malicious Domain:** secure-paypal-login123.com  

---

## Security Assessment
- Strong indicators of a phishing attack  
- High risk of:
  - Credential theft  
  - Account compromise  
  - Unauthorized access  

---

## Conclusion
This email is a confirmed phishing attempt using domain spoofing and social engineering techniques to deceive users and steal credentials.

---

## Recommended Actions
- Block sender domain and malicious URL  
- Report email to the security team or SOC  
- Warn affected users  
- Check if any users clicked the link  
- Reset credentials if compromise is suspected  




