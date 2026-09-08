# Contributing to DetectionHub

Thank you for helping improve this public security operations content library. Contributions should be useful, testable, clearly documented, and safe to publish.

## Ways to contribute

- Add or improve Sigma, Splunk SPL, Microsoft Sentinel KQL, or Elastic detections.
- Submit threat hunting hypotheses, plans, or queries.
- Improve incident response and triage playbooks.
- Add controlled SOAR workflows or enrichment integrations.
- Add tested Python, PowerShell, or Bash analyst utilities.
- Improve documentation, field mappings, examples, and tests.

## Contribution workflow

1. Search existing content and issues to avoid duplication.
2. Create a focused branch.
3. Add the content under the correct directory.
4. Include documentation and sanitized test data where applicable.
5. Validate syntax and behavior in an authorized test environment.
6. Open a pull request explaining the use case, data requirements, validation, and known limitations.

## Detection requirements

A detection contribution should document:

- Name and concise behavioral description.
- Status: draft, test, validated, or deprecated.
- Author and date.
- Required product, log source, data source, and fields.
- MITRE ATT&CK tactics and technique identifiers.
- Detection or correlation logic.
- Expected false positives and tuning guidance.
- Severity, confidence, and risk rationale.
- Investigation and response guidance.
- Sanitized positive and negative test cases.
- Validation environment and result.

Do not claim a detection is production-ready without evidence from the stated target environment.

## Threat hunt requirements

A hunt should include:

- A falsifiable hypothesis.
- Threat and business rationale.
- Scope and assumptions.
- Required telemetry and retention.
- ATT&CK mapping.
- Queries and time ranges.
- Expected evidence and decision criteria.
- Validation method.
- Outcome, coverage gaps, and recommended follow-up.

## Incident response playbook requirements

A playbook should define:

- Trigger and scope.
- Severity and ownership.
- Prerequisites and evidence sources.
- Investigation steps and decision points.
- Escalation and communication paths.
- Required authorization for containment.
- Containment, eradication, recovery, and monitoring.
- Closure and lessons-learned criteria.

## Tools and automation requirements

Scripts and workflows should include:

- Purpose, inputs, outputs, permissions, dependencies, and examples.
- Safe defaults and explicit failure behavior.
- Tests using sanitized fixtures.
- Logging that does not expose secrets or personal data.
- Human approval for destructive or irreversible actions.
- Rollback or recovery guidance when state can be changed.

## Security and privacy

Never commit:

- Passwords, API keys, access tokens, certificates, or private keys.
- Real incident evidence, raw alerts, packet captures, or memory dumps.
- Customer, employee, victim, or attacker personal information.
- Internal hostnames, IP addresses, architecture, or confidential configurations.
- Live malware or uncontrolled exploit code.

Replace sensitive values with clearly marked synthetic examples. See [SECURITY.md](SECURITY.md) for private reporting guidance.

## Pull request checklist

- The content is in the correct directory.
- The README and examples are clear.
- Required ATT&CK and data-source metadata is included.
- Tests or validation evidence are provided where practical.
- False positives and limitations are documented.
- No secrets or sensitive operational data are present.
- Claims accurately reflect the validation performed.
