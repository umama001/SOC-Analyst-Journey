# Day 6 – IP Address Investigation

## Alert Description
A system communicated with the IP address 185.199.110.153

## Initial Analysis
The IP address 185.199.110.153 is a public external IP, meaning the system communicated with a host on the internet. External connections are normal, but unknown IPs require verification and monitoring.

## Possible Scenarios

### Normal
It could belong to a legitimate service such as a website, CDN, or API.

### Suspicious
- Command-and-control (C2) communication  
- Data exfiltration  
- Malware contacting an attacker-controlled server  

## Decision
Monitor

## Reason
There is no clear evidence of malicious activity at this stage. However, since the IP is external and unknown, it should be monitored and investigated further by checking related domains, processes, and connection frequency.

## Next Step
Further investigation should be performed using threat intelligence tools.
