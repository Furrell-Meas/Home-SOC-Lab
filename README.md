                    YOUR WINDOWS HOST
                           │
                    VirtualBox / VMware
                           │
              ┌────────────┴────────────┐
              │     Isolated Network    │
              │                         │
        ┌─────▼─────┐             ┌─────▼─────┐
        │   Kali    │             │  Windows  │
        │ Attacker  │────────────►│ Endpoint  │
        └───────────┘             └─────┬─────┘
                                       │
                                       │ Logs
                                       ▼
                                ┌─────────────┐
                                │    Wazuh    │
                                │     SIEM     │
                                └─────────────┘


# Home SOC Lab — Vulnerability Detection & Remediation

## Overview

This project documents a small home Security Operations Center (SOC) lab built to develop practical cybersecurity and security monitoring skills.

The lab focuses on identifying simple vulnerabilities and security misconfigurations, detecting relevant activity through security monitoring, applying remediation, and verifying that the issue has been resolved.

The project is intentionally kept simple and focuses on the fundamental SOC workflow rather than advanced detection engineering.

## Objectives

* Build a small isolated security lab
* Monitor endpoint activity using Wazuh
* Identify common vulnerabilities and misconfigurations
* Generate controlled security events
* Investigate the resulting alerts and evidence
* Apply appropriate remediation
* Verify that vulnerabilities have been resolved
* Document the process in a professional format

## Lab Environment

| Component  | Purpose                          |
| ---------- | -------------------------------- |
| Kali Linux | Security testing and validation  |
| Windows    | Monitored endpoint               |
| Wazuh      | Security monitoring and alerting |
| VirtualBox | Virtualisation                   |

## Lab Workflow

```text
Identify
   ↓
Test
   ↓
Detect
   ↓
Investigate
   ↓
Remediate
   ↓
Verify
   ↓
Document
```

## Findings

| ID    | Finding   | Severity | Status     |
| ----- | --------- | -------- | ---------- |
| F-001 | [Finding] | Medium   | Remediated |
| F-002 | [Finding] | Low      | Remediated |
| F-003 | [Finding] | Medium   | Remediated |

Detailed findings can be found in the `findings/` directory.

## Evidence

Screenshots and supporting evidence are stored in the `screenshots/` directory.

Evidence includes:

* Security alerts
* Command output
* Configuration before remediation
* Configuration after remediation
* Verification results

## Scope

This project is conducted entirely within an isolated home lab environment. Testing is performed only against systems owned and controlled by the lab operator.

## Lessons Learned

This project is intended to demonstrate practical understanding of:

* Basic security monitoring
* Vulnerability identification
* Alert investigation
* Security remediation
* Verification
* Technical documentation

## Future Improvements

Potential future additions include:

* Additional endpoint monitoring
* More vulnerability scenarios
* Automated alerting
* Additional Linux monitoring
* Basic incident-response exercises

