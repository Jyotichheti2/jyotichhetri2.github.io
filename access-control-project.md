# Case Study: Access Control & Incident Remediation

## Project Overview
This project involved analyzing a security incident where a former contractor accessed sensitive systems using administrative credentials. I identified the authorization gaps and recommended specific security controls to prevent future unauthorized access.

## Incident Analysis
* **User:** Robert Taylor Jr.
* **Timestamp:** October 3, 2023, 08:27 AM
* **Workstation:** Up2-NoGud
* **Issue:** The user was a contractor whose account remained active with administrative privileges after their contract ended.

## Recommended Controls
### 1. Technical Controls
* **Principle of Least Privilege (PoLP):** Restrict administrative access to authorized full-time personnel only.
* **Automated Disabling:** Use IAM tools to automatically disable accounts on the contract end date.

### 2. Operational Controls
* **Offboarding Checklist:** Implement a mandatory IT verification step for all departing contractors.

### 3. Managerial Controls
* **Access Reviews:** Conduct quarterly audits to identify and remove "stale" accounts.
