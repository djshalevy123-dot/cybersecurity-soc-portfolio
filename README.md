# Cybersecurity & SOC Analyst Portfolio

**Shalev Yehosua**  
Target role: **SOC Tier 1 / Junior Security Analyst**

This repository presents five hands-on cybersecurity projects completed in an isolated and authorized lab. The portfolio follows an end-to-end analyst workflow: collect telemetry, detect suspicious activity, investigate evidence, make a decision, respond, and document the outcome.

## Portfolio at a Glance

| # | Project | Core tools | Verified outcome |
|---|---|---|---|
| 01 | [SIEM Detection Engineering](projects/01-siem-detection-engineering/) | Splunk, Sysmon, Universal Forwarder, PowerShell | Onboarded Windows telemetry and built a scheduled detection for PowerShell `ExecutionPolicy Bypass`. |
| 02 | [Ticketing & Incident Management](projects/02-ticketing-incident-management/) | Splunk alerting, incident ticket, timeline, evidence review | Investigated INC-2026-001, met the SLA, and closed an authorized true positive with a documented rationale. |
| 03 | [Network Traffic Analysis](projects/03-network-traffic-analysis/) | Wireshark, PCAP, Nmap, TCP/IP | Identified scan activity involving ports 135, 139, and 445 and found no evidence of post-scan compromise. |
| 04 | [Linux Web Server Security](projects/04-linux-web-server-security/) | Ubuntu Server, Apache, systemd, netplan | Deployed and hardened a reachable Apache service with repeatable validation checks. |
| 05 | [IAM & Access Control](projects/05-iam-access-control/) | Linux ACLs, sudoers, password aging, user lifecycle | Implemented least privilege and verified access with positive and negative authorization tests. |

## Featured Case Study — INC-2026-001

A Splunk scheduled alert detected PowerShell execution with the `ExecutionPolicy Bypass` argument. The investigation correlated Sysmon events, reviewed the script contents and SHA-256 hash, checked for network activity, and documented the full incident lifecycle.

- Classification: **True Positive — Authorized Lab Test**
- Severity / priority: **Low / P2**
- Detection delay: **45.95 seconds**
- Incident lifecycle: approximately **40 minutes**
- Related Sysmon events: **1, 11, and 5**
- Final decision: no containment or remediation was required because the activity was authorized and isolated

## Skills Demonstrated

- SIEM onboarding, search, correlation, scheduled alerts, and validation
- Windows Security and Sysmon event analysis
- Incident triage, severity and priority assignment, evidence handling, and closure
- PCAP filtering and network indicator interpretation
- Linux service deployment, validation, and security hardening
- Identity lifecycle management, ACLs, restricted sudo, and least privilege
- Professional reporting in English and Hebrew

## Documentation

- [English Portfolio Overview](docs/Shalev_Yehosua_Cybersecurity_Portfolio_Overview_EN.docx)
- [Hebrew Portfolio Overview](docs/Shalev_Yehosua_Cybersecurity_Portfolio_Overview_HE.docx)
- [Hebrew repository guide](README_HE.md)
- [Public publication checklist](PUBLICATION_CHECKLIST.md)

## Lab Architecture

The lab used Windows 10, Kali Linux, Ubuntu Server, and Windows Server virtual machines in VirtualBox. NAT, Internal Network, and Host-Only networking were used according to the exercise. Splunk Enterprise ran as the SIEM platform, with Windows telemetry forwarded from the endpoint.

## Ethical Use

All activities were performed in systems owned or controlled by the author. No unauthorized systems were targeted. Commands and configurations are included only for defensive learning, detection engineering, and incident-response practice.

