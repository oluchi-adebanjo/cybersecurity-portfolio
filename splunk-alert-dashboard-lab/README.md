## 📊 Splunk Alert Rules & Security Dashboard

![Splunk](https://img.shields.io/badge/Splunk-Enterprise-FF5733?style=flat&logo=splunk&logoColor=white)
![SPL](https://img.shields.io/badge/SPL-Alert%20Rules-blueviolet?style=flat)
![Windows](https://img.shields.io/badge/Windows-Event%20Logs-0078D6?style=flat&logo=windows&logoColor=white)

> Automated real-time alerting and security monitoring dashboard built in Splunk Enterprise.

---

### Objective

To design and implement real-time alert rules for critical Windows security events and build a live security dashboard that visualizes authentication activity, high-priority events, and overall system behavior.

---

### Tools Used

| Tool | Purpose |
|------|---------|
| Splunk Enterprise | Alert engine and dashboard platform |
| Windows Event Logs | Log data source |
| SPL (Search Processing Language) | Query and alert logic |

---

### Alert Rules Created

| Alert Name | EventCode | Severity | Purpose |
|------------|-----------|----------|---------|
| New Local User Account Created | 4720 | High | Detects unauthorized or suspicious account creation |
| Member Added to Administrators Group | 4732 | Critical | Detects privilege escalation or account manipulation |

These alerts were configured to trigger in real time and generate notifications when malicious or suspicious activity occurred.

---

### Security Dashboard Panels

**1. Login Activity (Successful vs Failed)**
A column chart visualizing authentication patterns to identify brute-force attempts, unusual login spikes, or failed login bursts.

**2. Top Security Event Codes**
A pie chart showing the most frequent security-related EventCodes, helping highlight recurring or high-volume events.

**3. Recent High-Priority Security Events**
A table listing the latest critical and high-severity events, enabling quick triage and investigation.

---

### Screenshots

| File | Description |
|------|-------------|
| `01_splunk_restarted.png` | Splunk service restarted |
| `02_alert1_created.png` | Alert rule for EventCode 4720 created |
| `03_alert2_created.png` | Alert rule for EventCode 4732 created |
| `04_alerts_triggered.png` | Alerts firing after simulated attacks |
| `05_security_dashboard.png` | Full dashboard view |
| `05_security_dashboard_top.png` | Dashboard top section |
| `05_security_dashboard_bottom.png` | Dashboard bottom section |

These screenshots demonstrate the full workflow: alert creation, alert triggering, and dashboard visualization.

---

### Key Learning Outcomes

- Ability to build real-time alert rules in Splunk
- Understanding of critical Windows EventCodes related to account creation and privilege escalation
- Skill in designing security dashboards for monitoring authentication and system activity
- Experience translating raw logs into actionable security insights
- Familiarity with SPL for filtering, correlating, and visualizing events
