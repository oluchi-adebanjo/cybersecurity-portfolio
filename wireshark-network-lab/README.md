
Live network traffic capture and protocol analysis using Wireshark 4.6.4.

Objective
To capture live network traffic, apply protocol‑specific filters, and analyze DNS, HTTP, TLS, and external communications. Findings were documented in a formal Network Traffic Analysis Report.

Tools Used
Wireshark 4.6.4

Windows Wi‑Fi interface

PCAPNG capture file (network_capture_lab.pcapng)

What I Did
Captured 12,637 live packets on a Windows Wi‑Fi interface

Applied and analyzed four key display filters:

DNS (dns)

HTTP (http)

TLS (tls)

External traffic (non‑local IPs)

Identified protocol behavior, request/response patterns, and encrypted session characteristics

Documented findings in a formal Network Traffic Analysis Report (PDF)

Included screenshots showing each stage of the analysis
Screenshots Included
These images demonstrate the workflow and analysis steps:

09_wireshark_open.png — Wireshark interface opened

10_wireshark_capturing.png — Live packet capture in progress

11_wireshark_stopped.png — Capture stopped at 12,637 packets

12_filter_dns.png — DNS filter applied

13_filter_http.png — HTTP filter applied

14_filter_tls.png — TLS filter applied

15_filter_external.png — External traffic isolated

 Files
network_capture_lab.pcapng — Raw packet capture

Network_Analysis_Report_OluchiAdebanjo.pdf — Full analysis report

Screenshots 09–15 — Evidence of filtering and analysis

Key Learning Outcomes
Understanding of packet structure and protocol layers

Ability to isolate traffic using display filters

Recognition of encrypted vs unencrypted traffic

Identification of DNS queries, HTTP requests, and TLS handshakes

Improved familiarity with Wireshark’s interface and analysis workflow
