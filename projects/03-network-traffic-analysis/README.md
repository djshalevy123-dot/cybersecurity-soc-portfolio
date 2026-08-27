# Project 03 — Network Traffic Analysis with Wireshark

## Objective

Use packet evidence to identify reconnaissance activity and determine whether the traffic progressed into a compromise.

## Environment and Tools

- Wireshark and PCAP analysis
- Kali Linux and Windows endpoints
- Nmap
- TCP/IP, DNS, HTTP, and TCP flag analysis

## Work Performed

- Captured and reviewed normal DNS, HTTP, and TCP three-way handshake traffic.
- Identified repeated SYN attempts and RST/ACK responses consistent with port scanning.
- Traced traffic between the lab source and destination systems.
- Reviewed activity involving ports 135, 139, and 445.
- Searched for follow-on sessions or evidence of successful exploitation.

## Outcome

The capture contained clear reconnaissance indicators, but no evidence of post-scan compromise was identified in the available PCAP.

## Skills Demonstrated

Capture filtering, endpoint identification, TCP flag interpretation, scan analysis, timeline reasoning, and evidence-based conclusions with appropriate limitations.

## Project Evidence

📸 [View screenshots and supporting evidence](evidence/README.md)
