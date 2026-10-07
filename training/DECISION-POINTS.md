# Whiteout — Decision Points

The exercise includes operational decisions, not only forensic questions.

## Decision 1 — SOC visibility disappears
Central telemetry from FILE-SRV-02 stops arriving.

Choose:
A. Declare the server compromised immediately.  
B. Assume nothing occurred because there are no SOC events.  
C. Treat it as a visibility gap and preserve/analyze host-local evidence.

**Expected analytical behavior:** C.

## Decision 2 — Privileged authentication during outage
A privileged identity authenticates while the VPN is unstable.

The analyst must compare the authentication against approved recovery activity, source/destination context, identity baseline and local execution evidence before classifying it.

## Decision 3 — Backup failure
BACKUP-SRV-01 reports an interrupted job.

The analyst must determine whether the interruption is environmental, malicious, or a mixed event. A failed backup alone is not proof of sabotage.

## Decision 4 — Emergency administrator activity
An administrator performs legitimate recovery actions that resemble suspicious remote administration.

The analyst must avoid false attribution and use corroborating evidence.

## Decision 5 — Local evidence contradicts the SOC
A host-local artifact proves execution during a period in which SOC-SRV-01 received nothing.

The analyst must distinguish **event occurrence time** from **central ingestion time**.

## Decision 6 — Containment under business pressure
The audit is still active and business services are degraded.

The analyst must recommend targeted containment based on evidence rather than indiscriminately isolating every server.

## Scoring Principle
A technically correct artifact finding can still lose decision-quality points if the analyst makes an unsupported operational conclusion.
