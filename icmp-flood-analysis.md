# Project: ICMP Flood DDoS Attack Analysis (NIST Framework)

## Project Overview
I analyzed a network security incident where an unconfigured firewall allowed an abnormal volume of incoming ICMP packets, resulting in a DDoS attack that disrupted employee login services. Using the **NIST Cybersecurity Framework**, I documented the identification, protection, detection, response, and recovery phases of the incident.

## NIST Framework Analysis
### 1. Identify
* **Incident:** Employees reported network service failures.  A network sniffing test identified a flood of ICMP pings, confirming a **DDoS attack**.

### 2. Protect
*  **Technical Controls:** Configured the Firewall and **IPS** to limit ICMP traffic and block malicious source IP addresses.
*  **Operational Controls:** Trained team members on secure data practices, including **MFA**, VPN usage, and credential management.

### 3. Detect
*  **Vulnerability Management:** Implemented continuous network sniffing tests and deployed an **IDS** to identify suspicious traffic patterns and vulnerabilities.

### 4. Respond
*  **Containment & Remediation:** Stopped non-essential services, configured the IPS to block insecure protocols, and recorded the incident as a case study for future training.

### 5. Recover
*  **Restoration:** Restored the system to the latest clean backup and increased the frequency of backup practices to minimize future data loss.

## 🛠 Tools & Skills Used
*  **Security Frameworks:** NIST Cybersecurity Framework.
*  **Network Security Tools:** Firewall configuration, IDS/IPS, and Network Sniffing.
*  **Incident Response:** Threat identification, remediation, and post-mortem analysis.

## Impact
This project demonstrates my ability to handle a high-pressure network security event by applying industry-standard frameworks.  By implementing technical controls like IP verification and IDS filtering, the organization moved from a vulnerable state to a more resilient security posture.
