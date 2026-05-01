## 🔬 Network Traffic Analysis - Wireshark Lab

![Wireshark](https://img.shields.io/badge/Wireshark-4.6.4-1679A7?style=flat&logo=wireshark&logoColor=white)
![Protocols](https://img.shields.io/badge/Protocols-DNS%20%7C%20HTTP%20%7C%20TLS-4CAF50?style=flat)
![Packets](https://img.shields.io/badge/Packets%20Captured-12%2C637-blueviolet?style=flat)

> Live capture and protocol-level analysis of 12,637 packets on a Windows Wi-Fi interface, with findings documented in a formal Network Traffic Analysis Report.

---

### Objective

Capture live network traffic, apply protocol-specific filters, and analyze DNS, HTTP, TLS, and external communications using Wireshark 4.6.4.

---

### Tools Used

| Tool | Purpose |
|------|---------|
| Wireshark 4.6.4 | Packet capture and analysis |
| Windows Wi-Fi interface | Live traffic source |
| `network_capture_lab.pcapng` | Raw packet capture file |

---

### What I Did

- Captured **12,637 live packets** on a Windows Wi-Fi interface
- Applied and analyzed four key display filters:
  - `dns` — DNS query/response behavior
  - `http` — HTTP request and response patterns
  - `tls` — Encrypted session characteristics and TLS handshakes
  - External traffic filter to isolate non-local IP communications
- Identified protocol behavior across layers
- Documented all findings in a formal PDF analysis report
- Included 7 annotated screenshots of each analysis stage

---

### Screenshots

| File | Description |
|------|------------|
| `09_wireshark_open.png` | Wireshark interface opened |
| `10_wireshark_capturing.png` | Live packet capture in progress |
| `11_wireshark_stopped.png` | Capture stopped at 12,637 packets |
| `12_filter_dns.png` | DNS filter applied |
| `13_filter_http.png` | HTTP filter applied |
| `14_filter_tls.png` | TLS filter applied |
| `15_filter_external.png` | External traffic isolated |

---

### Files

```
├── network_capture_lab.pcapng
├── Network_Analysis_Report_OluchiAdebanjo.pdf
└── screenshots/
    ├── 09_wireshark_open.png
    ├── 10_wireshark_capturing.png
    ├── 11_wireshark_stopped.png
    ├── 12_filter_dns.png
    ├── 13_filter_http.png
    ├── 14_filter_tls.png
    └── 15_filter_external.png
```

---

### Key Learning Outcomes

- Understanding of packet structure and protocol layers
- Ability to isolate traffic using Wireshark display filters
- Recognition of encrypted vs. unencrypted traffic
- Identification of DNS queries, HTTP requests, and TLS handshakes
- Improved familiarity with Wireshark's interface and analysis workflow
