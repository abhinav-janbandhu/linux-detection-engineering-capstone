# Detection Rules

## Web Enumeration Detection

IF:
- Large volume of HTTP requests
- Majority are 404 responses
- User-Agent contains Gobuster

THEN:
Alert: Directory Enumeration Activity

---

## SSH Brute Force Detection

IF:
- Failed SSH logins >= 3
- Same source IP
- Within short time period

THEN:
Alert: SSH Brute Force Attempt

---

## Suspicious Artifact Detection

IF:
- Hidden directories created
- Unexpected files appear in user home directories

THEN:
Alert: Potential Persistence Activity
