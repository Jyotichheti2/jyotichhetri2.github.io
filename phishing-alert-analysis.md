# Incident Analysis: Phishing & Malware Investigation

## Project Overview
In this lab, I acted as a Tier 1 SOC Analyst to investigate a suspicious email alert. I performed header analysis, extracted a file hash, and used threat intelligence tools to confirm the presence of malware, leading to a successful escalation.

## Incident Ticket Summary
| Field | Details |
| :--- | :--- |
| **Ticket ID** | A-2703 |
| **Alert Message** | SERVER-MAIL: Potential Phishing & Malware Download |
| **Severity** | Medium |
| **Status** | Escalated to SOC Tier 2 |

## Investigation Details
### 1. Email Header & Content Analysis
* **Sender:** `Def Communications <76tguyhh6tgftrt7tg.su>` (Suspicious domain).
* **Subject:** `Re: Infrastructure Egnieer role` (Includes misspellings).
* **Red Flags:** The email requested the user to open a password-protected attachment (`bfsvc.exe`), a common tactic used to bypass automated email scanners.

### 2. Technical Malware Analysis
* **Action taken:** Generated a SHA256 hash value of the attachment in a virtual environment.
* **Artifact:** `54e6ea47eb04634d3e87fd7787e2136ccfbcc80ade34f246a12cf93bab527f6b`.
* **Tool:** VirusTotal confirmed the hash as malicious.

## Conclusion & Recommendation
The incident was escalated due to confirmed malware. 
* **Recommendation:** Implement email filtering rules to block the sender's domain and run a full system scan on the recipient's workstation (`hr@inergy.com`).

---

## 🛠 Tools Used
* **VirusTotal:** Utilized for reputation analysis and hash verification against global threat intelligence databases.
* **CyberChef:** Used for decoding and deobfuscating suspicious strings within the email headers.
* **Linux Terminal:** Employed to safely generate SHA256 checksums for file integrity and identification.
