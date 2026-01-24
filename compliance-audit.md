# Project: Controls & Compliance Audit – Botium Toys

## Project Overview
As part of my Foundations of Cybersecurity coursework, I conducted a comprehensive security audit for Botium Toys. This project involved assessing the organization's current security posture, identifying critical gaps in internal controls, and evaluating alignment with global compliance standards like PCI DSS, GDPR, and SOC.



## ✅ Controls Assessment & Gap Analysis

| Control Category | Status | Recommendations |
|:--- |:--- |:--- |
| **Least Privilege** | ❌ Not in place | Enforce access control based on specific job roles. |
| **Separation of Duties** | ❌ Not in place | Divide responsibilities to reduce insider threat risks. |
| **Encryption (PII/SPII)** | ❌ Missing | Implement AES encryption for sensitive customer data. |
| **Intrusion Detection (IDS)**| ❌ Missing | Deploy network-based IDS for real-time monitoring. |
| **Disaster Recovery** | ❌ Missing | Develop a formal DR plan and regular backup testing. |
| **Physical Security** | ✅ Implemented | Maintain existing CCTV and physical locking mechanisms. |

## 📜 Compliance Alignment

### PCI DSS (Payment Card)
* **Gap:** Lack of encryption for credit card transactions and weak password rotation.
* **Action:** Implement a centralized password management system and end-to-end encryption.

### GDPR (Privacy)
* **Gap:** No formal 72-hour breach notification procedure or data inventory.
* **Action:** Establish a data classification framework and Incident Response Plan.

### SOC 2 (Trust Services)
* **Gap:** Incomplete data integrity controls and weak user access policies.
* **Action:** Strengthen identity and access management (IAM) protocols.

## 🛠 Tools & Skills Used
* **Framework Alignment:** NIST CSF, PCI DSS, GDPR, and SOC 1/SOC 2.
* **Risk Management:** Gap analysis, internal control assessment, and threat identification.
* **Security Auditing:** Evaluating physical, technical, and administrative controls.

## Impact
By identifying these 8 critical security gaps, I provided Botium Toys with a roadmap to move from a high-risk state to a compliant, resilient security posture. This audit ensures the organization meets legal requirements and protects customer trust. 

## ✅ Technical Control Gap Analysis

| Security Control | Finding | Technical Recommendation |
|:--- |:--- |:--- |
| **Identity & Access Management** | Lack of Least Privilege | Implement Role-Based Access Control (RBAC) to restrict PII access. |
| **Data Security** | Missing Encryption | Deploy AES-256 encryption for data at rest and in transit. |
| **Network Monitoring** | No IDS/SIEM | Deploy an Intrusion Detection System to monitor for lateral movement. |
| **Business Continuity** | No DR Plan | Establish a RTO/RPO-based Disaster Recovery and backup policy. |
