# Correctover — AI Reliability 🔬

**Verifiable evidence infrastructure for AI agent security.** Every claim we make ships as an Ed25519-signed receipt with a Bitcoin-anchored timestamp (OpenTimestamps). Don't trust — verify with one command.

[![Free weak-entropy check](https://img.shields.io/badge/🦠_Free-weak--entropy_check-C0392B)](https://entropy.correctover.com)
[![IETF draft-correctover-ccs](https://img.shields.io/badge/IETF-draft--correctover--ccs-blue)](https://datatracker.ietf.org/doc/draft-correctover-ccs/)
[![npm: correctover-scan](https://img.shields.io/npm/v/correctover-scan)](https://www.npmjs.com/package/correctover-scan)
[![PyPI: ccs-verifier](https://img.shields.io/pypi/v/ccs-verifier)](https://pypi.org/project/ccs-verifier/)

## What lives here

| Tool | What it does | Verify it yourself |
|---|---|---|
| **[entropy.correctover.com](https://entropy.correctover.com)** | Free weak-entropy lockfile check — runs 100% in your browser, nothing uploaded. Live weak-RNG watchlist over 600 high-traffic npm packages (163 flagged). | Paste your `package-lock.json`, 30 seconds |
| **[correctover-scan](https://www.npmjs.com/package/correctover-scan)** (npm) | Security scanner for MCP servers & AI agents — 18 checks mapped to OWASP AISVS, incl. weak-RNG fingerprints (CVE-2026-71851 crypto-js / CVE-2026-73567 jsbn). SARIF output. | `npx correctover-scan` |
| **[ccs-verifier](https://www.npmjs.com/package/ccs-verifier)** (npm · [PyPI](https://pypi.org/project/ccs-verifier/)) | One-command independent verification of CCS signed receipts — Ed25519 (RFC 8032) over canonical JSON + SPKI fingerprint. Zero dependencies. | `npx ccs-verifier verify receipt.json` |
| **[ccs-conformance-vectors](https://github.com/DSHCorrectover/ccs-conformance-vectors)** | 66 signed conformance test vectors — reproducible by anyone | clone & run |

## Standards work

- **[draft-correctover-ccs](https://datatracker.ietf.org/doc/draft-correctover-ccs/)** (rev 10, Active) — fail-closed runtime verification + per-invocation cryptographic evidence for AI agents. *Individual Internet-Draft; no IETF endorsement.*
- **[draft-correctover-gg-mcp-parameter-risk](https://datatracker.ietf.org/doc/draft-correctover-gg-mcp-parameter-risk/)** (rev 01) — byte-frozen parameter-risk baseline (benign FPR = 0 on dev split)
- **W3C** interop submissions · **Zenodo DOIs** for methodology (10.5281/zenodo.21783723 et al.)

## Field evidence (all reproducible)

- **SM2 zero-entropy key recovery** — private key from public key + second-level timestamp alone; 5 third-party chain SDKs, black-box, 3/3 reproduced ([demo](https://entropy.correctover.com/media/demo.cast))
- **AWS official MCP sandbox escape** era (CVE-2026-115845): blacklist-style validation lost — runtime verification is the missing layer
- 600-package weak-entropy watchlist: **163 flagged** incl. wallet SDKs at millions of monthly downloads

## Contact

**Guigui Wang** — [wangguigui@correctover.com](mailto:wangguigui@correctover.com) · [entropy.correctover.com](https://entropy.correctover.com)
