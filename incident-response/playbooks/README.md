# Incident Response Playbooks

This directory contains repeatable response procedures organized by incident category.

## Categories

- `phishing/` — phishing, malicious attachments, credential harvesting, and BEC.
- `malware/` — malware investigation, containment, eradication, and recovery.
- `ransomware/` — rapid containment, impact assessment, recovery, and communication.
- `identity/` — account compromise, token theft, authentication abuse, and privilege escalation.
- `endpoint/` — compromised hosts, persistence, execution, and endpoint isolation.
- `network/` — intrusion, scanning, lateral movement, command-and-control, and exfiltration.
- `cloud/` — cloud identity, workload, storage, SaaS, and control-plane incidents.
- `data-exfiltration/` — data-loss investigation, containment, preservation, and notification.
- `insider-threat/` — human-governed insider-risk procedures coordinated with legal and HR.

Every playbook should define its trigger, scope, severity, roles, prerequisites, evidence sources, investigation steps, decision points, approval requirements, containment, recovery, communication, escalation, and closure criteria. Never store real case evidence or personal information in GitHub.
