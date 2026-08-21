# Project 05 — IAM & Access Control

## Objective

Implement and verify least-privilege identity and access controls on Linux.

## Environment and Tools

- Ubuntu Server
- Linux users and groups
- `chmod`, `chown`, and POSIX ACLs
- `sudoers` and restricted `systemctl` permissions
- Password aging, locking, unlocking, and account expiry

## Work Performed

- Created users and assigned role-appropriate ownership and permissions.
- Used ACLs to grant specific access without weakening the base permission model.
- Verified allowed and denied access with positive and negative tests.
- Confirmed that the Apache service account could read required content but could not write to protected locations.
- Restricted delegated administration to approved Apache restart and reload commands.
- Tested password aging, account expiry, lock and unlock behavior, and offboarding controls.
- Remediated two configuration gaps and repeated the validation tests.

## Outcome

Role separation and least privilege were successfully enforced. Authorized operations succeeded, unauthorized operations were denied, and no unresolved high-risk issue remained at closure.

## Skills Demonstrated

Identity lifecycle management, authorization design, ACLs, delegated administration, service-account security, control validation, remediation, and audit-ready documentation.

