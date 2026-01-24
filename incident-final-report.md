# Project: Cybersecurity Incident Report – Data Breach Investigation

## Project Overview
This project involved a comprehensive forensic investigation into a data breach affecting 50,000 customer records. I documented the attack timeline, identified the technical root cause (Forced Browsing), and proposed structural remediations to prevent future e-commerce vulnerabilities.

## Executive Summary
* **Incident Date:** December 28, 2022
* **Impact:** Unauthorized access to PII and financial data of ~50,000 customers.
* **Estimated Cost:** $100,000 (direct costs and potential revenue loss).
* **Status:** Resolved and remediated.

## Technical Investigation
### 1. Root Cause: Forced Browsing Attack
The investigation revealed a vulnerability in the organization's e-commerce web application. The attacker manipulated URL strings on purchase confirmation pages to access other customers' transaction data sequentially.
* **Evidence:** Web server logs showed an exceptionally high volume of sequential customer order requests from a single source.

### 2. Incident Timeline
* **Initial Threat:** December 22 – Phishing/Ransom email received by an employee (incorrectly flagged as spam).
* **Escalation:** December 28 – Second ransom demand received with a sample of stolen data.
* **Investigation:** December 28–31 – Forensic analysis of web application logs conducted by the security team.

## Response & Remediation
* **Public Disclosure:** Collaborated with PR to inform affected customers.
* **Customer Support:** Provided free identity protection services to impacted individuals.
* **Technical Fix:** Identified and patched the web application vulnerability.

## 🛠 Tools & Skills Used
* **Log Analysis:** Reviewing web server access logs for anomalous traffic patterns.
* **Vulnerability Assessment:** Identifying forced browsing and URL manipulation vulnerabilities.
* **Incident Documentation:** Formalizing technical findings into a professional executive report.

## Recommendations for Prevention
* **Access Control:** Implement URL allowlisting and enforce strict authentication for all sensitive content.
* **Proactive Testing:** Establish a schedule for routine vulnerability scans and penetration testing.
