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


How I ran the scan

1. Found local IP / network (example):

ipconfig


2. Performed a SYN scan and service/OS detection with Nmap:

nmap -sS -A 192.168.56.1

(Replace 192.168.56.1 with the target IP / IP range you want to scan.)




---

Raw Nmap Output

Starting Nmap 7.98 ( https://nmap.org ) at 2025-10-20 20:53 +0530
NSE: Loaded 158 scripts for scanning.
NSE: Script Pre-scanning
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


🖼 Screenshots








---

🚀 Outcome

Gained hands-on experience in basic network reconnaissance.

Learned how to identify and interpret open ports and services.

Understood how Nmap and Wireshark complement each other for network analysis.



---

