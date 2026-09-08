# Threat Hunting Queries

This directory contains reusable hunting queries grouped by platform and query language.

## Subdirectories

- `sigma/` — portable Sigma hunt rules.
- `splunk/` — Splunk SPL hunt queries.
- `kql/` — Microsoft Sentinel and Defender KQL queries.
- `elastic/` — Elastic EQL, ES|QL, and Elasticsearch queries.

Each query should document its hypothesis, required data sources, time range, expected output, ATT&CK mappings, known false positives, author, and validation status. Hunting queries are exploratory and must not be promoted to production detections without testing and review.
