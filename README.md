# Paper Notes — 中文精读笔记合集

离线可读的中文精读笔记 + 论文 PDF。两个主题分别放在子目录里。

## 🔵 spec-rl/ — Speculative Decoding × RL (6 篇)

| # | 笔记 | 主题 | 大小 |
|---|---|---|---|
| 01 | [NVIDIA NeMo-RL × EAGLE-3](https://zhangshuibai.github.io/paper-notes/spec-rl/notes/01_NVIDIA_NeMoRL_EAGLE3.html) | 系统集成 / verifier-exact / .detach() 栅栏 | 50 KB |
| 02 | [EAGLE-1/2/3 + DFlash 演化合集](https://zhangshuibai.github.io/paper-notes/spec-rl/notes/02_EAGLE_evolution_DFlash.html) | 底层 drafter 一线发展轨迹 | 50 KB |
| 03 | [SPEC-RL (Shopee)](https://zhangshuibai.github.io/paper-notes/spec-rl/notes/03_SPEC-RL_2509.23232.html) | 复用上一 epoch trajectory + lenience ℓ | 43 KB |
| 04 | [ReSpec](https://zhangshuibai.github.io/paper-notes/spec-rl/notes/04_ReSpec_2510.26475.html) | 三个 gap + reward-weighted KD | 50 KB |
| 05 | [DAS](https://zhangshuibai.github.io/paper-notes/spec-rl/notes/05_DAS_2511.13841.html) | suffix tree + length-aware budget | 40 KB |
| 06 | [SRT](https://zhangshuibai.github.io/paper-notes/spec-rl/notes/06_SRT_2601.09083.html) | per-prompt token-frequency trie + run-ahead | 40 KB |

建议阅读顺序: **02 (EAGLE 演化) → 04 (ReSpec) → 03 (SPEC-RL) → 05 (DAS) → 01 (NVIDIA) → 06 (SRT)**

ReSpec 三个 gap 分析最系统;SPEC-RL 思路最简洁;DAS suffix tree + length-aware budget 工程最优雅;NVIDIA 是产品级集成;SRT 最 niche(model-free + 利用 long-tail bubble)。

## 🟡 models/ — 前沿模型 / 训练系统技术报告 (8 篇)

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

### INTELLECT 系列阅读建议

I-1 (decentralized **pretrain** / DiLoCo) → I-2 (decentralized **RL** / TOPLOC + SHARDCAST) → I-3 (**agentic RL** on top of GLM-4.5-Air-Base / 务实转向)。

三代叙事曲线: 从证明跨地理预训练可行,到证明跨地理 RL 可信,到放弃 from-scratch 而转向 agentic 实用。

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

### 前沿模型 / 训练系统

| 论文 | 团队 | 日期 | arXiv |
|---|---|---|---|
| INTELLECT-1 | Prime Intellect | 2024-12 | [2412.01152](https://arxiv.org/abs/2412.01152) |
| MiniMax-01 | MiniMax | 2025-01 | [2501.08313](https://arxiv.org/abs/2501.08313) |
| INTELLECT-2 | Prime Intellect | 2025-05 | [2505.07291](https://arxiv.org/abs/2505.07291) |
| MiniMax-M1 | MiniMax | 2025-06 | [2506.13585](https://arxiv.org/abs/2506.13585) |
| INTELLECT-3 | Prime Intellect | 2025-12 | [2512.16144](https://arxiv.org/abs/2512.16144) |
| MiMo-V2-Flash | Xiaomi LLM-Core | 2026-01 | [2601.02780](https://arxiv.org/abs/2601.02780) |
| MARS | gradient + 港大 + McGill 等 | 2026-01 | [2601.15498](https://arxiv.org/abs/2601.15498) |
| Kimi K2.5 | Kimi Team | 2026-02 | [2602.02276](https://arxiv.org/abs/2602.02276) |

## 设计原则

- **单文件 HTML, 无外部依赖**——飞机/无网环境可读
- 中文为主,技术术语保留英文(Transformer / draft / target / acceptance length / KV cache / GRPO …)
- 每篇含: 动机 → 背景速查 → 核心方法 → 公式逐行翻译 → 实验亮点 → 局限 → 待验证问题
- 关键机制配 SVG 示意图或动画

## 目录结构

```
.
├── README.md
├── spec-rl/                              # Speculative decoding × RL
│   ├── *.pdf (9 篇)
│   └── notes/ (6 个 HTML)
└── models/                               # 前沿模型 / 训练系统
    ├── *.pdf (8 篇)
    └── notes/ (8 个 HTML)
```
