# Security Policy

DetectionHub is a public defensive-security content repository. Protecting operational information, contributor data, and users of the published content is a priority.

## Reporting a vulnerability

Do not disclose vulnerabilities, leaked credentials, sensitive incident details, or exploitable weaknesses in a public issue.

Use GitHub's **Security** tab and **Report a vulnerability** option when private vulnerability reporting is available. If it is unavailable, contact the repository owner privately through the maintainer profile: https://github.com/saeedtakbiri.

Include:

- A clear description of the issue.
- The affected file, rule, script, workflow, or version.
- Reproduction steps using non-sensitive data.
- Security impact and realistic abuse scenario.
- Suggested mitigation, if known.

Do not include real credentials, personal data, customer data, production logs, malware samples, or confidential infrastructure details.

## Scope

Appropriate private reports include:

- Credentials or secrets accidentally committed to the repository.
- Unsafe scripts or automation that could cause unintended destructive actions.
- Command, query, template, or workflow injection vulnerabilities.
- Dependency or supply-chain risks in repository tooling.
- Documentation that exposes sensitive operational details.
- A detection rule or response procedure whose published behavior creates a material security risk.

Ordinary false positives, detection tuning requests, documentation corrections, and feature requests can use public issues when they contain no sensitive information.

## Safe use

All detections, hunts, scripts, automations, and playbooks must be reviewed and tested in an authorized environment before production use. Public content is not evidence of suitability for a specific environment.
