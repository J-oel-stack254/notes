# Ethical Hacking Notes  
_Complete Markdown Notes with Explanations_

---

# 1. Introduction to Ethical Hacking

## 1.1 What is Ethical Hacking?
Ethical hacking is the legal and authorized practice of testing computers, networks, and systems to identify vulnerabilities before malicious hackers exploit them.  
Ethical hackers help organizations strengthen their security by:
- Discovering weaknesses  
- Reporting them  
- Helping fix them  

Ethical hacking must always be:
- Legally authorized  
- Performed within scope  
- Documented carefully  

---

## 1.2 Types of Hackers

### White-Hat Hackers (Ethical Hackers)
- Work with permission  
- Improve security  
- Follow laws and guidelines  

### Black-Hat Hackers
- Unauthorized  
- Steal data or cause damage  
- Malicious intent  

### Grey-Hat Hackers
- Unauthorized but not malicious  
- Still illegal  
- Often report vulnerabilities without permission  

---

## 1.3 Phases of Ethical Hacking

### Phase 1: Reconnaissance (Information Gathering)
Used to collect information about the target.  
Types:
- **Passive Recon:** No direct interaction (Google, social media, public data).  
- **Active Recon:** Direct interaction (scanning, probing).

### Phase 2: Scanning
Analyzing the target system for:
- Open ports  
- Running services  
- Possible vulnerabilities  
Tools: Nmap, Nessus, OpenVAS.

### Phase 3: Gaining Access
Exploiting vulnerabilities discovered in the scanning phase.  
Techniques include:
- SQL injection  
- Brute-force attacks  
- Exploiting misconfigurations  

### Phase 4: Maintaining Access
Keeping access long enough to fully test the system.  
Examples:
- Installing backdoors  
- Privilege escalation  
- Persisting in the system  

### Phase 5: Clearing Tracks
Attackers hide their presence.  
Ethical hackers **do not** hide anything; they only study these techniques for defense knowledge.

---

# 2. Ethical Hacking Concepts

## 2.1 Vulnerabilities
Weak points in a system that attackers can exploit.  
Types:
- Software vulnerabilities  
- Misconfigurations  
- Weak passwords  
- Outdated systems  

---

## 2.2 Exploits
A method or code used to take advantage of a vulnerability.

Example:
- Exploiting an outdated Apache server to gain root access.

---

## 2.3 Payloads
Malicious code delivered through an exploit.  
Examples:
- Reverse shells  
- Meterpreter sessions  

---

## 2.4 Attack Vectors
Entry points attackers use to infiltrate a system.  
Examples:
- Phishing  
- Open ports  
- Weak Wi-Fi security  
- Unsafe websites  

---

# 3. Essential Tools for Ethical Hacking

## 3.1 Reconnaissance Tools
- **WHOIS** – Domain registration info  
- **NSlookup** – DNS information  
- **Recon-ng** – Automated OSINT framework  
- **Maltego** – Relationship mapping for OSINT  

---

## 3.2 Scanning Tools

### Nmap
Used to scan networks and identify:
- Open ports  
- Services  
- Operating system fingerprinting  

Examples:
```bash
nmap 192.168.1.1
nmap -A target.com
nmap -p 1-1000 target.com
Nessus / OpenVAS
Automated vulnerability scanners that detect:

Weak software

Configuration issues

High-risk vulnerabilities

3.3 Exploitation Tools
Metasploit – Framework for exploiting vulnerabilities

SQLmap – Automates SQL injection

Burp Suite – Web application testing

BeEF – Browser exploitation

3.4 Password Attacking Tools
John the Ripper – Local password cracking

Hashcat – Advanced hash cracking

Hydra – Network login brute force

3.5 Wireless Hacking Tools
Aircrack-ng – Wi-Fi password cracking

Kismet – Wireless monitoring

Reaver – WPS PIN brute force

4. Types of Attacks in Ethical Hacking
4.1 Social Engineering Attacks
Manipulating people instead of systems.
Examples:

Phishing

Impersonation

Fake websites

4.2 Network Attacks
ARP Poisoning
Tricks devices into sending data to the attacker by altering MAC/IP mappings.

MITM (Man-in-the-Middle)
Attacker intercepts communication between two devices.

DNS Spoofing/Poisoning
Redirects users to fake malicious websites.

Packet Sniffing
Capturing network traffic using tools like Wireshark.

4.3 Web Application Attacks
SQL Injection
Injecting malicious SQL queries.
Example:

sql
Copy code
' OR '1'='1
XSS (Cross-Site Scripting)
Injecting JavaScript into web pages to steal cookies or modify content.

CSRF (Cross-Site Request Forgery)
Forcing users to perform unintended actions.

#4.4 System Attacks
- Privilege Escalation – Gaining higher access

- Buffer Overflow – Crashing memory to run commands

- Zero-Day Exploits – Unknown vulnerabilities

5. Wireless Hacking
# 5.1 Wi-Fi Encryption Standards
- Standard	Strength
- WEP	Very weak
- WPA	Weak–medium
- WPA2	Strong
- WPA3	Very strong

5.2 Wireless Attacks
#Deauthentication attacks – Disconnecting users

- Handshake capture – For password cracking

- Evil Twin attack – Fake Wi-Fi network

6. Penetration Testing Reports
# A good pentest report includes:

- Executive summary

- Scope of testing

# Tools and methods used

- Vulnerabilities found

- Risk level (High/Medium/Low)

- Solutions and recommendations

7. **Legal and Ethical Requirements**
- Ethical hacking must always follow rules:

- Get written permission

- Do not exceed the agreed scope

- Do not damage systems

- Keep data confidential

- Provide accurate reports

- Unauthorized hacking is illegal and punishable.

8. **Ethical Hacking Certifications**
- Certification	Level	Purpose
- CEH	Intermediate	Ethical hacking fundamentals
- OSCP	Advanced	Practical penetration testing
- Security+	Beginner	Cybersecurity basics
- eJPT	Beginner	Hands-on penetration testing

9. Practice Labs
- HackTheBox

- TryHackMe

- OverTheWire

- VulnHub

- DVWA (Damn Vulnerable Web App)





