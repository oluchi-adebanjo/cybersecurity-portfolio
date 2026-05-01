**Cybersecurity Portfolio - Oluchi Adebanjo**

BSc Computer Science | Cybersecurity Diploma Student | CompTIA Security+ (June 2026)

Edmonton, Alberta | [LinkedIn URL:https://www.linkedin.com/in/oluchi-adebanjo-170301172/]


**Project 1:** Splunk SIEM - Live Threat Detection Lab

**Tools**: Splunk Enterprise, Windows Event Logs, PowerShell  
**Techniques:** MITRE ATT&CK T1136.001, T1098, T1053.005

**What I did**
- Installed and configured Splunk Enterprise on a Windows endpoint
- Ingested live Windows Security, System and Application Event Logs
- Simulated 3 real attacker techniques on my own machine:
  Created a rogue backdoor user account
  Escalated the account to the Administrators group
  Created a persistent scheduled task disguised as a Windows update
- Detected all 3 attacks in Splunk using custom SPL queries
- Documented findings in a formal Incident Investigation Report

Key Splunk detections
| EventCode | Description | Severity |
|-----------|-------------|----------|
| 4720 | New user account created | High |
| 4732 | Member added to Administrators group | High |
| 4698 | Scheduled task created | Medium |

**Files**
- `Incident_Report_OluchiAdebanjo.pdf` - Full investigation report
- Screenshots 01-07 - Evidence of detection

**Certifications In Progress**
- CompTIA Security+ - Exam scheduled June 2026
- Cybersecurity Diploma - Expected October 2026

**Learning Platforms**
- TryHackMe: (https://tryhackme.com/p/OluchiAdebanjo)]
