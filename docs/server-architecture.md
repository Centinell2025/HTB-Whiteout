# Whiteout Server Architecture

## AUDIT-SRV-01
Audit coordination server. Evidence: Windows Security events, audit application logs, file access metadata.

## EDGE-GW-01
Communications edge / VPN gateway. Evidence: VPN sessions, connection state, packet-loss summaries, tunnel resets, authentication metadata.

## IDENTITY-SRV-01
Identity and authentication server. Evidence: successful/failed logons, privileged account activity, authentication timing.

## FILE-SRV-02
Corporate file server. Evidence: Security EVTX, file access, NTFS-derived timeline evidence, staging activity.

## BACKUP-SRV-01
Backup and recovery server. Evidence: backup job logs, service activity, Windows events, recovery attempts.

## SOC-SRV-01
Security telemetry collector. Evidence: ingestion timestamps, delayed-forwarding records, collector restarts, gap windows.

## Network Model
```
Remote / Branch Sites
        |
    EDGE-GW-01
        |
  -------------------------
  |        |        |     |
IDENTITY  AUDIT    FILE  BACKUP
-SRV-01  -SRV-01  -SRV-02 -SRV-01
        \          /
          SOC-SRV-01
```

The storm may interrupt centralized visibility without necessarily interrupting every local action occurring on the servers.
