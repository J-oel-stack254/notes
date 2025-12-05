# Kali Linux Notes for Ethical Hacking

Kali Linux is a Debian-based penetration testing OS used by ethical hackers, cybersecurity professionals, and security researchers.

---

## 1. Introduction to Kali Linux

### What is Kali Linux?
Kali Linux is a security-focused operating system containing **hundreds of penetration-testing tools** for:
- Reconnaissance
- Exploitation
- Password cracking
- Digital forensics
- Wireless attacks
- Reverse engineering
- Social engineering

### Why Hackers Use Kali Linux
- Pre-installed hacking tools  
- Strong community support  
- Built for pentesting workflows  
- Customizable and lightweight  
- Works well in virtual machines

---

## 2. Installation Options

### 2.1 Install as Main OS
Kali replaces Windows/Linux entirely.  
**Risk:** Not recommended for beginners.

### 2.2 Dual Boot (Windows + Kali)
You choose which OS to start at boot.

### 2.3 Virtual Machine (Recommended)
Install Kali on:
- VMware
- VirtualBox
- Hyper-V

### 2.4 Live USB
Boot directly from a USB stick without installing.

---

## 3. Kali Linux Desktop Overview

Kali uses the **Xfce** or **Gnome** desktop.

### Important Areas
- **Terminal** — main hacking command area  
- **Applications Menu** → Tools grouped by category  
- **File Manager** — like Windows Explorer  
- **Settings** — customize environment  

---

## 4. Essential Linux Commands for Kali

### 4.1 File & Directory Commands
```bash
pwd          # show current directory
ls           # list files
ls -la       # list all files with details
cd           # change directory
cd ..        # go back
mkdir name   # create folder
rm file      # delete file
rm -r dir    # delete folder
cp src dst   # copy
mv src dst   # move/rename
4.2 Reading & Editing Files
bash
Copy code
cat file.txt      # view file
nano file.txt     # edit file (easy editor)
less file.txt     # scroll view
echo text > file  # write to file
4.3 System Commands
bash
Copy code
whoami        # show current user
uname -a      # system info
df -h         # disk storage
free -m       # RAM usage
top           # running processes
5. Package Management (APT)
5.1 Updating Kali
bash
Copy code
sudo apt update
sudo apt upgrade -y
5.2 Installing Tools
bash
Copy code
sudo apt install toolname
5.3 Removing Tools
bash
Copy code
sudo apt remove toolname
6. User & Permission Management
6.1 File Permissions
bash
Copy code
chmod 755 file
chmod +x script.sh      # make file executable
6.2 Ownership
bash
Copy code
chown user:user file
6.3 Switch Users
bash
Copy code
su root          # switch to root
sudo command     # run as admin
7. Kali Linux Tool Categories
Kali groups hacking tools by purpose.

7.1 Information Gathering
Nmap

Recon-ng

Maltego

7.2 Vulnerability Analysis
Nikto

OpenVAS

Nmap scripts (NSE)

7.3 Exploitation Tools
Metasploit Framework

ExploitDB

Armitage

7.4 Wireless Attacks
Aircrack-ng

Bettercap

Wifite

7.5 Password Attacks
Hydra

John the Ripper

Hashcat

7.6 Sniffing & Spoofing
Wireshark

Ettercap

Bettercap

7.7 Web Application Tools
Burp Suite

OWASP ZAP

SQLmap

Dirb / Gobuster

7.8 Forensics Tools
Autopsy

Sleuthkit

7.9 Reverse Engineering
Ghidra

Radare2

8. Useful Directories in Kali
Folder	Description
/home/user/	personal files
/etc/	configuration files
/opt/	third-party tools
/var/log/	logs
/usr/share/wordlists/	wordlists (rockyou.txt)

9. Networking Commands in Kali
9.1 Show Network Interfaces
bash
Copy code
ip a
9.2 Start/Stop Network Managers
bash
Copy code
sudo systemctl start NetworkManager
sudo systemctl stop NetworkManager
9.3 Monitor Mode (WiFi Hacking)
bash
Copy code
sudo airmon-ng start wlan0
sudo airmon-ng stop wlan0mon
10. Ethical Hacking Workflow in Kali Linux
Step 1 — Reconnaissance
Tools:

Nmap

Recon-ng

Whois

Dig

Step 2 — Enumeration
Dirb

Gobuster

Enum4linux

SMBclient

Step 3 — Exploitation
Metasploit

SQLmap

ExploitDB

Step 4 — Privilege Escalation
LinPEAS

SUID abuse

Kernel exploits

Step 5 — Post-Exploitation
Persistence

Extract hashes

Lateral movement

Step 6 — Reporting
Document findings.

11. Important Kali Tools and Their Use
11.1 Nmap
Port scanning & network mapping.

bash
Copy code
nmap -sV target
11.2 Metasploit
Exploit framework.

bash
Copy code
msfconsole
11.3 SQLmap
Automated SQL injection tool.

bash
Copy code
sqlmap -u URL --batch
11.4 Aircrack-ng
WiFi hacking suite.

11.5 Hydra
Password brute-forcing.

bash
Copy code
hydra -l user -P passlist.txt target ssh
12. Customizing Kali Linux
Change Wallpaper
Settings → Appearance.

Install New Themes
bash
Copy code
sudo apt install kali-themes
Add Tools Manually
bash
Copy code
git clone https://github.com/tool/tool.git
13. Tips for Beginners
Use a virtual machine to avoid damaging your system.

Take snapshots before testing tools.

Practice on legal environments (CTFs, labs, virtual boxes).

Learn Linux basics first.

Keep your system updated.

Always test ethically

