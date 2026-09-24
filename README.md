# Stellar Alert & Case Relay Docs

Mintlify documentation for **Stellar Alert & Case Relay**.

The relay fetches Stellar Cyber alerts and cases, stores delivery state in a durable SQLite queue, and forwards newline-delimited JSON (NDJSON) over TCP to existing SIEM/SOC workflows.

## Documentation site

- Site name: **Stellar Alert & Case Relay**
- Production URL: **https://stellar-relay.xdr.ooo**
- Languages: **English / 한국어**
- Docs framework: **Mintlify**

## Current runtime workflow

The documentation covers the wizard-enabled `Stellar_Alert_Case_Syslog.py` build.

- Run with no arguments, or with `--setup`, to start the interactive setup wizard.
- Configure alert-only, case-only, or both streams.
- Optionally install and start the relay automatically as a `systemd` service.
- Continue to use the original CLI flags for manual/foreground operation.
- API tokens are not stored in the systemd unit or command line when the wizard installs the service.

Before following the wizard instructions, verify that your script supports them:

```bash
python3 Stellar_Alert_Case_Syslog.py --help | grep -- --setup
```

If `--setup` is not shown, the host is using an older runtime script.

## Documentation structure

- Overview / 개요
- Quickstart / 빠른 시작
- Configuration / 설정
- systemd operations / systemd 운영
- Output format / 출력 형식
- Troubleshooting / 문제 해결

## Runtime verification

The current usage documentation was updated against the wizard-enabled runtime script and validated on Ubuntu with synthetic Stellar API responses and local TCP receivers. The tested paths include interactive setup, manual CLI operation, alert/case delivery, SQLite queue/checkpoint behavior, duplicate-instance protection, receiver-unreachable queue retention, and generated systemd unit validation.
