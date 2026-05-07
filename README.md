# LLM Paper Notes — 中文精读笔记

离线可读的中文精读笔记 + 论文 PDF 合集。主题: 前沿 LLM 技术报告 + 推理系统(speculative decoding 等)。

## 在线阅读 (GitHub Pages)

| # | 笔记 | 主题 | 大小 |
|---|---|---|---|
| 01 | [INTELLECT-1](https://zhangshuibai.github.io/paper-notes/notes/01_INTELLECT1_2412.01152.html) | 跨地理 GPU 的去中心化训练 / DiLoCo / int8 ring all-reduce | 54 KB |
| 02 | [MiniMax-01](https://zhangshuibai.github.io/paper-notes/notes/02_MiniMax01_2501.08313.html) | Lightning Attention + 32-expert MoE / 1M context | 45 KB |
| 03 | [MiniMax-M1](https://zhangshuibai.github.io/paper-notes/notes/03_MiniMaxM1_2506.13585.html) | Hybrid lightning + softmax / CISPO / open-source reasoning frontier | 47 KB |
| 04 | [MiMo-V2-Flash](https://zhangshuibai.github.io/paper-notes/notes/04_MiMo-V2-Flash_2601.02780.html) | 5:1 SWA-global / sink bias / 256 fine-grained experts / MTP | 62 KB |
| 05 | [MARS](https://zhangshuibai.github.io/paper-notes/notes/05_MARS_2601.15498.html) | Margin-aware speculative verification (logit-ratio) | 41 KB |
| 06 | [Kimi K2.5](https://zhangshuibai.github.io/paper-notes/notes/06_KimiK2.5_2602.02276.html) | 多模态 agentic / Agent Swarm / PARL | 53 KB |

## 论文清单

| 论文 | 团队 | 日期 | arXiv |
|---|---|---|---|
| INTELLECT-1 | Prime Intellect | 2024-12 | [2412.01152](https://arxiv.org/abs/2412.01152) |
| MiniMax-01 | MiniMax | 2025-01 | [2501.08313](https://arxiv.org/abs/2501.08313) |
| MiniMax-M1 | MiniMax | 2025-06 | [2506.13585](https://arxiv.org/abs/2506.13585) |
| MiMo-V2-Flash | Xiaomi LLM-Core | 2026-01 | [2601.02780](https://arxiv.org/abs/2601.02780) |
| MARS | gradient + 港大 + McGill 等 | 2026-01 | [2601.15498](https://arxiv.org/abs/2601.15498) |
| Kimi K2.5 | Kimi Team | 2026-02 | [2602.02276](https://arxiv.org/abs/2602.02276) |

## 相关仓库

更专题的 speculative decoding × RL 笔记另见: [zhangshuibai/spec-rl-notes](https://github.com/zhangshuibai/spec-rl-notes)

## 设计原则

- 单文件 HTML, 无外部依赖, 飞机/无网环境可读
- 中文为主, 技术术语保留英文 (Transformer / MoE / lightning attention / SWA / KV cache / GRPO …)
- 每篇含: 动机 → 背景速查 → 核心方法 → 公式逐行翻译 → 实验亮点 → 局限 → 待验证问题
- 关键机制配 SVG 示意图

## 目录结构

```
.
├── README.md
├── notes/                              # 中文精读 HTML(自包含,可离线)
│   ├── 01_INTELLECT1_2412.01152.html
│   ├── 02_MiniMax01_2501.08313.html
│   ├── 03_MiniMaxM1_2506.13585.html
│   ├── 04_MiMo-V2-Flash_2601.02780.html
│   ├── 05_MARS_2601.15498.html
│   └── 06_KimiK2.5_2602.02276.html
├── INTELLECT1_2412.01152.pdf
├── KimiK2.5_2602.02276.pdf
├── MARS_2601.15498.pdf
├── MiMo-V2-Flash_2601.02780.pdf
├── MiniMax01_2501.08313.pdf
└── MiniMaxM1_2506.13585.pdf
```
