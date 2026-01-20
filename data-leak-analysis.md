# Case Study: Data Leak Analysis & NIST CSF Implementation

## Project Overview
This analysis examines a real-world data leak scenario where confidential product and customer data were accidentally exposed. I applied the **NIST Cybersecurity Framework (CSF)** and **SP 800-53** guidelines to identify the root cause and propose corrective actions.

## Incident Investigation
* **Scenario:** Unauthorized public exposure of an internal-only folder containing unannounced product details and customer analytics.
* **Root Cause:** Excessive access permissions granted to a sales representative, violating the **Principle of Least Privilege (AC-6)**.

## Security Framework Alignment
This project aligns with the **NIST CSF "Protect" (PR.DS-5)** function, focusing on protections against data leaks through:
* **Least Privilege (AC-6):** Ensuring only the minimal authorization required for a task is provided.

## Recommended Controls
* **Technical:** Implement granular file-level permissions and data encryption to prevent unauthorized reading of leaked files.
* **Operational:** Establish automated workflows to revoke temporary access once a meeting or project is concluded.
* **Managerial:** Launch mandatory security awareness training specifically focused on secure data sharing and link-sharing protocols.
