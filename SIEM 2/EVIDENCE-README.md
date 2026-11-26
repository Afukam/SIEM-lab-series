# Splunk SIEM Lab 2 — Evidence Index

This folder is the evidence record for the Splunk exercise. Add only output captured from the actual Splunk environment. The checklist is a plan, not a claim that each item has already been collected.

## Evidence checklist

- [ ] **Environment:** Splunk Enterprise and Universal Forwarder versions, host OS, and forwarding configuration (with secrets removed).
- [ ] **Ingestion:** sanitized event sample showing the intended source, sourcetype, index, and timestamp.
- [ ] **Search:** exact SPL query, selected time range, and explanation of the fields/results.
- [ ] **Visualization:** screenshot of a dashboard or report, with its purpose explained.
- [ ] **Detection:** alert configuration, trigger condition, schedule, and action (if configured).
- [ ] **Validation:** controlled test, expected result, observed result, and alert outcome.
- [ ] **Limitations:** missing fields, parsing issues, data gaps, and false-positive considerations.
- [ ] **Report:** completed detection-validation record or lab report.

## Suggested filenames

`screenshots/splunk-search.png`, `screenshots/forwarder-inputs.png`, `screenshots/dashboard.png`, `screenshots/alert-configuration.png`, `sample-events/sanitized-event.json`, and `lab-report.md`.

## Sanitization

Remove credentials, tokens, internal/public IP addresses where identifying, personal usernames, email addresses, and sensitive hostnames. Do not publish passwords or unredacted configuration files.

## Validation status

**Not yet independently revalidated for this evidence record.** Do not describe searches or alerts as validated until the test and resulting event/alert are documented.
