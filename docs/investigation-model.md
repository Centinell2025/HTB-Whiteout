# TRACE-W Investigation Method

## T — Triage & Trust
Verify evidence hashes, record source server and acquisition context, and identify collection gaps before drawing conclusions.

## R — Reconstruct Time
Normalize timestamps to UTC, separate event occurrence time from log ingestion time, and identify storm-related delay windows.

## A — Analyze & Correlate
Correlate authentication, VPN/gateway activity, process and PowerShell execution, backup activity, filesystem evidence, and SOC ingestion gaps.

## C — Classify Cause
Classify each major event as:
- **ENVIRONMENTAL**
- **BENIGN-ADMIN**
- **MALICIOUS**
- **UNKNOWN**

## E — Evidence-Based Reconstruction
Produce affected servers, identities, ordered event chain, environmental timeline, malicious timeline, confidence level, and exact artifacts supporting each conclusion.

## W — Weather/Visibility Correlation
Compare the cyber timeline against the communications degradation timeline. Missing central telemetry is not proof that an event did not occur locally.
