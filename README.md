# Stellar Alert & Case Relay Docs

Mintlify documentation for **Stellar Alert & Case Relay**.

The project forwards Stellar Cyber alerts and cases into existing SIEM/SOC workflows. The guide documents a Python daemon that reads from the Stellar Cyber API and sends newline-delimited JSON (NDJSON) over TCP, with alert-only, case-only, or combined operation.

## Documentation site

- Site name: **Stellar Alert & Case Relay**
- Production URL: **https://stellar-relay.xdr.ooo**
- Languages: **English / 한국어**
- Docs framework: **Mintlify**
- Custom domain SSL: managed by Mintlify

## Documentation structure

- Overview / 개요
- Quickstart / 빠른 시작
- Configuration / 설정
- systemd operations / systemd 운영
- Output format / 출력 형식
- Troubleshooting / 문제 해결

## Source-verification note

This repository was initialized from the available product/operations guide. The runtime source code is not currently present in this repository, so implementation-specific details that are not documented in the guide are intentionally not guessed. Before publishing exact API authentication, checkpoint storage, backfill semantics, JSON field schemas, or retry behavior, verify them against the runtime script.
