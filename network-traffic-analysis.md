# Project: Cybersecurity Incident Report – Network Traffic Analysis

## Project Overview
In this incident response simulation, I analyzed network traffic logs to identify the cause of a website connection timeout. I performed forensic analysis on TCP/UDP traffic and documented the mechanics of a SYN flood attack to provide actionable remediation strategies.

## Incident Summary
* **Attack Type:** SYN Flood Denial of Service (DoS) with IP Spoofing.
* **Impact:** The web server was unable to complete the TCP three-way handshake for legitimate users, leading to service timeouts.
* **Key Findings:** Packet sniffing revealed a massive influx of SYN requests in a short interval, most resulting in "RST" (reset) or failure to complete the connection.

## Technical Analysis
### 1. The TCP Three-Way Handshake Breakdown
* **Step 1 (SYN):** The client sends a synchronization request.
* **Step 2 (SYN/ACK):** The server acknowledges and grants permission to communicate.
* **Step 3 (ACK):** The client acknowledges, and the connection is established.
* **The Attack:** The threat actor flooded the server with Step 1 requests but never completed the handshake, exhausting server resources and blocking legitimate traffic.

### 2. Network Protocol Investigation
* **DNS Issues:** Investigation found that UDP port 53 (DNS) became unreachable, preventing the conversion of domain names to IP addresses.
* **Port Monitoring:** Abnormal traffic was detected on port 443 (HTTPS), indicating an attempt to disrupt encrypted communications.

## 🛠 Tools & Skills Used
* **Network Analysis:** tcpdump, Wireshark (packet sniffing).
* **Protocols:** TCP/IP, UDP, ICMP, DNS (Port 53), HTTPS (Port 443).
* **Incident Response:** Threat identification, risk mitigation, and system recovery.

## Impact
My analysis allowed the IT team to identify the specific attack vector and mitigate the risk by isolating affected systems. This prevented further service degradation and helped establish a baseline for improved firewall rules to filter spoofed IP traffic.
