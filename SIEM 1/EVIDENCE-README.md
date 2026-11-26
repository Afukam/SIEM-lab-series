# Elastic SIEM Lab 1 — Evidence Index

This folder is the evidence record for the Elastic SIEM exercise. Add only files captured from the actual lab. The repository currently documents the exercise, but the items below must not be treated as completed evidence until they have been captured and reviewed.

## Evidence checklist

- [ ] **Environment:** Elastic/Kibana version, endpoint OS, agent/integration details.
- [ ] **Telemetry:** sanitized event document showing the relevant endpoint/network activity.
- [ ] **Investigation:** Discover view or saved query with the time range and relevant fields visible.
- [ ] **Detection:** exact rule export or readable rule configuration, including query, schedule, severity, and required fields.
- [ ] **Validation:** controlled test steps, timestamp/timezone, expected result, observed result, and alert outcome.
- [ ] **Tuning:** legitimate activity considered, false-positive analysis, and limitations.
- [ ] **Report:** completed detection-validation record linked from this folder.

## Suggested filenames

`screenshots/elastic-overview.png`, `screenshots/endpoint-event.png`, `screenshots/detection-rule.png`, `screenshots/alert-result.png`, `sample-events/sanitized-event.json`, and `lab-report.md`.

## Sanitization

Remove credentials, API keys, tokens, email addresses, personal usernames, public IPs, private hostnames, and unrelated personal data. Preserve timestamps, event field names, process names, and other technical details needed to understand the detection. Never fabricate or edit evidence to imply a test succeeded.

## Validation status

**Not yet independently revalidated for this evidence record.** Complete the checklist using the actual Elastic environment before describing a detection as validated.
