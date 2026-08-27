# Project 04 — Linux Web Server Security

## Objective

Deploy an Ubuntu Apache web service, validate availability, and reduce unnecessary information exposure.

## Environment and Tools

- Ubuntu Server and Apache HTTP Server
- systemd and journal/service validation
- netplan and Host-Only networking
- Linux permissions and configuration files

## Work Performed

- Configured the server network interface for the lab environment.
- Deployed Apache and verified that the service was active.
- Confirmed HTTP accessibility and a successful HTTP 200 response.
- Used Apache configuration validation before applying changes.
- Reduced the server banner so that it exposed Apache without detailed version or operating-system information.
- Re-tested service state and web accessibility after hardening.

## Outcome

The server remained reachable and functional after hardening, with reduced banner disclosure and repeatable validation steps.

## Skills Demonstrated

Linux administration, network configuration, web-service deployment, service troubleshooting, secure configuration, change validation, and documentation.

## Project Evidence

📸 [View screenshots and supporting evidence](evidence/README.md)
