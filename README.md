# Correctover

**AI agent runtime security:** fail-closed tool-call interception + offline-verifiable Ed25519 evidence.

```text
Agent → Tool Call → [Guard] → Allow / Block → Signed Receipt
```

## Start here (30 seconds)

```bash
npx -y agent-runtime-guard
npx correctover-scan --demo
```

## Flagship repos

| Repo | What | Why star |
|------|------|----------|
| **[agent-runtime-guard](https://github.com/DSHCorrectover/agent-runtime-guard)** | Pre-execution MCP interceptor, Ed25519 receipts | Product |
| **[correctover-scan](https://github.com/DSHCorrectover/correctover-scan)** | MCP / agent config scanner | Fast try |
| **[mcp-atlas-census](https://github.com/DSHCorrectover/mcp-atlas-census)** | 42,163 servers · 229,827 tools (CC0) | Data |

Compare layers: [COMPARE.md](https://github.com/DSHCorrectover/agent-runtime-guard/blob/main/COMPARE.md)

## Positioning

| Layer | We | Others |
|-------|----|--------|
| Discovery / posture | — | Reco / Pluto class |
| Config scan | correctover-scan | many scanners |
| **Runtime tool-call block** | **agent-runtime-guard** | HOL Guard class |
| Egress proxy | complement | Pipelock class |

We answer: **can this tool call execute now, with a receipt?**  
Not: full SaaS agent inventory.

## Commercial (monetization)

Free tools generate qualified pipeline. Paid work is the business.

| Offering | Public anchor (USD) |
|----------|---------------------|
| Runtime Guard + Scan (open tools) | **Free** |
| Standard human audit (CCS-mapped) | **$2,500** |
| Deep audit + PoC + remediation | **$8,000+** |
| Private deploy / integration | **$5,000** |
| Annual retainer | **$25,000/yr** |

Public numbers are anchors only. Formal quote requires written scoping (async email). 1:1 commercial quotes follow internal PRICE-CARD (higher-ticket tracks). Zero phone. Payment details only after signed scope.

**Contact:** wangguigui@correctover.com  
Subject: `CCS audit scoping — [your stack]`

## Standard

- [draft-correctover-ccs](https://datatracker.ietf.org/doc/draft-correctover-ccs/) — personal Internet-Draft (not an RFC)

## Contact

wangguigui@correctover.com · [SkillPay audit](https://skillpay.alipay.com/public/correctover)

---

**中文：** 执行前 fail-closed 拦截 + 可离线验证收据。国内网络不稳时，优先用 GitHub + `npx` 入口。

## Independent authorization audits (commercial)

MCP migration vendors prove you can handshake. **We certify you didn't go naked after migration** — five binding checks, two independently written verifiers, zero-disagreement requirement, court-ready dossier.

| | |
|---|---|
| Tiers & free sample | [dshcorrectover.github.io/correctover-recovery-admission/services.html](https://dshcorrectover.github.io/correctover-recovery-admission/services.html) |
| Engagement | USD 8,000–15,000 (T1 bounded review) |
| Self-service payment | USDC on Base → `0xfF5EB80DF3Bf4506cd2d0CCC3c8303e1ee267459`, email tx hash to wangguigui@correctover.com |
| Small items (verification pass, $1.99) | same address; on-chain reconciliation, report ships ≤24h |
