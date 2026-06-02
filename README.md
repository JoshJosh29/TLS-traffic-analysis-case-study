# TLS Traffic Analysis and Malware Detection with Wireshark
## Overview
This project documents a network traffic investigation where encrypted HTTPS/TLS traffic was analyzed and decrypted to identify a malicious file download.
## Objectives
- Analyze TLS traffic in Wireshark
- Decrypt encrypted communications using session keys
- Extract files from network traffic
- Investigate suspicious files with VirusTotal
- Identify the affected host
## Investigation Process
### Step 1: Traffic Analysis
- Filtered HTTP GET requests and TLS handshake traffic.
- Identified suspicious communication between a source IP and destination IP.
- Observed a request for an `invest.tll` file.
### Step 2: TLS Decryption
- Followed the TLS stream.
- Used the provided TLS session keys from the PCAP file.
- Successfully decrypted the encrypted traffic.
### Step 3: File Extraction
- Extracted and saved the downloaded file from the network capture.
### Step 4: Malware Verification
- Submitted the extracted file to VirusTotal.
- Multiple security vendors flagged the file as malicious.
- Detection results classified the file as a Trojan.
## Findings
- The system downloaded a malicious file.
- The file was identified as a Trojan by several security vendors.
- The affected host was identified through network traffic analysis.
## Lessons Learned
- Decrypting TLS traffic using session keys in Wireshark.
- Extracting files from network captures.
- Using VirusTotal for malware investigation.
- Identifying compromised systems through network traffic.
## Tools Used
- Wireshark
- VirusTotal
- PCAP Analysis
## Skills Demonstrated
- Network Traffic Analysis
- Threat Hunting
- Incident Response
- Malware Investigation
- Packet Analysis
