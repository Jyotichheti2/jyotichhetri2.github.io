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
