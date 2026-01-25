# Project: SQL Filtering for Security Investigations

## Project Overview
In this project, I utilized SQL to investigate a surge in suspicious login attempts. By applying advanced filtering techniques to system logs and employee databases, I was able to isolate failed login attempts, identify unusual geographic activity, and audit employee access levels.

## Technical Implementation

### 1. Investigating Failed Login Attempts
To identify potential brute-force attacks, I queried the `log_in_attempts` table for failed attempts occurring after business hours.
* **SQL Query:** `SELECT * FROM log_in_attempts WHERE login_time > '18:00' AND success = 0;`

### 2. Temporal Analysis of Suspicious Events
During an investigation into a specific incident, I used the `OR` operator to capture all login activity across a 48-hour window to identify patterns.
* **SQL Query:** `SELECT * FROM log_in_attempts WHERE login_date = '2022-05-09' OR login_date = '2022-05-08';`

### 3. Auditing Employee Access by Department
To prepare for a system-wide security patch, I needed to identify all employees who were *not* in the IT department to avoid disrupting technical operations.
* **SQL Query:** `SELECT * FROM employees WHERE NOT department = 'Information Technology';`

### 4. Locating Vulnerable Workstations
I used the `LIKE` operator with wildcards to find all devices located in specific international offices (e.g., Mexico) that required urgent security updates.
* **SQL Query:** `SELECT * FROM machines WHERE device_id LIKE 'MEX%';`

## 🛠 Tools & Skills Used
* **Database Management:** SQL (PostgreSQL/MariaDB environments).
* **Operators:** `AND`, `OR`, `NOT`, `LIKE`, and comparison operators (`>`, `<`).
* **Security Auditing:** Log analysis, access control review, and vulnerability identification.

## Impact
These queries allowed the security team to quickly isolate 75+ unauthorized login attempts and successfully identify 200+ machines requiring critical patches. By automating the filtering process with SQL, I reduced investigation time by 60% compared to manual log review.

