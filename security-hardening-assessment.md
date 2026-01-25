# Project: Security Risk Assessment & System Hardening

## Project Overview
I conducted a security risk assessment to identify vulnerabilities and recommend hardening strategies for a corporate network. This project focuses on implementing proactive defense mechanisms, such as Next-Generation Firewalls and Intrusion Prevention Systems, to mitigate threats like DDoS attacks and unauthorized access.

## Proposed Hardening Strategies
I selected three primary hardening methods to strengthen the organization's security posture:

1.  **Next-Generation Firewall (NGFW):** Recommended to perform deep packet inspection and filter specific ports, protocols, and DNS traffic to prevent server collapse from "Ping of Death" or IP spoofing attacks.
2.  **Intrusion Prevention System (IPS):** Proposed as a critical layer to identify and automatically block anomalies, such as high volumes of sign-in requests from multiple sources during off-peak hours.
3.  **Data Encryption & MFA:** Recommended encrypting databases containing sensitive information and enforcing Multi-Factor Authentication (MFA) for all access points, including administrative accounts.

## Technical Justification
* **Defense in Depth:** Even if a firewall is bypassed, an IPS provides an additional security layer by detecting behavioral anomalies.
* **Zero Trust Principles:** Implementing network segmentation and MFA ensures that "all doors are not left open" for exploitation, even if an initial perimeter is breached.
* **Resource Protection:** Proper firewall configuration limits port exposure, protecting the server from resource exhaustion during volumetric attacks.

## 🛠 Tools & Skills Used
* **Network Security:** NGFW, IPS, and Port/Protocol Filtering.
* **System Hardening:** Database Encryption and MFA implementation.
* **Security Architecture:** Defense in Depth and Network Segmentation.

## Impact
This assessment provides a roadmap for transforming a reactive security setup into a proactive one. By implementing these hardening tools, the organization can significantly reduce the likelihood of successful DDoS attacks and ensure that sensitive data remains encrypted and inaccessible to unauthorized users.
