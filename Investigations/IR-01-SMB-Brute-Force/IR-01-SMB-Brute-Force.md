# Title

**Environtment:**
**Test date:**
**MITRE ATT&CK:**

## 1. Executive Summary

## 2. Objective and Scope

## 3. Test Environment

## 4. Methodology and Evidence

### 4.1 Preparation
A test account was created to safely conduct this brute-force attack, with the username `labuser`. The IP address of the victim was also obtained.
![Figure 1 — Dedicated lab account](screenshots/01-lab-account.png)

## Findings and Interpretation

## 6. Incident timeline

## 7. Responses and Remediation

## 8. Lessons learned and Limitations

## 9. Evidence index

| Figure | Filename | Purpose |
| --- | --- | --- |
| 1 | `screenshots/01-lab-account.png` | Test account |
| 2 | `screenshots/02-target-ip-smb.png` | Target IP and SMB |
| 3 | `screenshots/03-smb-troubleshooting.png` | Connection issue |
| 4 | `screenshots/04-firewall-fix.png` | Scoped firewall troubleshooting |
| 5 | `screenshots/05-netexec-password-spray.png` | Initial test results |
| 6 | `screenshots/06-windows-failed-logins.png` | Windows failure records |
| 7 | `screenshots/07-windows-success-event.png` | Windows success records — verify attribution |
| 8 | `screenshots/08-event-viewer-evidence.png` | Endpoint record detail |
| 9 | `screenshots/09-wazuh-failure-alerts.png` | Wazuh baseline alerts |
| 10 | `screenshots/10-wazuh-success-details-unverified.png` | ANONYMOUS LOGON; not evidence of labuser success |
| 11 | `screenshots/11-custom-rule-xml.png` | Detection rule implementation |
| 12 | `screenshots/12-custom-rule-alert.png` | Correlation trigger |
| 13 | `screenshots/13-wazuh-timeline.png` | Event timeline view |

## 10. References

- [MITRE ATT&CK T1110 — Brute Force](https://attack.mitre.org/techniques/T1110/)
- [Wazuh rules syntax documentation](https://documentation.wazuh.com/current/user-manual/ruleset/ruleset-xml-syntax/rules.html)
- [Microsoft Event 4625 documentation](https://learn.microsoft.com/en-us/windows/security/threat-protection/auditing/event-4625)
- [Microsoft Event 4624 documentation](https://learn.microsoft.com/en-us/windows/security/threat-protection/auditing/event-4624)
