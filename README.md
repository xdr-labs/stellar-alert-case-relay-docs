# Stellar Alert & Case Relay Docs

Mintlify documentation for **Stellar Alert & Case Relay**.

The project forwards Stellar Cyber alerts and cases into existing SIEM/SOC workflows. The current product guide documents a Python daemon that reads from the Stellar Cyber API and sends newline-delimited JSON (NDJSON) over TCP, with alert-only, case-only, or combined operation.

## Documentation site

- Site name: **Stellar Alert & Case Relay**
- Intended custom domain: **stellar-relay.xdr.ooo**
- Docs framework: **Mintlify**

## Source-verification note

This repository was initialized from the available product/operations guide. The runtime source code is not currently present in this repository, so implementation-specific details that are not documented in the guide are intentionally called out rather than guessed. Before publishing exact API authentication, checkpoint storage, backfill semantics, JSON field schemas, or retry behavior, verify them against the runtime script.
