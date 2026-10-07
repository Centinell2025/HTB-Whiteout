# Scenario — Whiteout

## Executive Situation
Northwind Meridian Group is a fictional enterprise undergoing a high-priority internal and regulatory audit. During the audit window, a severe winter storm impacts regional power and telecommunications.

The enterprise begins experiencing unstable site-to-site communications, intermittent VPN connectivity, packet loss, delayed log forwarding, temporary loss of centralized visibility, backup interruptions, authentication retries, and service restarts.

At first, operations attributes the anomalies to the storm.

The forensic problem begins when several actions cannot be explained by weather or infrastructure instability alone.

## Investigative Conflict
The analyst must distinguish between:
1. **Storm-caused operational degradation**
2. **Benign recovery and administrator activity**
3. **Malicious activity intentionally hidden inside the disruption**

## Core Question
Was the incident only a communications outage, or was the outage used to conceal an intrusion?

## Final Investigative Goal
Produce a defensible incident reconstruction identifying which failures were environmental, which actions were legitimate recovery work, which actions were malicious, the first affected server, the identity used, the server-to-server path, any persistence or collection activity, and the final evidence-supported timeline.
