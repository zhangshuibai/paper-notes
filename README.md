# Paper Notes — 中文精读笔记合集

离线可读的中文精读笔记 + 论文 PDF。三个主题分别放在子目录里。

## 🔵 spec-rl/ — Speculative Decoding × RL (8 篇)

| # | 笔记 | 主题 | 大小 |
|---|---|---|---|
| 01 | [NVIDIA NeMo-RL × EAGLE-3](https://zhangshuibai.github.io/paper-notes/spec-rl/notes/01_NVIDIA_NeMoRL_EAGLE3.html) | 系统集成 / verifier-exact / .detach() 栅栏 | 50 KB |
| 02 | [EAGLE-1/2/3 + DFlash 演化合集](https://zhangshuibai.github.io/paper-notes/spec-rl/notes/02_EAGLE_evolution_DFlash.html) | 底层 drafter 一线发展轨迹 | 50 KB |
| 03 | [SPEC-RL (Shopee)](https://zhangshuibai.github.io/paper-notes/spec-rl/notes/03_SPEC-RL_2509.23232.html) | 复用上一 epoch trajectory + lenience ℓ | 43 KB |
| 04 | [ReSpec](https://zhangshuibai.github.io/paper-notes/spec-rl/notes/04_ReSpec_2510.26475.html) | 三个 gap + reward-weighted KD | 50 KB |
| 05 | [DAS](https://zhangshuibai.github.io/paper-notes/spec-rl/notes/05_DAS_2511.13841.html) | suffix tree + length-aware budget | 40 KB |
| 06 | [SRT](https://zhangshuibai.github.io/paper-notes/spec-rl/notes/06_SRT_2601.09083.html) | per-prompt token-frequency trie + run-ahead | 40 KB |
| 07 | [DFlash 详细版](https://zhangshuibai.github.io/paper-notes/spec-rl/notes/07_DFlash_2602.06036.html) | 块扩散 drafter / 5 层 K/V 注入 / EAGLE-3 范式分叉 | 80 KB |
| 08 | [Hidden States Drift](https://zhangshuibai.github.io/paper-notes/spec-rl/notes/08_HiddenStatesDrift_2604.26412.html) | KV-only reuse vs hidden reuse / KVShot 框架 | 52 KB |
| 09 | [Mirror-SD](https://zhangshuibai.github.io/paper-notes/spec-rl/notes/09_MirrorSD_2510.13161.html) | early-exit + GPU/NPU 异构并行 / +30% over EAGLE-3 | 55 KB |
| 10 | [SSD (Speculative Speculative Decoding)](https://zhangshuibai.github.io/paper-notes/spec-rl/notes/10_SSD_2603.03251.html) | 预测 verify 结果 / draft 隐藏在 verify 后面 / Saguaro 5× | 57 KB |
| 11 | [Performance or Illusion?](https://zhangshuibai.github.io/paper-notes/spec-rl/notes/11_PerformanceOrIllusion_2601.11580.html) | 生产级 vLLM 审视 / paper vs production / 决策 cheatsheet | 51 KB |
| 12 | [DropMatch](https://zhangshuibai.github.io/paper-notes/spec-rl/notes/12_DropMatch_2603.03333.html) | LM head MC dropout / semantic-level acceptance / training-free | 40 KB |
| 13 | [Speculative Verification (SV)](https://zhangshuibai.github.io/paper-notes/spec-rl/notes/13_SpecVerification_2509.24328.html) | info-gain 动态 verify length / companion 模型 | 44 KB |
| 14 | [LK Losses](https://zhangshuibai.github.io/paper-notes/spec-rl/notes/14_LKLosses_2602.23881.html) | 直接优化 acceptance rate / TV+KL hybrid / 反对 proxy 训练 | 41 KB |
| 15 | [📐 Lossless 证明 (Tutorial)](https://zhangshuibai.github.io/paper-notes/spec-rl/notes/15_Lossless_Proof_Tutorial.html) | rejection sampling 数学证明全步详解 (Leviathan/Chen 2023) | 53 KB |
| 16 | [DDTree](https://zhangshuibai.github.io/paper-notes/spec-rl/notes/16_DDTree_2604.12989.html) | 块扩散 drafter 上的最优 draft tree / best-first heap | 47 KB |

建议阅读顺序: **15 (Lossless 数学证明) → 02 (EAGLE 演化) → 04 (ReSpec) → 03 (SPEC-RL) → 05 (DAS) → 01 (NVIDIA) → 06 (SRT) → 07 (DFlash) → 08 (Hidden States Drift) → 09 (Mirror-SD) → 10 (SSD) → 14 (LK Losses) → 13 (SV) → 12 (DropMatch) → 11 (Performance or Illusion?)**

## 🟡 models/ — 前沿模型 / 训练系统 / LM 方法 (13 篇)

| # | 笔记 | 主题 | 大小 |
|---|---|---|---|
| 01 | [INTELLECT-1](https://zhangshuibai.github.io/paper-notes/models/notes/01_INTELLECT1_2412.01152.html) | 跨地理 GPU 去中心化预训练 / DiLoCo / int8 ring all-reduce | 54 KB |
| 02 | [MiniMax-01](https://zhangshuibai.github.io/paper-notes/models/notes/02_MiniMax01_2501.08313.html) | Lightning Attention + 32-expert MoE / 1M context | 45 KB |
| 03 | [MiniMax-M1](https://zhangshuibai.github.io/paper-notes/models/notes/03_MiniMaxM1_2506.13585.html) | Hybrid lightning + softmax / CISPO | 47 KB |
| 04 | [MiMo-V2-Flash](https://zhangshuibai.github.io/paper-notes/models/notes/04_MiMo-V2-Flash_2601.02780.html) | 5:1 SWA-global / sink bias / 256 fine-grained experts / MTP | 62 KB |
| 05 | [MARS](https://zhangshuibai.github.io/paper-notes/models/notes/05_MARS_2601.15498.html) | Margin-aware speculative verification (logit-ratio) | 41 KB |
| 06 | [Kimi K2.5](https://zhangshuibai.github.io/paper-notes/models/notes/06_KimiK2.5_2602.02276.html) | 多模态 agentic / Agent Swarm / PARL | 53 KB |
| 07 | [INTELLECT-2](https://zhangshuibai.github.io/paper-notes/models/notes/07_INTELLECT2_2505.07291.html) | 全球去中心化 RL / PRIME-RL / TOPLOC / SHARDCAST | 59 KB |
| 08 | [INTELLECT-3](https://zhangshuibai.github.io/paper-notes/models/notes/08_INTELLECT3_2512.16144.html) | 106B MoE agentic RL / prime-rl 三件套 / IcePop | 57 KB |
| 09 | [OmniHuman 1.5](https://zhangshuibai.github.io/paper-notes/models/notes/09_OmniHuman1.5_2508.19209.html) | 数字人 / Sys1+Sys2 / Pseudo Last Frame | 48 KB |
| 10 | [TOP](https://zhangshuibai.github.io/paper-notes/models/notes/10_TOP_2508.19228.html) | Token Order Prediction / learning-to-rank LM 损失 | 48 KB |
| 11 | [TIDE](https://zhangshuibai.github.io/paper-notes/models/notes/11_TIDE_2604.26951.html) | 跨架构 dLLM 蒸馏 / TIDAL+CompDemo+Reverse CALM | 51 KB |
| 12 | [NCP / ConceptLM](https://zhangshuibai.github.io/paper-notes/models/notes/12_NCP_2602.08984.html) | Next Concept Prediction / VQ 离散 latent | 50 KB |
| 13 | [LongLLaDA](https://zhangshuibai.github.io/paper-notes/models/notes/13_LongLLaDA_2506.14429.html) | 扩散 LLM 长上下文 / NTK-RoPE training-free | 46 KB |
| 14 | [MTP (Gloeckle, Meta)](https://zhangshuibai.github.io/paper-notes/models/notes/14_MTP_Gloeckle_2404.19737.html) | MTP 元论文 / 共享 trunk + n heads / 自-spec | 36 KB |
| 15 | [FastMTP](https://zhangshuibai.github.io/paper-notes/models/notes/15_FastMTP_2509.18362.html) | 单 head + position-shared / self-distill / 2.03× lossless | 54 KB |
| 16 | [L-MTP (Leap MTP)](https://zhangshuibai.github.io/paper-notes/models/notes/16_LMTP_2505.17505.html) | 跳跃式 MTP / 非相邻 future / NeurIPS 2025 | 50 KB |
| 17 | [MuToR (Registers)](https://zhangshuibai.github.io/paper-notes/models/notes/17_MuToR_2505.10518.html) | 可学习 register tokens 替代 n heads | 53 KB |
| 18 | [FSP (Beyond MTP)](https://zhangshuibai.github.io/paper-notes/models/notes/18_FSP_2510.14751.html) | Future Summary Prediction / RevLM 蒸馏 | 41 KB |

### MTP 系列阅读建议

**14 (Gloeckle 元论文) → 15 (FastMTP 工程化) → 16 (L-MTP 跳跃) → 17 (MuToR registers) → 18 (FSP summary)**

- 14 是起源(n 个独立 heads,提 sample efficiency + 自-spec decoding)
- 15 是把 MTP 真正做成可工程化的 spec decoding(单 head + self-distill + 2.03× lossless 加速)
- 16/17 是对 head 设计的两条改良路线: 跳跃 vs register
- 18 是对 MTP "预测精确 token"这一根本目标的反思——预测未来摘要更稳

也可参考 [TOP (10)](https://zhangshuibai.github.io/paper-notes/models/notes/10_TOP_2508.19228.html) 看反向观点(用 ranking 替代 MTP)。

### INTELLECT 系列阅读建议

I-1 (decentralized **pretrain** / DiLoCo) → I-2 (decentralized **RL** / TOPLOC + SHARDCAST) → I-3 (**agentic RL** on top of GLM-4.5-Air-Base / 务实转向)。

三代叙事曲线: 从证明跨地理预训练可行,到证明跨地理 RL 可信,到放弃 from-scratch 而转向 agentic 实用。

## 🟢 agents/ — Agent 训练 / 环境 / 内存 (4 篇)

| # | 笔记 | 主题 | 大小 |
|---|---|---|---|
| 01 | [DR-Venus](https://zhangshuibai.github.io/paper-notes/agents/notes/01_DR-Venus_2604.19859.html) | 4B 边缘部署 deep research agent / IGPO + 信息增益 reward | 52 KB |
| 02 | [LiteResearcher](https://zhangshuibai.github.io/paper-notes/agents/notes/02_LiteResearcher_2604.17931.html) | Lite 虚拟 Web 世界 / 4B GAIA 71.3% 反超 30B | 50 KB |
| 03 | [Agent-World](https://zhangshuibai.github.io/paper-notes/agents/notes/03_AgentWorld_2604.18292.html) | 1,978 真实环境 / 19,822 工具 / self-evolving arena | 60 KB |
| 04 | [MemPalace 审视](https://zhangshuibai.github.io/paper-notes/agents/notes/04_MemPalace_2604.21284.html) | 空间隐喻 LLM 内存的批判分析 / 96.6% 主要来自哪 | 52 KB |

## 论文清单 (按时间)

### Speculative Decoding × RL

| 论文 | 团队 | 日期 | arXiv |
|---|---|---|---|
| EAGLE-1 | SJTU et al | 2024-01 | [2401.15077](https://arxiv.org/abs/2401.15077) |
| EAGLE-2 | SJTU et al | 2024-06 | [2406.16858](https://arxiv.org/abs/2406.16858) |
| EAGLE-3 | SJTU et al | 2025-03 | [2503.01840](https://arxiv.org/abs/2503.01840) |
| SPEC-RL | Shopee | 2025-09 | [2509.23232](https://arxiv.org/abs/2509.23232) |
| ReSpec | NTU + 阿里 | 2025-10 | [2510.26475](https://arxiv.org/abs/2510.26475) |
| DAS | Together AI + UIUC | 2025-11 | [2511.13841](https://arxiv.org/abs/2511.13841) |
| SRT | — | 2026-01 | [2601.09083](https://arxiv.org/abs/2601.09083) |
| DFlash | — | 2026-02 | [2602.06036](https://arxiv.org/abs/2602.06036) |
| NVIDIA NeMo-RL + EAGLE-3 | NVIDIA | 2026-04 | [2604.26779](https://arxiv.org/abs/2604.26779) |
| Hidden States Drift (KVShot) | — | 2026-04 | [2604.26412](https://arxiv.org/abs/2604.26412) |
| Mirror-SD | — | 2025-10 | [2510.13161](https://arxiv.org/abs/2510.13161) |
| SSD (Speculative Speculative Decoding) | Tri Dao 等 | 2026-03 | [2603.03251](https://arxiv.org/abs/2603.03251) |
| Performance or Illusion? | — | 2026-01 | [2601.11580](https://arxiv.org/abs/2601.11580) |
| DropMatch | — | 2026-03 | [2603.03333](https://arxiv.org/abs/2603.03333) |
| Speculative Verification (SV) | — | 2025-09 | [2509.24328](https://arxiv.org/abs/2509.24328) |
| LK Losses | — | 2026-02 | [2602.23881](https://arxiv.org/abs/2602.23881) |
| DDTree | — | 2026-04 | [2604.12989](https://arxiv.org/abs/2604.12989) |
| (经典) Leviathan et al. — Fast Inference via SD | Google | 2022-11 | [2211.17192](https://arxiv.org/abs/2211.17192) |
| (经典) Chen et al. — Accelerating LLM Decoding | DeepMind | 2023-02 | [2302.01318](https://arxiv.org/abs/2302.01318) |

### 前沿模型 / 训练系统 / LM 方法

| 论文 | 团队 | 日期 | arXiv |
|---|---|---|---|
| INTELLECT-1 | Prime Intellect | 2024-12 | [2412.01152](https://arxiv.org/abs/2412.01152) |
| MiniMax-01 | MiniMax | 2025-01 | [2501.08313](https://arxiv.org/abs/2501.08313) |
| INTELLECT-2 | Prime Intellect | 2025-05 | [2505.07291](https://arxiv.org/abs/2505.07291) |
| MiniMax-M1 | MiniMax | 2025-06 | [2506.13585](https://arxiv.org/abs/2506.13585) |
| LongLLaDA | OpenMOSS / SJTU | 2025-06 | [2506.14429](https://arxiv.org/abs/2506.14429) |
| OmniHuman 1.5 | ByteDance | 2025-08 | [2508.19209](https://arxiv.org/abs/2508.19209) |
| TOP | Zuhri et al | 2025-08 | [2508.19228](https://arxiv.org/abs/2508.19228) |
| INTELLECT-3 | Prime Intellect | 2025-12 | [2512.16144](https://arxiv.org/abs/2512.16144) |
| MiMo-V2-Flash | Xiaomi LLM-Core | 2026-01 | [2601.02780](https://arxiv.org/abs/2601.02780) |
| MARS | gradient + 港大 + McGill 等 | 2026-01 | [2601.15498](https://arxiv.org/abs/2601.15498) |
| NCP / ConceptLM | — | 2026-02 | [2602.08984](https://arxiv.org/abs/2602.08984) |
| Kimi K2.5 | Kimi Team | 2026-02 | [2602.02276](https://arxiv.org/abs/2602.02276) |
| TIDE | PKU YuanGroup | 2026-04 | [2604.26951](https://arxiv.org/abs/2604.26951) |
| MTP (Gloeckle, Meta) | Meta FAIR | 2024-04 | [2404.19737](https://arxiv.org/abs/2404.19737) |
| MuToR (Registers) | — | 2025-05 | [2505.10518](https://arxiv.org/abs/2505.10518) |
| L-MTP (Leap MTP) | NeurIPS'25 | 2025-05 | [2505.17505](https://arxiv.org/abs/2505.17505) |
| FastMTP | Tencent BAC | 2025-09 | [2509.18362](https://arxiv.org/abs/2509.18362) |
| FSP (Beyond MTP) | — | 2025-10 | [2510.14751](https://arxiv.org/abs/2510.14751) |

### Agent 训练 / 环境 / 内存

| 论文 | 团队 | 日期 | arXiv |
|---|---|---|---|
| LiteResearcher | — | 2026-04 | [2604.17931](https://arxiv.org/abs/2604.17931) |
| Agent-World | — | 2026-04 | [2604.18292](https://arxiv.org/abs/2604.18292) |
| DR-Venus | inclusionAI | 2026-04 | [2604.19859](https://arxiv.org/abs/2604.19859) |
| MemPalace 审视 | — | 2026-04 | [2604.21284](https://arxiv.org/abs/2604.21284) |

## 设计原则

- **单文件 HTML, 无外部依赖**——飞机/无网环境可读
- 中文为主,技术术语保留英文(Transformer / draft / target / acceptance length / KV cache / GRPO …)
- 每篇含: 动机 → 背景速查 → 核心方法 → 公式逐行翻译 → 实验亮点 → 局限 → 待验证问题
- 关键机制配 SVG 示意图或动画

## 目录结构

```
.
├── README.md
├── spec-rl/        # Speculative decoding × RL  — 10 PDFs / 8 HTML
├── models/         # 前沿模型 / 训练系统 / LM 方法 — 14 PDFs / 13 HTML
└── agents/         # Agent 训练 / 环境 / 内存    — 4 PDFs / 4 HTML
```
