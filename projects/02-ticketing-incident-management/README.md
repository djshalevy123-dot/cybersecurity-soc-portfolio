# Project 02 — Ticketing & Incident Management

## Objective

Apply a documented incident lifecycle from detection through investigation, response decision, and closure.

## Incident Summary

- Ticket: **INC-2026-001**
- Alert: **Suspicious PowerShell ExecutionPolicy Bypass**
- Classification: **True Positive — Authorized Lab Test**
- Severity / priority: **Low / P2**
- Detection delay: **45.95 seconds**
- SLA target: **4 hours**
- Lifecycle duration: approximately **40 minutes**

## Investigation

- Reviewed the alert result and affected endpoint.
- Correlated Sysmon events 1, 11, and 5 by process context.
- Reviewed the script content and calculated its SHA-256 hash.
- Confirmed that the script only executed a benign `Write-Output` command.
- Checked the correlated activity for network connections and found no Sysmon Event ID 3 associated with the test process.

## Analyst Decision

The alert logic correctly identified suspicious syntax. The activity was an authorized lab test, so containment and remediation were not required. Evidence, reasoning, SLA performance, and closure details were recorded in the incident ticket.

## Skills Demonstrated

Alert triage, evidence preservation, event correlation, severity and priority assignment, SLA tracking, analyst decision-making, timeline construction, and professional closure documentation.

