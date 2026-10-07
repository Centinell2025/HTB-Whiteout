# Whiteout — Real-World DFIR Operations Exercise

## Mission
Whiteout is designed to train analysts to make defensible decisions during a realistic enterprise incident in which cyber activity and genuine infrastructure failure occur at the same time.

The analyst is not rewarded for finding the most alerts. The analyst is rewarded for correctly separating environmental failure, legitimate recovery work, malicious activity, and unresolved uncertainty.

## Operational Conditions
During a severe winter storm:
- WAN/VPN links become intermittent.
- Centralized logging is delayed.
- Some servers continue operating locally while SOC visibility is degraded.
- Backup jobs fail or restart.
- Administrators perform emergency recovery.
- Authentication retries increase.
- Audit deadlines remain active.
- Suspicious activity occurs inside the same time window.

## Analyst Role
You are the incident analyst supporting both Security Operations and the audit team. You must protect evidence while avoiding unnecessary disruption to critical services.

You are expected to answer:
- What is failing?
- Why is it failing?
- What is merely missing from central visibility?
- What activity is legitimate?
- What activity is malicious?
- What must be contained now?
- What can remain operational?
- What evidence supports each decision?

## Operational Phases

### Phase 1 — Stabilize and preserve
Verify evidence integrity, identify affected services, establish the storm window, identify visibility gaps, and preserve local evidence.

### Phase 2 — Establish ground truth
Build separate timelines for infrastructure degradation, administrator recovery actions, and suspicious activity. Normalize to UTC.

### Phase 3 — Correlate
Compare gateway/VPN telemetry, identity events, local Windows events, SOC ingestion times, backup logs, filesystem evidence and audit activity.

### Phase 4 — Decide
Classify every major event:
- ENVIRONMENTAL
- BENIGN-ADMIN
- MALICIOUS
- UNKNOWN

### Phase 5 — Respond
Recommend containment only where evidence justifies it. Preserve business continuity where activity is benign or still uncertain.

### Phase 6 — Report
Deliver a technical timeline and an executive incident assessment suitable for Security, IT Operations and Audit.

## Success Standard
A senior-quality solution must explain not only **what happened**, but also **why alternative explanations were rejected**, what evidence is missing, and how uncertainty affects the response decision.
