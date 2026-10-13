<div align="center">
  <img src="https://raw.githubusercontent.com/Centinell2025/the-last-evidence-standing/main/branding/BEACON_SEAL.png" alt="Beacon of the Eagle LLC — logotipo corporativo" width="165" />
  <p><strong>BEACON OF THE EAGLE LLC</strong><br/><strong>CENTINELL SUITE DEFENSE</strong></p>
</div>

# HTB Whiteout

**Hack The Box Sherlock candidate**  
Category: **DFIR**  
Target difficulty: **Hard**  
Language: **English**  
Status: **Development / evidence validation**

Whiteout is a server-focused DFIR investigation set during a severe winter storm while a fictional enterprise is undergoing a critical audit. Communications degrade, telemetry is delayed, infrastructure becomes unstable, and malicious activity is concealed inside legitimate operational failures.

> Was the incident caused by the storm, or did an attacker exploit the communications failure to hide malicious activity?

## Server Architecture
- `AUDIT-SRV-01` — audit coordination and evidence intake
- `EDGE-GW-01` — VPN / gateway / communications edge
- `IDENTITY-SRV-01` — identity and authentication services
- `FILE-SRV-02` — corporate file services
- `BACKUP-SRV-01` — backup and recovery services
- `SOC-SRV-01` — security telemetry / event collection

## Investigation Principles
- Separate infrastructure failure from malicious activity.
- Normalize all timestamps to UTC.
- Correlate events across servers.
- Treat missing telemetry as an investigative condition, not proof of absence.
- Require independent corroboration for high-impact findings.
- Preserve evidence integrity with SHA-256 and provenance.
- Use no real credentials, customer data, or external infrastructure.

## Repository Layout
- `docs/` — scenario, server architecture, investigation model and questions
- `artifacts/` — evidence manifest and provenance templates
- `training/` — analyst workflow and standardized answer format
- `submission/` — HTB caption and final release checklist
- `writeup/` — private author solution
- `scripts/` — defensive evidence validation helpers

> Private challenge-development repository intended for HTB review and controlled DFIR training.


---
**Ethical and educational use / Uso ético y educativo:** This is a fictional or simulated defensive cybersecurity training exercise. Test only systems you own or are explicitly authorized to assess. / Ejercicio de ciberseguridad defensiva ficticio o simulado. Realice pruebas solo en sistemas propios o con autorización expresa. See / Consulte [Educational Purpose Notice](EDUCATIONAL_PURPOSE_NOTICE.md).
