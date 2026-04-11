# 🌐 Web Browsing Traffic Analysis

## Objective
Analyze network traffic generated during normal web browsing activities using Wireshark to understand how DNS, TCP, and TLS behave in real-time user sessions.

---

## Observed Activity
Web browsing sessions included access to:
- Wikipedia
- Amazon
- TryHackMe
- Google Search
- YouTube (video streaming)

---

## Traffic Analysis
### DNS Activity
- Multiple DNS queries observed for visited domains
- Each website triggered domain resolution before connection establishment
- No unknown or suspicious domains detected
### TCP Activity
- Continuous TCP connections established for web browsing and video streaming
- High packet volume observed during YouTube video playback
- Connections remained stable and consistent
### TLS Activity
- HTTPS traffic observed for all major websites
- All communications were encrypted
- No visible payload data due to TLS encryption

---

## Behavioral Analysis
- DNS requests matched user-visited domains
- TCP traffic increased significantly during video streaming
- No unexpected external IP connections observed
- Traffic pattern aligned with normal user browsing behavior
  
---

## Security Assessment
- No suspicious domains identified
- No abnormal or unknown external communication
- Traffic behavior consistent with legitimate web usage

---

Conclusion
The observed network activity represents normal web browsing behavior. No indicators of compromise or malicious activity were detected during this session.
