# Project: SQL Filtering for Security Investigations

## Project Overview
In this project, I utilized SQL to investigate a surge in suspicious login attempts. By applying advanced filtering techniques to system logs and employee databases, I was able to isolate failed login attempts, identify unusual geographic activity, and audit employee access levels.

## Technical Implementation

### 1. Investigating Failed After-Hours Logins
To identify potential brute-force attacks occurring outside of business hours, I filtered for failed attempts (status 0) occurring after 18:00.
```sql
SELECT *
FROM log_in_attempts
WHERE TIME(login_time) > '18:00:00' AND status = 0;

### 2. Geographic Threat Hunting
To narrow the focus of the investigation, I excluded known-safe regions (Mexico) to isolate traffic from other global origins using wildcards and the NOT operator.
```sql
SELECT *
FROM log_in_attempts
WHERE country NOT LIKE 'Mex%';

### 3. 3. Employee Access Auditing
I performed audits on specific departments and office locations to verify access patterns, using both exact matches and the OR operator for broader searches.
```sql
-- Auditing Marketing employees in the East wing
SELECT *
FROM employees
WHERE department = 'Marketing' AND office LIKE 'East%';

-- Auditing Finance and Sales departments
SELECT *
FROM employees
WHERE department = 'Finance' OR department = 'Sales';
