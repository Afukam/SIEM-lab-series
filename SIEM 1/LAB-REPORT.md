# Elastic SIEM Lab 1 — Evidence Review

## Overview

This report records what can be supported by the screenshots in the 36-page evidence PDF supplied for portfolio review. The Elastic SIEM material is primarily on pages 4–16. The report distinguishes visible configuration work from outcomes that the screenshots do not establish.

## Environment and telemetry

The screenshots show an Elastic environment accessed from a Kali Linux desktop, the Elastic home page and integrations catalogue, and the Elastic Defend integration page. The Elastic Defend page displays version 8.12.0 and one agent policy (PDF pages 7–9).

A terminal screenshot and the Elastic Observability Stream view show endpoint process events. The stream is filtered with a query resembling `process.args : "sudo"`; event details expose process and user-related fields (PDF pages 9–10). This supports that endpoint telemetry was available for review in Elastic.

## Visualization work

The screenshots show the Kibana visualization editor being used to create an area visualization with `@timestamp` on the horizontal axis and a count of records on the vertical axis (PDF page 5). A later screenshot shows a time-series area chart of record counts (PDF page 13).

The dashboard views on PDF pages 4 and 11 appear empty. The evidence therefore demonstrates visualization-editor use and a chart preview, but does not clearly establish a completed, saved dashboard populated with multiple security panels.

## Detection-rule work

The Security application shows the custom-query rule workflow (PDF pages 6 and 13–16). The visible query is:

```text
event.action : "nmap_scan"
```

The rule form shows the name **Nmap**, a description indicating that it detects an Nmap scan, **Critical** severity, and a risk score of **99** (PDF pages 14–15). The scheduling step shows a five-minute interval (PDF page 15). The final screen presents the options to create the rule without enabling it or create and enable it (PDF page 16).

The screenshots do not show the final creation action, a saved rule state, a controlled Nmap test correlated with the rule, or a resulting alert. Accordingly, this report describes the rule as configured in the creation workflow, not as successfully deployed or validated.

## Alert evidence and limitations

The Alerts page shown on PDF page 12 contains no alert items. This is not proof that the rule failed; it means the supplied screenshots do not demonstrate a triggered alert.

The screenshots also do not provide a complete controlled-test record: there is no clear test timestamp, expected-versus-observed result, alert document, or false-positive assessment.

## Evidence assessment

| Area | What the screenshots support | What remains unverified |
|---|---|---|
| Elastic environment | Elastic interface and Elastic Defend integration visible | Full deployment architecture and configuration |
| Endpoint telemetry | Process events and event details visible in the stream | Reproducible event export and complete source details |
| Visualization | Record-count area chart created in the editor | A saved, populated operational dashboard |
| Detection | Nmap custom-query rule fields configured | Final save/enable state and successful alert trigger |
| Alerting | Alerts interface accessed | A generated alert and response workflow |

## Recommended next steps

1. Confirm whether the Nmap rule was saved and enabled in the original Elastic environment.
2. Re-run a controlled Nmap scan against a lab-owned target and record the exact test time.
3. Capture the matching event, rule configuration, and resulting alert (if one is generated).
4. Save a dashboard with useful panels such as process activity over time, Nmap-related events, and alert counts.
5. Record false-positive considerations and any required fields or integration dependencies.
6. Replace any unclear or duplicated screenshots with sanitized, focused evidence.

## Scope statement

This is a learning-lab evidence review, not a production detection deployment or a claim that the Nmap detection has been validated. The findings above are limited to what is visible in the supplied screenshots.
