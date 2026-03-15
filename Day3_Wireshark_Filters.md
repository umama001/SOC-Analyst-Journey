# Day 3 – Wireshark Filtering

## Filters Used
dns
tcp
tls

## Observations

### DNS
DNS traffic showed small requests from my computer to resolve domain names into IP addresses.

### TCP
TCP traffic showed communication between my device and web servers while browsing websites.

### TLS
TLS traffic showed encrypted communication when visiting secure websites.

## Example DNS Query

Source IP: 192.168.100.103  
Destination IP: 192.168.100.1  
Domain: youtube.com  

Explanation:  
My computer sent a DNS request to the router (acting as a DNS server) to resolve the domain youtube.com.
This shows normal browsing activity and does not appear suspicious.

