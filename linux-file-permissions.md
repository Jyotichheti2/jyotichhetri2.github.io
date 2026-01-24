# Project: Auditing & Modifying File Permissions in Linux

## Project Overview
In this project, I acted as a security professional responsible for ensuring that research team members had the correct system authorizations. I audited existing file permissions and utilized the Linux command line to revoke unauthorized access, thereby strengthening the organization's security posture.

## Technical Implementation
### 1. System Auditing
* **Command Usage:** Used `ls -l` and `ls -la` to display detailed permission strings for both visible and hidden files.
* **Analysis:** Interpreted 10-character permission strings to identify user, group, and other access levels (Read, Write, Execute).

### 2. Remediating Permissions
* **Action:** Utilized the `chmod` command to modify access.
* **Example:** I removed execute permissions from users and write permissions from groups where they were not required:
  `chmod u-x, g-w, o+r [filename]`

### 3. Handling Hidden Files & Directories
* **Navigation:** Used `pwd` and `cd` to locate target research directories.
* **Hidden Assets:** Identified and secured hidden files (prefixed with `.`) using specialized flags in the `ls` command.

## 🛠 Tools & Skills Used
* **Linux CLI:** `chmod`, `ls`, `cd`, `pwd`.
* **Access Control:** Managing Read (r), Write (w), and Execute (x) permissions.
* **Security Principles:** Implementing the Principle of Least Privilege and securing system authorizations.

## Impact
This audit identified and corrected multiple permission gaps, ensuring that only authorized researchers could modify sensitive files. This reduced the risk of accidental or malicious data modification within the organization's research environment.
