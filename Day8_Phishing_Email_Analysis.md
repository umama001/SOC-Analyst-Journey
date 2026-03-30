# Day 8 – Phishing Email Analysis

## Evidence – Phishing Email

**Subject:** Urgent! Your account will be suspended  
**From:** support@paypaI.com  

**Message:**  
Dear user,  
Your account has been flagged for unusual activity.  
Please click the link below to verify your account immediately:  
http://secure-paypal-login123.com  

Failure to act will result in permanent suspension.  

*Note: This email is a simulated phishing scenario used for training purposes.*

---

## Email Summary
The email claims that the user's account has been flagged for unusual activity and urges the user to verify their account immediately to avoid suspension.

## Indicators of Phishing
- Suspicious sender email (support@paypaI.com)  
- Lookalike domain using capital “I” instead of “l” (paypaI.com)  
- Urgent language (“verify immediately”)  
- Fear tactic (“account will be suspended”)  
- Suspicious link with misleading domain  

## Link Analysis
The URL http://secure-paypal-login123.com is not an official PayPal domain. It uses the word “paypal” to appear legitimate, but additional words like “login123” indicate it is likely a fake phishing site.

## Sender Analysis
The sender email (support@paypaI.com) is a spoofed address. It uses a lookalike domain where the letter “l” in “paypal” is replaced with a capital “I,” which is a common phishing technique.

## Decision
Phishing

## Reason
The email contains multiple phishing indicators, including a fake sender domain, misleading link, urgency, and fear tactics. These signs strongly indicate an attempt to trick users into revealing sensitive information.



