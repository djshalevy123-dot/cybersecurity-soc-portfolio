# Project 01 — SIEM Detection Engineering

## Objective

Build endpoint visibility in Splunk and create a repeatable detection workflow for suspicious PowerShell execution.

## Environment and Tools

- Splunk Enterprise and Search & Reporting
- Splunk Universal Forwarder 10.4.2
- Sysmon 15.21
- Windows Event Viewer and PowerShell
- Windows 10 endpoint in VirtualBox

## Work Performed

- Configured TCP receiving on port 9997 and validated connectivity from the endpoint.
- Forwarded Application, Security, System, and Sysmon Operational logs.
- Verified Windows Security event IDs including 4624, 4648, 4672, and 4616.
- Installed Sysmon with a validated XML configuration.
- Correlated Sysmon process creation, file creation, and process termination events.
- Created a scheduled Splunk alert for PowerShell `ExecutionPolicy Bypass` execution.

## Outcome

The SIEM successfully detected the test PowerShell command and preserved the evidence required for investigation. The resulting alert became the detection source for INC-2026-001.

## Evidence Highlights

- Sysmon Event ID 1 — process creation
- Sysmon Event ID 11 — file creation
- Sysmon Event ID 5 — process termination
- Successful TCP test to the Splunk receiver on port 9997
- Triggered Splunk scheduled alert

## Skills Demonstrated

SIEM onboarding, Windows telemetry, SPL searches, XML field extraction, correlation, alert creation, troubleshooting, and detection validation.

## Project Evidence

📸 [View screenshots and supporting evidence](evidence/README.md)
