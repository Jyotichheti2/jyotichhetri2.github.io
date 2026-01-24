# Project: Healthcare Network Access Control Automation (Python)

## Project Overview
This project involved developing a Python-based algorithm to automate the maintenance of an IP address allow list for a healthcare organization's restricted subnetwork. The goal was to ensure that only authorized employees could access sensitive patient records by automatically revoking access based on a "remove list."

## Technical Implementation
### 1. File Handling & Parsing
* **Safe Operations:** Used `with open()` context managers to handle file I/O operations, ensuring files were properly closed and resource leaks were prevented.
* **Data Transformation:** Utilized `.read()` to load file contents and `.split()` to convert space-separated IP address strings into a manageable Python list.

### 2. The Core Algorithm
The algorithm identifies and removes unauthorized IP addresses by comparing the current allow list against a predefined remove list.

```python
# Safe iteration over a copy of the list to ensure all matches are processed
for element in ip_addresses[:]:
    if element in remove_list:
        ip_addresses.remove(element)
```
## Tools & Skills Used

- **Python:** List manipulation, string parsing, and algorithm design.
- **File I/O:** Reading from and writing to text files using context managers.
- **Security Principles:** Implementing automated Least Privilege and Access Revocation.
