# Private Ground Truth — Draft

> Author-only design document. Do not distribute with the player package.

## Intended Story
- A real severe-weather communications degradation begins first.
- EDGE-GW-01 experiences legitimate tunnel instability.
- SOC-SRV-01 receives delayed or incomplete forwarded telemetry.
- Administrators perform legitimate recovery actions.
- During this visibility degradation, an unauthorized actor abuses a privileged or service identity.
- The actor traverses at least one server boundary.
- Activity on FILE-SRV-02 and/or BACKUP-SRV-01 cannot be explained by the storm.
- Evidence collection/staging occurs while centralized visibility is impaired.
- Host-local artifacts prove actions that the SOC did not receive in real time.
- Final answer: **combined event — legitimate storm outage plus malicious activity exploiting the visibility gap.**

Exact identities, timestamps, commands, object names and hashes remain TBD until controlled evidence generation is complete.
