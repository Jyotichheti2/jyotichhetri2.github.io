# Project: PASTA Threat Modeling for E-commerce Application

## Project Overview
I conducted a comprehensive threat modeling exercise using the **PASTA (Process for Attack Simulation and Threat Analysis)** framework for a sneaker marketplace application. This risk-centric approach involved defining business objectives, technical scoping, and identifying potential vulnerabilities to develop a proactive security strategy.

## Threat Modeling Stages
### 1. Business & Technical Scoping
* **Objectives:** The application processes high-volume transactions between collectors and sellers, requiring strict adherence to **PCI DSS** and **SPII** regulations.
* **Tech Stack:** Utilizes APIs, Public Key Infrastructure (PKI), SHA-256 encryption, and SQL databases.

### 2. Threat & Vulnerability Analysis
* **Threat Profiles:** Identified both internal risks (DevSecOps data leaks) and external risks (competitors and global hackers exploiting system vulnerabilities).
* **Vulnerabilities:** Analyzed risks associated with the codebase and database, specifically identifying **Cross-Site Scripting (XSS)** as a high-priority vulnerability if encryption or access controls are bypassed.

### 3. Risk Analysis & Mitigation
I proposed a defense-in-depth strategy centered on four key security controls:
1. **Encryption:** Securing data-at-rest and data-in-transit.
2. **Injection Prevention:** Protecting the application from malicious input.
3. **Prepared Statements:** Ensuring database queries are handled securely to prevent SQL injection.
4. **Database Hardening:** Implementing strict access controls and regular auditing.

## 🛠 Tools & Skills Used
* **Frameworks:** PASTA (Risk-Centric Threat Modeling).
* **Compliance:** PCI DSS and SPII data protection standards.
* **Technical Analysis:** Identifying XSS, SQL injection risks, and PKI implementation.

## Impact
By applying the PASTA framework, I moved beyond simple vulnerability scanning to a holistic understanding of how technical threats impact business survival. This model ensures that security resources are prioritized for the application's most critical transaction paths and data entry points.
