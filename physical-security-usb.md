# Project: Social Engineering Analysis – Physical Media Risks

## Project Overview
This project involved analyzing the risks associated with unauthorized physical media, specifically a "lost" USB drive found in a corporate parking lot. I evaluated the contents of the device, assessed how a threat actor could use the information for social engineering, and proposed technical and operational controls to mitigate these risks.

## Incident Analysis
### 1. Data Sensitivity & PII
* [cite_start]**Findings:** The device contained Personally Identifiable Information (PII) for multiple employees, including budget files and shift schedules.
* [cite_start]**Risk:** Storing sensitive work files alongside personal data on unencrypted mobile media creates a high risk of data leakage if the device is lost or stolen.

### 2. Attacker Mindset & Social Engineering
I analyzed how a threat actor could weaponize the discovered information:
* [cite_start]**Establishing Trust:** Information found can be used to impersonate colleagues or administrators to manipulate targets.
* [cite_start]**Phishing/Baiting:** Sensitive details can be used as "bait" to target relatives or employees for monetary gain or Sensitive PII (SPII).
* [cite_start]**System Access:** Data from the device provides a foundation for brute-force attacks against organizational systems.

## Risk Mitigation & Controls
* [cite_start]**Malicious Software:** Unauthorized devices may contain ransomware or rootkits designed to compromise systems upon connection.
* [cite_start]**Technical Controls:** Recommended the use of Virtual Machines (VMs) for analyzing unknown media to prevent direct host infection.
* [cite_start]**Operational Controls:** Proposed strict policies against connecting unauthorized USB devices and the implementation of endpoint protection to block unknown media.

## 🛠 Tools & Skills Used
* [cite_start]**Threat Modeling:** Analyzing attacker motivations and social engineering tactics.
* [cite_start]**Risk Assessment:** Evaluating the impact of physical security breaches on organizational data.
* [cite_start]**Security Policy:** Proposing managerial and technical controls to reduce the attack surface.
