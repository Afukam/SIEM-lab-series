# SIEM Detection Validation Record

Use this template for each detection or alerting exercise in this repository. Complete it only after running the test and reviewing the resulting telemetry.

## Detection overview

- **Detection name:**
- **Author/date:**
- **SIEM/platform and version:**
- **Log source / integration:**
- **Detection objective:**
- **MITRE ATT&CK tactic/technique (if supported):**

## Hypothesis

Describe the behaviour the detection is intended to identify and why it may be suspicious. State what the detection does not prove.

## Data and prerequisites

- Required event fields:
- Required data source:
- Lab configuration:
- Known telemetry gaps:

## Detection logic

Paste the exact query or rule below. Include the rule format and version where relevant.

```text
<!-- Insert the tested query or rule here. -->
```

## Test procedure

1. Describe the controlled activity used to generate the event.
2. Record the test host and relevant configuration (sanitize identifying details).
3. Record the time window and timezone.
4. Explain how the event was located in the SIEM.

## Results

- **Expected result:**
- **Observed result:**
- **Alert generated?**
- **Relevant event IDs / sanitized evidence:**
- **Screenshot or evidence path:**

## False positives and tuning

Describe legitimate activity that could match the rule, exclusions considered, and the impact of any tuning. Do not add broad exclusions without evidence.

## Limitations

Document missing fields, incomplete telemetry, assumptions, and conditions under which the detection may fail.

## Conclusion

State whether the test passed, partially passed, or failed. A rule should not be described as validated unless the test evidence supports that conclusion.

## References

Link vendor documentation, ATT&CK references, and other sources used.
