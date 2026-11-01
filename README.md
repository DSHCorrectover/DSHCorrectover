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

## Standard

- [draft-correctover-ccs](https://datatracker.ietf.org/doc/draft-correctover-ccs/) — personal Internet-Draft (not an RFC)

## Contact

wangguigui@correctover.com · [SkillPay audit](https://skillpay.alipay.com/public/correctover)

---

**中文：** 执行前 fail-closed 拦截 + 可离线验证收据。国内网络不稳时，优先用 GitHub + `npx` 入口。
