# 🌐 Network Traffic Analysis Using Wireshark

## Objective
Analyze network traffic using Wireshark to understand DNS resolution, TCP communication, and TLS encryption behavior in normal browsing activity.

---

## Filters Applied
- dns – to observe domain resolution requests
- tcp – to analyze connection establishment and data transfer
- tls – to observe encrypted communication

---

## Observations
### DNS Traffic
- Device sent DNS requests to resolve domain names into IP addresses
- Example domain: youtube.com
- DNS queries were frequent during web browsing sessions
### TCP Traffic
- TCP connections were established between local device and remote web servers
- Three-way handshake observed (SYN, SYN-ACK, ACK)
- Indicates stable and reliable communication channels
### TLS Traffic
- Encrypted communication observed during HTTPS sessions
- Payload data was not visible due to encryption
- Confirms secure communication between client and server

---

## Example Analysis
- Source IP: 192.168.100.103
- Destination IP: 192.168.100.1
- Domain: youtube.com
Protocol: DNS
## Analysis
- The client requested DNS resolution for a well-known domain
- The request was sent to the local router acting as DNS resolver
-This is expected behavior during normal web browsing

---

## Security Assessment
- No suspicious domains observed
- No unusual external IP communication detected
- Traffic pattern matches normal user browsing behavior

---

## Conclusion
Network traffic observed in this session is consistent with normal browsing activity. DNS, TCP, and TLS behaviors all align with expected communication patterns in secure web usage.
