# Scope of Work: Isolated Vulnerable Web Application Lab

**Document version:** 1.0
**Date:** 22 November 2026
**Prepared by:** Lab owner (student)

## 1. Purpose

This document defines the legal and technical boundaries for security testing practice in a personal lab. It exists to ensure all testing is authorized, contained and ethical.

## 2. Lab Environment

| Item | Detail |
|---|---|
| Hypervisor | Oracle VirtualBox on a personal Windows laptop |
| Guest OS | Ubuntu 26.04 virtual machine ("vuln-lab") |
| Target application | OWASP Juice Shop, run in Docker (deliberately vulnerable) |
| Network mode | NAT with one port-forward: host 8080 to guest 3000 |
| Access | localhost only (http://localhost:8080) |

## 3. Scope Statement

- **Own lab only.** All testing happens only on the virtual machine and application described in Section 2, which I own and control.
- **No external targets.** No external systems, websites, networks, services or devices are tested, scanned or touched.
- **Synthetic data only.** All data in the lab is fictional. No real personal, customer or company data is stored, used or collected.

## 4. In Scope

- OWASP Juice Shop running inside the "vuln-lab" VM
- The VM's own guest operating system and Docker container
- Testing reached through localhost only

## 5. Out of Scope

- Any system, IP address, domain or service outside this lab
- The host Windows laptop, home network, or any other device
- Any third-party or production website
- Denial-of-service attacks against anything outside the VM
- Use of any real credentials or real personal data

## 6. Rules of Engagement

1. Testing is performed only by the lab owner.
2. The VM uses NAT, and no bridged or public network exposure is used.
3. The Juice Shop container is stopped when the lab is not in use.
4. Any technique learned is used only inside this lab.
5. Findings are recorded for learning purposes only.

## 7. Legal and Ethical Compliance

Testing systems without written permission can be illegal. This lab keeps all activity on systems owned by the tester, so no third-party authorization is required. Any extension of scope to another system requires prior written authorization from that system's owner.

## 8. Evidence

- `images/lab-screenshot.png`: Juice Shop running at localhost:8080
- `images/vm-docker-status.png`: container status inside the VM

## 9. Sign-off

| Name | Role | Signature | Date |
|---|---|---|---|
| ________________ | Lab owner | ________________ | ____ / ____ / ______ |
