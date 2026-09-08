# DetectionHub — Security Operations, Detection Engineering and Threat Hunting

[![GitHub stars](https://img.shields.io/github/stars/saeedtakbiri/DetectionHub?style=social)](https://github.com/saeedtakbiri/DetectionHub/stargazers)
[![GitHub forks](https://img.shields.io/github/forks/saeedtakbiri/DetectionHub?style=social)](https://github.com/saeedtakbiri/DetectionHub/forks)
[![Last commit](https://img.shields.io/github/last-commit/saeedtakbiri/DetectionHub)](https://github.com/saeedtakbiri/DetectionHub/commits/main)

**DetectionHub is a public Security Operations Center (SOC) content repository for detection engineering, threat hunting, incident response, SOAR automation, and blue-team tools.** It provides a structured foundation for Sigma rules, Splunk SPL, Microsoft Sentinel KQL, Elastic queries, MITRE ATT&CK mappings, investigation playbooks, and reusable security scripts.

> **Project status:** The repository structure and content standards are established. Operational rules, queries, playbooks, and tools will be added and validated over time. Content should not be treated as production-ready until its documentation records successful testing in the target environment.

## Why DetectionHub?

Security operations content is often scattered across SIEM consoles, analyst notes, ticketing systems, and unreviewed scripts. DetectionHub organizes that material as version-controlled, reviewable security content so SOC teams can improve detection coverage, investigation consistency, and response quality.

The repository is intended for:

- SOC managers building a measurable security operations program.
- Detection engineers managing detections as code.
- Threat hunters creating hypothesis-driven hunts.
- Incident responders standardizing triage, containment, and recovery.
- Blue-team analysts working with Splunk, Microsoft Sentinel, Elastic, Sigma, and MITRE ATT&CK.
- Security automation engineers developing SOAR workflows and analyst utilities.

## Security operations content

### [SOC detection engineering](soc-detection/)

Detection rules, correlation logic, data-source requirements, lookups, tests, lifecycle documentation, and deprecated content.

Supported content areas include:

- Vendor-neutral [Sigma rules](soc-detection/sigma/)
- [Splunk SPL detections](soc-detection/splunk/)
- [Microsoft Sentinel KQL detections](soc-detection/kql/)
- [Elastic Security rules](soc-detection/elastic/)
- [Correlation detections](soc-detection/correlations/)
- [Detection tests and sanitized fixtures](soc-detection/tests/)

### [SOC threat hunting](soc-threat-hunting/)

Falsifiable hunt hypotheses, repeatable hunt plans, SIEM queries, ATT&CK mappings, data requirements, validation results, and sanitized hunt reports.

Query formats include [Sigma](soc-threat-hunting/queries/sigma/), [Splunk SPL](soc-threat-hunting/queries/splunk/), [KQL](soc-threat-hunting/queries/kql/), and [Elastic](soc-threat-hunting/queries/elastic/).

### [SOC automation](soc-automation/)

Human-governed automation for SOAR orchestration, enrichment, SIEM and EDR integrations, notifications, ticketing, validation pipelines, and security operations workflows.

### [Incident response](incident-response/)

Structured triage and response playbooks for phishing, malware, ransomware, identity compromise, endpoint incidents, network intrusion, cloud incidents, data exfiltration, and insider threats.

### [Tools and scripts](tools-and-scripts/)

Reusable Python, PowerShell, and Bash utilities, plus query converters, parsers, tests, and analyst documentation.

## Standards and technologies

DetectionHub is designed around commonly used defensive-security standards and technologies:

- **MITRE ATT&CK** for tactics, techniques, and coverage mapping.
- **Sigma** for portable detection rules.
- **Splunk SPL** for Splunk Enterprise Security detection and hunting.
- **Microsoft Sentinel KQL** for Microsoft security analytics.
- **Elastic EQL and ES|QL** for Elastic Security.
- **SOAR** practices for controlled security automation.
- **DFIR and NIST incident response** concepts for investigation and response.
- **Detection as Code** practices for review, testing, versioning, and CI/CD.

## Repository structure

```text
DetectionHub/
├── soc-detection/         # Detection rules, correlations, telemetry and tests
├── soc-threat-hunting/    # Hypotheses, hunt plans, queries and reports
├── soc-automation/        # SOAR workflows, enrichment and integrations
├── incident-response/     # Triage and incident response playbooks
├── tools-and-scripts/     # Python, PowerShell, Bash and analyst utilities
├── CONTRIBUTING.md        # Contribution and content-quality requirements
├── SECURITY.md            # Security and vulnerability reporting policy
├── CITATION.cff           # Machine-readable citation metadata
└── llms.txt               # Curated repository guide for AI tools
```

Each directory contains its own README describing its purpose and expected content.

## Getting started

```bash
git clone https://github.com/saeedtakbiri/DetectionHub.git
cd DetectionHub
```

Choose the area relevant to your work:

- Start a detection in `soc-detection/`.
- document a hunt in `soc-threat-hunting/`.
- create a response procedure in `incident-response/`.
- place controlled workflow automation in `soc-automation/`.
- contribute a tested analyst utility under `tools-and-scripts/`.

Read [CONTRIBUTING.md](CONTRIBUTING.md) before submitting content.

## Content quality principles

All contributed security content should be:

1. **Threat-informed** — explain the behavior or risk being addressed.
2. **Data-aware** — identify required telemetry and important fields.
3. **Mapped** — include applicable MITRE ATT&CK technique identifiers.
4. **Testable** — provide sanitized positive and negative examples where practical.
5. **Tunable** — document expected false positives and environment assumptions.
6. **Actionable** — include investigation or response guidance.
7. **Safe** — never include credentials, personal information, production evidence, or uncontrolled destructive actions.
8. **Honest** — clearly distinguish drafts, validated content, and production-tested content.

## Frequently asked questions

### What is DetectionHub?

DetectionHub is a structured GitHub repository for SOC detections, threat hunting queries, incident response playbooks, security automation, and blue-team tools.

### Which SIEM platforms are supported?

The structure supports vendor-neutral Sigma, Splunk SPL, Microsoft Sentinel KQL, and Elastic Security query formats. Additional platforms can be added when they include clear documentation and validation evidence.

### Is the content mapped to MITRE ATT&CK?

ATT&CK mapping is an expected content-quality requirement. Rules and hunts should identify relevant tactics and techniques without treating ATT&CK coverage alone as proof of detection effectiveness.

### Is every rule production-ready?

No. A public rule is not automatically production-ready. Every detection must be tested against the target telemetry, field mappings, ingestion behavior, and expected false positives before deployment.

### Can I contribute?

Yes. Open an issue or pull request after reviewing [CONTRIBUTING.md](CONTRIBUTING.md). Do not submit private incident data, credentials, malware, personal information, or confidential infrastructure details.

## Security

Review [SECURITY.md](SECURITY.md) before reporting a security concern. Never place sensitive operational details in a public GitHub issue.

## Citation

Machine-readable citation metadata is available in [CITATION.cff](CITATION.cff). If this repository supports your research, training, or SOC program, link to the repository and the specific commit or release you used.

## Maintainer

Maintained by [Saeed Takbiri](https://github.com/saeedtakbiri).
