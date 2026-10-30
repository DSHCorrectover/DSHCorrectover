# Correctover

**Runtime verification & cryptographic evidence for AI agents and node infrastructure.**
从「提示词劝导」到「密码学契约」——运行时七维验证 + Ed25519 签名收据（第三方离线可验）。

## 我们在做什么（一条主线）
- **CCS 运行时验证框架**：AI Agent 工具调用的七维运行时验证（Structure/Schema/Latency/Cost/Identity/Integrity/Security），fail-closed 默认
- **密码学证据链**：每笔授权产出 Ed25519 over JCS（RFC 8785/8032）签名收据——执法/保险/审计可离线核验，无需信任我们的数据库
- **守夜人服务**：矿池/验证节点的签名机安全审计 + 分布式节点契约验证（签名回执链）+ 链上状态突变监控

## 实证（可独立复核）
- **GHSA-vh45-f885-3848**：独立复现并纠正 sm-crypto 弱熵死代码根因，维护者公开致谢
- **[mcphub PR #1299](https://github.com/samanhappy/mcphub/pull/1299)**：高危工具调用前守卫（merged，6 commits/6 files）
- **IETF 草案在案**：agent 运行时验证与签名收据设计（draft-correctover-ccs）
- **弱熵武器库**：secp256k1 九算法（nonce 复用/biased nonce/Weak RNG 枚举），纯手写 ECC 引擎零依赖

## 工具链
| 工具 | 用途 |
|---|---|
| mcp-atlas | 42,163 MCP servers / 229,827 tools 参数级普查（CC0） |
| correctover-scan | MCP/Agent 契约与弱 RNG 风险 CLI 扫描器 |
| ccs-verifier | Ed25519 收据离线验证器 |

## 联系
- 商务: wangguigui@correctover.com
- IETF/W3C 标准线: 同邮箱（标题注明 [standards]）
