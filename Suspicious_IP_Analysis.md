# 🌐 Suspicious IP Address Investigation Report

## Incident Summary
A connection was detected between an internal system and an external IP address **185.199.110.153**, requiring analysis to determine whether the activity is legitimate or potentially malicious.

---

## Incident Details
- **IP Address:** 185.199.110.153  
- **Activity:** Outbound connection observed  
- **Incident Type:** External IP Communication  
- **Severity:** Low (Pending further validation)

---

## Investigation & Analysis
- The IP address is a public external IP, meaning communication occurred outside the internal network.
- External connections are common in normal operations (e.g., websites, APIs, CDNs).
- However, unknown IP addresses require validation to rule out malicious activity.

---

## Behavioral Considerations
If the connection is:
- Frequent and repetitive → could indicate automated communication  
- Associated with unknown processes → potential malware activity  
- Linked to suspicious domains → higher risk  

---

## Indicators of Compromise (IOCs)
- **IP Address:** 185.199.110.153

---

## Security Assessment

### Possible Legitimate Use
- Content delivery networks (CDNs)  
- Web services or APIs  
- Cloud-hosted platforms  

### Potential Threat Scenarios
- Command-and-Control (C2) communication  
- Data exfiltration  
- Malware beaconing to external server  

---

## Conclusion
At this stage, there is no confirmed evidence of malicious activity. The connection appears to be normal external communication, but further validation is required.

---

## Recommended Actions
- Monitor connection frequency and behavior  
- Check associated domains linked to the IP  
- Investigate processes initiating the connection  
- Validate IP reputation using threat intelligence tools  

