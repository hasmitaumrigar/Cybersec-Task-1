# Cybersec-Task-1
Objective:
The objective of this task is to discover open ports on devices in the local network using Nmap in order to understand network exposure and basic network reconnaissance techniques.

Tools Used:
Nmap

## Step 1: Install Nmap
Nmap was downloaded and installed from the official website:
https://nmap.org

Installation was verified using:
nmap --version

## Step 2: Find Local IP Range
Command used
ipconfig

## Step 3: Perform Nmap Scan
Command used: (Example)
nmap -sS 10.175.254.0/24

Explanation:
-sS performs a TCP SYN (half-open) scan.
It scans all devices in the local network range.
It identifies open TCP ports.

## Step 4: Analyze Results
The scan output shows:
Active hosts
Open ports
Services running on those ports

## Example output format:
PORT   STATE  SERVICE
80/tcp open   http
22/tcp open   ssh

Open ports indicate that services are actively accepting connections.

## Step 5: Optional Packet Analysis
Wireshark can be used to capture packets during the scan to observe:
SYN packets sent by Nmap
SYN-ACK or RST responses
TCP handshake behavior

## Step 6: Identify Security Risks
Open ports may expose services to:
Unauthorized access
Brute-force attacks
Exploitation of vulnerabilities
Malware attacks
Unused services should be disabled and protected using firewall rules.
