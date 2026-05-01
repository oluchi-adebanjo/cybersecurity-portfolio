## 🛡️ Splunk SIEM - Live Threat Detection Lab

![Splunk](https://img.shields.io/badge/Splunk-Enterprise-FF5733?style=flat&logo=splunk&logoColor=white)
![MITRE ATT&CK](https://img.shields.io/badge/MITRE%20ATT%26CK-3%20Techniques-red?style=flat)
![Windows](https://img.shields.io/badge/Windows-Event%20Logs-0078D6?style=flat&logo=windows&logoColor=white)

> Live threat detection and log analysis using Splunk Enterprise and Windows Event Logs.

---

### Objective

To simulate real attacker behaviors on a Windows endpoint, ingest the resulting logs into Splunk Enterprise, and detect malicious activity using custom SPL queries mapped to MITRE ATT&CK techniques.

---

### Tools Used

| Tool | Purpose |
|------|---------|
| Splunk Enterprise (Free) | Log ingestion and threat detection |
| Windows Event Logs | Security, System, and Application log sources |
| PowerShell | Attack simulation |
| MITRE ATT&CK Framework | Technique mapping and documentation |

---

### What I Did

- Installed and configured Splunk Enterprise on a Windows endpoint
- Ingested live Windows Security, System, and Application logs
- Simulated three attacker techniques aligned with MITRE ATT&CK:
  - Created a rogue local backdoor user account
  - Added the account to the Administrators group
  - Created a persistent scheduled task disguised as a Windows update
- Wrote custom SPL queries to detect each malicious action
- Documented all findings in a formal Incident Investigation Report (PDF)

---

### MITRE ATT&CK Techniques Simulated

| Technique ID | Technique Name | Description |
|--------------|---------------|-------------|
| T1136.001 | Create Local Account | Adversary creates a new local user for persistence or privilege escalation |
| T1098 | Account Manipulation | Adding user to privileged groups to escalate access |
| T1053.005 | Scheduled Task | Creating scheduled tasks for persistence |

---

### Key Splunk Detections

| EventCode | Description | Severity |
|-----------|-------------|----------|
| 4720 | New user account created | High |
| 4732 | User added to Administrators group | High |
| 4698 | Scheduled task created | Medium |

These detections confirm that Splunk successfully captured and surfaced the malicious activity generated during the simulation.

---

### Files

```
├── Incident_Report_OluchiAdebanjo.pdf
└── screenshots/
    ├── 01 — 07 (detection evidence and SPL queries)
```

---

### Key Learning Outcomes

- Ability to configure Splunk for endpoint log ingestion
- Understanding of Windows Event Log artifacts for account creation, privilege escalation, and persistence
- Skill in writing SPL queries to detect malicious behavior
- Experience mapping detections to MITRE ATT&CK
- Improved documentation and incident reporting skills
