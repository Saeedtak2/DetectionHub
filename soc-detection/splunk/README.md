# Splunk detections

Converted Splunk Security Content YAML analytics sourced from SigmaHQ rules with `status: stable`.

Each file follows Splunk ESCU `EventBasedDetection` schema:

- New Splunk analytic UUID (not the Sigma rule ID)
- `status: experimental` until a DetectionHub unit test succeeds
- Original Sigma authors retained alongside DetectionHub conversion credit
- CIM `tstats` search when the Splunk data-model backend supports the log source
- Full SPL envelope when CIM conversion is not supported

Source corpus:

- Production: `security-detections/sigma/rules` (77 stable)
- Threat hunting: `security-detections/sigma/rules-threat-hunting` (2 stable)

These detections are not production-ready in Splunk until validated against local telemetry and unit-test fixtures.
