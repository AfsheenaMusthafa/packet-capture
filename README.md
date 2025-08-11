# packet-capture
packet capturing in wireshark while applying filters
# Wireshark Network Analysis

## Steps Followed

1. **Start capturing** on the active network interface in Wireshark.  
2. **Browse a website** and **ping a server** to generate network traffic.  
3. **Stop the capture** after approximately 1 minute.  
4. **Apply protocol filters** (e.g., `dns`, `http`, `icmp`, `https`) to isolate traffic by type.  
5. **Identify at least 3 different protocols** from the capture.  
6. **Export the capture** as a `.pcap` file for documentation.  
7. **Summarize findings** with protocol-specific details.  



## Protocol Findings & Packet Details

### 1. **Protocol: DNS**
- **Packet Type:** Query  
- **Domain:** example.com  
- **Query Type:** A (IPv4 address)  
![DNS Packet Screenshot](images/dns.png)



### 2. **Protocol: HTTPS**
- **Destination IP:** 93.184.216.34  
- **Port:** 443  
- **Details:** TLS Handshake initiated  
![HTTPS Packet Screenshot](images/https.png)



### 3. **Protocol: HTTP**
- **Request Method:** GET  
- **Host:** example.com  
- **Resource:** /index.html  
- **Response Code:** 200 OK  
![HTTP Packet Screenshot](images/http.png)



### 4. **Protocol: ICMP (Echo Request)**
- **Type:** Echo Request  
- **Source:** 192.168.1.5  
- **Destination:** 8.8.8.8  
![ICMP Request Screenshot](images/icmp_request.png)



### 5. **Protocol: ICMP (Echo Reply)**
- **Type:** Echo Reply  
- **Source:** 8.8.8.8  
- **Destination:** 192.168.1.5  
![ICMP Reply Screenshot](images/icmp_reply.png)



## Summary

The packet capture revealed multiple network protocols in action:

- **DNS** resolved domain names to IP addresses.  
- **HTTPS** established a secure connection via TLS handshake.  
- **HTTP** was used for direct web requests and responses.  
- **ICMP** was observed for network diagnostics (ping request/reply).  

This analysis shows how various protocols interact to enable web browsing and connectivity checks.

screenshots-includes pcap files of dns,icmp,http

