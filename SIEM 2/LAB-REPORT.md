# Splunk SIEM Lab 2 — Evidence Review

## Overview

This report records what can be supported by the screenshots in the 36-page evidence PDF supplied for portfolio review. The Splunk-related material appears across PDF pages 17–25 and 31–36. Some pages are product/download information rather than evidence of hands-on analysis; they should not be presented as completed SOC work.

## Installation and initial setup

The screenshots show the Splunk Enterprise 9.2.0.1 Linux download page and download process (PDF pages 20–22). A terminal view shows the installer starting Splunk Enterprise, followed by a browser view of the first-time login page and the Splunk home screen (PDF pages 23–24).

These screenshots support that Splunk Enterprise was installed and its web interface was reached. The product-marketing pages on PDF pages 17–19 do not add technical evidence and are not necessary in a concise portfolio presentation.

## Universal Forwarder and collection workflow

The terminal screenshots on PDF pages 31–32 show work with the Splunk Universal Forwarder package and service commands, including start/enable/restart activity. The visible output includes warnings and setup messages; the screenshots alone do not establish a fully verified, persistent forwarding pipeline.

The Splunk interface shows the data-input options (upload, monitor, forward) and a data collection task-template workflow (PDF pages 25 and 33–35). The screenshots show a distributed collection task being configured and a review/start-collection step.

## Event data

PDF page 36 shows a file upload selected as a data source and a source-type selection/preview screen with rows of web access-style events. This supports that sample data was selected and previewed in Splunk's data onboarding workflow.

The supplied evidence does not clearly show the final successful indexing state, a search against the ingested events, an SPL query, a report, or a dashboard built from the data.

## Evidence assessment

| Area | What the screenshots support | What remains unverified |
|---|---|---|
| Installation | Splunk Enterprise 9.2.0.1 download, installation activity, web login and home screen | Complete configuration details and service health over time |
| Forwarder | Universal Forwarder setup and service-management commands | Confirmed forwarding destination, successful connection, and persistent data delivery |
| Collection | Data-input choices and collection task wizard | Completed collection with verified results |
| Ingestion | File selected and event preview/source-type screen visible | Successful indexing and searchable events |
| Analysis | No clear completed search is visible in the supplied screenshots | SPL searches, interpretation, reports, dashboards, alerting and validation |

## Recommended next steps

1. Verify the Universal Forwarder service status and confirm its configured receiver and inputs.
2. Confirm that the intended events arrive in the expected Splunk index and sourcetype.
3. Run and document a small set of SPL searches, including the time range and fields examined.
4. Build a dashboard from the ingested events and capture the saved dashboard.
5. If alerting is part of the exercise, configure a controlled alert and document its expected and observed behaviour.
6. Capture sanitized evidence of successful ingestion, searches and visualizations.
7. Curate the screenshots: prioritize installation, forwarder configuration, successful ingestion, search results and dashboard evidence; omit vendor marketing pages.

## Scope statement

This is a learning-lab evidence review. The screenshots support installation and data-onboarding work, but do not yet demonstrate a completed Splunk investigation, operational dashboard, or validated alert.
