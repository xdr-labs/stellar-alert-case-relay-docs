# Stellar Alert & Case Relay Docs

Mintlify documentation for **Stellar Alert & Case Relay**.

The relay fetches Stellar Cyber alerts and cases and forwards them as newline-delimited JSON (NDJSON) over TCP to existing SIEM/SOC workflows.

## Documentation site

- **Site:** https://stellar-relay.xdr.ooo
- **Languages:** English / 한국어
- **Runtime source:** https://github.com/xdr-labs/Stellar-Case-Alert-to-Sylog

## Runtime

The current `Stellar_Alert_Case_Syslog.py` supports:

- Interactive setup with `python3 Stellar_Alert_Case_Syslog.py` or `--setup`
- Alert-only, Case-only, or combined forwarding
- Optional automatic systemd installation
- Manual CLI operation
- SQLite queue/checkpoint persistence and retry/recovery

## Docs

- Overview
- Quickstart
- Configuration
- systemd operations
- Output format
- Troubleshooting
