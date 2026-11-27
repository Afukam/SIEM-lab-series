# SIEM Lab Series

A collection of hands-on SIEM exercises and supporting evidence, accompanied by technical walkthroughs published on Hashnode.

The goal of this series is to practise the core security operations workflow: generate or collect telemetry, search and interpret events, build visualizations, and explore alerting.

## Labs

### Lab 1 — Elastic SIEM

- Walkthrough: [SIEM Lab 1 — Elastic SIEM](https://afukamwrites.hashnode.dev/siem-lab-1)
- Focus: Elastic deployment, endpoint telemetry, event searches, dashboard visualizations, and a basic detection/alerting exercise.
- Evidence: see the [SIEM 1 evidence checklist](./SIEM%201/EVIDENCE-README.md) and [evidence-reviewed lab report](./SIEM%201/LAB-REPORT.md).

### Lab 2 — Splunk

- Walkthrough: [SIEM Lab 2 — Splunk](https://afukamwrites.hashnode.dev/siem-lab-2)
- Focus: Splunk Enterprise, Universal Forwarder setup, log ingestion, searches, reports, and dashboards.
- Evidence: see the [SIEM 2 evidence checklist](./SIEM%202/EVIDENCE-README.md) and [evidence-reviewed lab report](./SIEM%202/LAB-REPORT.md).

## Detection engineering documentation

Use the [Detection Validation Record](./DETECTION-VALIDATION-TEMPLATE.md) to document each detection exercise consistently. Record the exact query or rule, telemetry prerequisites, controlled test, observed result, false-positive considerations, and limitations.

## What This Series Demonstrates

- Foundational SIEM deployment and configuration.
- Endpoint/log-source onboarding and telemetry collection.
- Searching and reviewing security events.
- Creating dashboards and basic alerting workflows.
- Documenting lab procedures and observations.

## Scope and Limitations

These are learning labs and walkthroughs, not production SOC deployments. The evidence-reviewed reports describe only what the supplied screenshots support. Elastic rule creation is visible, but a saved/triggered alert is not established. Splunk installation and data-onboarding work is visible, but completed searches, dashboards, and alert validation are not established. Detection logic should be independently tested and documented before being described as a validated detection.

## Related Work

- [Cybersecurity Projects index](https://github.com/Afukam/Cybersecurity-Projects)
- [Hashnode technical writing](https://afukamwrites.hashnode.dev/)
- [Current AWS Cowrie + Wazuh SIEM lab journal](https://github.com/Afukam/What-s-going-on-in-Afukam-s-head/blob/main/AWS-Cowrie-Wazuh-SIEM-Lab.md)
