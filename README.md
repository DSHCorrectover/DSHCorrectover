# Correctover

**Independent Authorization Verification for AI agents and MCP deployments.**  
We certify that an agent’s action did not exceed the authorization it was actually granted — with evidence a third party can re-verify offline.

```text
Agent → Tool Call → [Decision] → Allow / Block / Escalate → Offline-verifiable Receipt
```

## Start here (30 seconds)

```bash
npx -y agent-runtime-guard
npx correctover-scan --demo
python3 -c "import urllib.request; urllib.request.urlretrieve('https://raw.githubusercontent.com/DSHCorrectover/correctover-recovery-admission/main/verify-recovery.py','v.py')"  # then: python3 v.py
```

## Flagship public assets

| Repo | Layer | What |
|------|-------|------|
| **[correctover-recovery-admission](https://github.com/DSHCorrectover/correctover-recovery-admission)** | Evidence + Audit | 576-anchor decision table: did the action exceed the authorization actually granted? |
| **[verifier-divergence-corpus](https://github.com/DSHCorrectover/verifier-divergence-corpus)** | Evidence | Same Ed25519 vectors, different trust decisions across mainstream verifiers |
| **[findings-registry](https://github.com/DSHCorrectover/findings-registry)** | Evidence | Numbered independent findings (incl. vendor-confirmed P1) |
| **[agent-runtime-guard](https://github.com/DSHCorrectover/agent-runtime-guard)** | Runtime Evidence | Pre-execution MCP interceptor + Ed25519 receipts |
| **[mcp-atlas-census](https://github.com/DSHCorrectover/mcp-atlas-census)** | Evidence | 42k+ servers · 229k+ tools (CC0) |

## Positioning

| Layer | We | Others |
|-------|----|--------|
| Discovery / posture | — | inventory platforms |
| Config scan | correctover-scan | many scanners |
| **Authorization decision + offline-verifiable evidence** | **Correctover** | (gap) |
| Runtime tool-call block | agent-runtime-guard | runtime guards |
| Egress proxy | complement | network proxies |

We answer:  
**Can this tool call execute now, with a receipt?**  
**Did this action stay inside the authorization that was actually granted?**

We are not a full SaaS agent inventory or another platform suite. We occupy the adjudication and evidence layer.

## Commercial

Free corpora and harnesses generate qualified pipeline. Paid work is independent review with court-ready dossiers.

| Offering | Public anchor (USD) |
|----------|---------------------|
| Public evidence corpora + replay | **Free** |
| Standard independent audit | **$2,500** (anchor) |
| Deep audit + PoC + remediation | **$8,000+** (anchor) |
| Bounded authorization review (court-ready) | **$8,000–15,000** |
| Private deploy / integration | **$5,000** (anchor) |
| Annual retainer | **$25,000/yr** (anchor) |

Public numbers are anchors only. Formal quote requires written scoping (async email). 1:1 commercial quotes follow internal price card. Zero phone. Payment details only after signed scope.

**Contact:** wangguigui@correctover.com  
Subject: `Authorization verification scoping — [your stack]`

Service page: [correctover-recovery-admission/services](https://dshcorrectover.github.io/correctover-recovery-admission/services.html)

## Standard note

- [draft-correctover-ccs](https://datatracker.ietf.org/doc/draft-correctover-ccs/) — personal Internet-Draft (not an RFC, not IETF endorsement)

---

**中文**  
独立授权验证：证明 Agent 的动作没有超出实际被授予的授权，并交付第三方可离线复验的证据。我们不做又一个平台，我们占据裁决与证据层。
