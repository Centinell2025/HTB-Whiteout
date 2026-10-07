# START HERE — Whiteout

## Recommended Analyst Machine
**Primary:** Windows 11 analysis workstation with FLARE-VM-compatible tooling.  
**Alternative:** Ubuntu LTS forensic workstation with equivalent EVTX/timeline tooling.

Recommended resources:
- 4 vCPU minimum
- 8 GB RAM minimum
- 16 GB RAM recommended
- 100 GB free disk
- UTC analysis timezone

## Investigation Path
1. Verify `manifest.sha256`.
2. Review `provenance.csv`.
3. Establish the weather/communications degradation window.
4. Establish the SOC visibility gap.
5. Analyze each server locally.
6. Normalize all events to UTC.
7. Apply TRACE-W.
8. Classify major events: ENVIRONMENTAL / BENIGN-ADMIN / MALICIOUS / UNKNOWN.
9. Build the unified timeline.
10. Complete the standardized result report.
