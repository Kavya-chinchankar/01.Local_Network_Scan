Cyber Security Internship – Task 1

Scan Your Local Network for Open Ports


---

📘 Objective

The goal of this task is to learn network reconnaissance by scanning a local network to identify open ports and services using Nmap. This helps understand how network exposure can lead to potential security risks.


---

🧰 Tools Used

Nmap – for network and port scanning

Command Prompt (Windows) – to find local IP and run commands

Wireshark (optional) – for packet analysis



---

⚙ Steps I Followed

1. Installed Nmap from the official Nmap website.


2. Opened Command Prompt and used:

ipconfig

to find my local IP address and network range (e.g., 192.168.1.0/24).


3. Performed a TCP SYN Scan using the command:

nmap -sS 192.168.1.0/24


4. Analyzed the Scan Results to identify:

Active devices on the network

Open ports and running services

5. Saved the scan output as a text/HTML file for submission.




---

📊 Example Output

Starting Nmap 7.98 ( https://nmap.org ) at 2025-10-20 20:53 +0530
NSE: Loaded 158 scripts for scanning.
NSE: Script Pre-scanning.
Initiating NSE at 20:53
Completed NSE at 20:53, 0.00s elapsed
Initiating NSE at 20:53
Completed NSE at 20:53, 0.00s elapsed
Initiating NSE at 20:53
Completed NSE at 20:53, 0.00s elapsed
Initiating Parallel DNS resolution of 1 host. at 20:53
Completed Parallel DNS resolution of 1 host. at 20:53, 1.51s elapsed
Initiating SYN Stealth Scan at 20:53
Scanning 192.168.56.1 [1000 ports]
Discovered open port 135/tcp on 192.168.56.1
Discovered open port 445/tcp on 192.168.56.1
Discovered open port 139/tcp on 192.168.56.1
Discovered open port 5357/tcp on 192.168.56.1
Completed SYN Stealth Scan at 20:53, 0.15s elapsed (1000 total ports)
Initiating Service scan at 20:53
Scanning 4 services on 192.168.56.1
Completed Service scan at 20:53, 11.07s elapsed (4 services on 1 host)
Initiating OS detection (try #1) against 192.168.56.1
NSE: Script scanning 192.168.56.1.
Initiating NSE at 20:53
Completed NSE at 20:53, 14.32s elapsed
Initiating NSE at 20:53
Completed NSE at 20:53, 0.05s elapsed
Initiating NSE at 20:53
Completed NSE at 20:53, 0.00s elapsed
Nmap scan report for 192.168.56.1
Host is up (0.00038s latency).
Not shown: 996 closed tcp ports (reset)
PORT     STATE SERVICE       VERSION
135/tcp  open  msrpc         Microsoft Windows RPC
139/tcp  open  netbios-ssn   Microsoft Windows netbios-ssn
445/tcp  open  microsoft-ds?
5357/tcp open  http          Microsoft HTTPAPI httpd 2.0 (SSDP/UPnP)
|_http-title: Service Unavailable
|_http-server-header: Microsoft-HTTPAPI/2.0
Device type: general purpose
Running: Microsoft Windows 10
OS CPE: cpe:/o:microsoft:windows_10
OS details: Microsoft Windows 10 1809 - 21H2
Network Distance: 0 hops
TCP Sequence Prediction: Difficulty=252 (Good luck!)
IP ID Sequence Generation: Incremental
Service Info: OS: Windows; CPE: cpe:/o:microsoft:windows

Host script results:
| smb2-security-mode: 
|   3.1.1: 
|_    Message signing enabled but not required
| smb2-time: 
|   date: 2025-10-20T15:23:36
|_  start_date: N/A

NSE: Script Post-scanning.
Initiating NSE at 20:53
Completed NSE at 20:53, 0.00s elapsed
Initiating NSE at 20:53
Completed NSE at 20:53, 0.00s elapsed
Initiating NSE at 20:53
Completed NSE at 20:53, 0.00s elapsed
Read data files from: C:\Program Files (x86)\Nmap
OS and Service detection performed. Please report any incorrect results at https://nmap.org/submit/ .
Nmap done: 1 IP address (1 host up) scanned in 29.73 seconds
           Raw packets sent: 1016 (45.418KB) | Rcvd: 2044 (87.206KB)



---

🔍 Key Concepts Learned

What open ports are and how they expose services

How TCP SYN scanning works

Difference between TCP and UDP scans

Basic understanding of network reconnaissance

---

🧠 Interview Questions & Answers

1. What is an open port?
→ An open port is a communication endpoint that listens for incoming network traffic.


2. How does Nmap perform a TCP SYN scan?
→ It sends a SYN packet and waits for a response (SYN-ACK). It doesn’t complete the handshake, making it a stealthy scan.


3. What risks are associated with open ports?
→ Attackers can exploit services running on open ports to gain unauthorized access.


4. How can open ports be secured?
→ By closing unused ports, using firewalls, and configuring access control rules.

---

🖼 Screenshots








---

🚀 Outcome

Gained hands-on experience in basic network reconnaissance.

Learned how to identify and interpret open ports and services.

Understood how Nmap and Wireshark complement each other for network analysis.



---

