# Networking Notes for Ethical Hacking

## 1. Introduction to Computer Networks
A **computer network** is a system that connects multiple devices so they can communicate and share data.

### Why Networking Matters in Ethical Hacking
- Understand how data travels
- Identify weaknesses in communication paths
- Find vulnerable services
- Perform reconnaissance and exploitation
- Secure networks against attacks

---t

## 2. Types of Networks
### 2.1 PAN (Personal Area Network)
Small-scale network like Bluetooth or hotspot.

### 2.2 LAN (Local Area Network)
Covers homes, offices. Most labs use LAN.

### 2.3 WAN (Wide Area Network)
Large-scale networks like the Internet.

### 2.4 MAN (Metropolitan Area Network)
City-wide networks.

---

## 3. Network Models

## 3.1 OSI Model (7 Layers)
| Layer | Name | Example | Hacker Focus |
|------|------|---------|--------------|
| 7 | Application | HTTP, DNS | Web hacking, DNS attacks |
| 6 | Presentation | SSL/TLS | Encryption issues |
| 5 | Session | APIs, sessions | Session hijacking |
| 4 | Transport | TCP, UDP | Port scanning, DoS |
| 3 | Network | IP | IP spoofing |
| 2 | Data Link | MAC | ARP spoofing |
| 1 | Physical | Cables, WiFi | Sniffing, jamming |

## 3.2 TCP/IP Model
| Layer | Equivalent OSI Layers | Protocols |
|-------|------------------------|-----------|
| Application | 5–7 | HTTP, DNS, FTP |
| Transport | 4 | TCP, UDP |
| Internet | 3 | IP, ICMP |
| Network Access | 1–2 | Ethernet, WiFi |

---

## 4. IP Addressing

### 4.1 IPv4
Example: `192.168.1.10`

### 4.2 Types of IP Addresses
- **Public IP** – ISP assigned  
- **Private IP** – LAN internal  
- **Static IP** – Manually set  
- **Dynamic IP** – From DHCP  

Private IP ranges:
- 10.0.0.0 – 10.255.255.255  
- 172.16.0.0 – 172.31.255.255  
- 192.168.0.0 – 192.168.255.255  

### 4.3 Subnetting
Dividing a network into smaller parts.  
Common subnet: **/24 = 255.255.255.0 (256 IPs)**

---

## 5. Important Protocols

### 5.1 TCP
Connection-oriented and reliable.

### 5.2 UDP
Connectionless and faster but unreliable.

### 5.3 ICMP
Used by **ping**, host discovery.

### 5.4 DNS
Domain name → IP.  
Targets: spoofing, poisoning, enumeration.

---

## 6. Ports

### 6.1 Well-Known Ports
| Port | Service |
|------|---------|
| 20/21 | FTP |
| 22 | SSH |
| 23 | Telnet |
| 25 | SMTP |
| 53 | DNS |
| 67/68 | DHCP |
| 80 | HTTP |
| 110 | POP3 |
| 443 | HTTPS |

### 6.2 Why Ports Matter
Used for:
- Reconnaissance  
- Service discovery  
- Vulnerability identification  

Tools: Nmap, Netcat, Masscan.

---

## 7. Network Devices

### 7.1 Router
Connects networks. Target for misconfig attacks.

### 7.2 Switch
Connects devices in LAN. Supports VLANs.

### 7.3 Firewall
Filters traffic. Hackers try to bypass it.

### 7.4 Access Point
Wireless device. Target for WiFi attacks.

---

## 8. Packet Structure

### 8.1 What is a Packet?
Small chunk of data sent over networks.

### 8.2 Packet Parts
- **Header** – sender/receiver info  
- **Payload** – actual data  
- **Trailer** – error checking  

Tools to inspect:
- Wireshark  
- tcpdump  

---

## 9. Common Network Attacks

### 9.1 Man-in-the-Middle (MITM)
Interception of traffic.

### 9.2 ARP Spoofing
Fake ARP messages to redirect data.

### 9.3 DoS / DDoS
Overloading a system.

### 9.4 Port Scanning
Discovering open ports.

### 9.5 Packet Sniffing
Capturing network traffic.

### 9.6 DNS Attacks
Spoofing, poisoning.

### 9.7 Password Attacks
Bruteforce, dictionary attacks.

---

## 10. Wireless Networking

### 10.1 WiFi Bands
- 2.4 GHz – longer range  
- 5 GHz – faster  

### 10.2 WiFi Security Protocols
| Protocol | Security |
|---------|----------|
| WEP | Very weak |
| WPA | Improved |
| WPA2 | Standard |
| WPA3 | Strongest |

### 10.3 WiFi Attacks
- Deauthentication  
- Evil twin  
- Handshake capture  
- WPA2 cracking  

Tools: Aircrack-ng, Bettercap.

---

## 11. VPN & Proxy Basics

### 11.1 VPN
Encrypts and hides your traffic.

### 11.2 Proxy
Forwards requests for anonymity.

---

## 12. Network Security Best Practices
- Strong passwords  
- Disable unused services  
- Enable firewalls  
- Use VPN  
- Patch systems  
- Use encryption  
- Monitor network traffic  

---

## 13. Important Tools for Networking & Hacking
| Tool | Use |
|------|-----|
| Nmap | Port scanning |
| Wireshark | Packet analysis |
| Aircrack-ng | WiFi hacking |
| Netcat | Connections, reverse shells |
| Bettercap | MITM attacks |
| Metasploit | Exploitation |

---








