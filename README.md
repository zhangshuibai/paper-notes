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
| 19 | [📊 RL 框架横评 (AReaL/veRL/slime/NeMo-RL/OpenRLHF…)](https://zhangshuibai.github.io/paper-notes/models/notes/19_RL_Frameworks_Comparison.html) | 10 框架 / 12 维对比 / 决策树 / sync vs async | 53 KB |
| 20 | [CoPD (Co-Evolving Policy Distillation)](https://zhangshuibai.github.io/paper-notes/models/notes/20_CoPD_2604.27083.html) | RLVR + OPD 同步 / mutual teacher / 钟形 η(O) | 50 KB |
| 21 | [Prism (test-time scaling for dLLM)](https://zhangshuibai.github.io/paper-notes/models/notes/21_Prism_2602.01842.html) | 离散扩散 LLM 的 hierarchical search + self-verify | 50 KB |
| 22 | [Retrofitting Recurrence](https://zhangshuibai.github.io/paper-notes/models/notes/22_RetrofitRecurrence_2511.07384.html) | 把 pretrained TinyLlama/OLMo/Llama 切成 depth-recurrent / curriculum + Muon | 50 KB |

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

## 🟢 agents/ — Agent 训练 / 环境 / 内存 (31 篇)

| # | 笔记 | 主题 | 大小 |
|---|---|---|---|
| 01 | [DR-Venus](https://zhangshuibai.github.io/paper-notes/agents/notes/01_DR-Venus_2604.19859.html) | 4B 边缘部署 deep research agent / IGPO + 信息增益 reward | 52 KB |
| 02 | [LiteResearcher](https://zhangshuibai.github.io/paper-notes/agents/notes/02_LiteResearcher_2604.17931.html) | Lite 虚拟 Web 世界 / 4B GAIA 71.3% 反超 30B | 50 KB |
| 03 | [Agent-World](https://zhangshuibai.github.io/paper-notes/agents/notes/03_AgentWorld_2604.18292.html) | 1,978 真实环境 / 19,822 工具 / self-evolving arena | 60 KB |
| 04 | [MemPalace 审视](https://zhangshuibai.github.io/paper-notes/agents/notes/04_MemPalace_2604.21284.html) | 空间隐喻 LLM 内存的批判分析 / 96.6% 主要来自哪 | 52 KB |
| 05 | [Rethinking Agentic RL](https://zhangshuibai.github.io/paper-notes/agents/notes/05_RethinkingAgenticRL_2604.27859.html) | 范式重定义: 退化 single-step bandit → POMDP / capability taxonomy | 52 KB |
| 06 | [AgentGym-RL](https://zhangshuibai.github.io/paper-notes/agents/notes/06_AgentGymRL_2509.08755.html) | 模块化框架 / ScalingInter-RL 课程 / 27 任务 | 57 KB |
| 07 | [AgentRL](https://zhangshuibai.github.io/paper-notes/agents/notes/07_AgentRL_2510.04206.html) | 全异步管道 / cross-policy sampling / 跨任务标准化 | 52 KB |
| 08 | [CoEvolve](https://zhangshuibai.github.io/paper-notes/agents/notes/08_CoEvolve_2604.15840.html) | agent ↔ data mutual evolution / GRPO + 信号驱动数据进化 | 44 KB |
| 09 | [HeavySkill](https://zhangshuibai.github.io/paper-notes/agents/notes/09_HeavySkill_2605.02396.html) | Agent Swarm 内化为单模型 inner skill / parallel + summarize | 52 KB |
| 10 | [Search-R1](https://zhangshuibai.github.io/paper-notes/agents/notes/10_SearchR1_2503.09516.html) | search-augmented RL / retrieved-token masking / +41% over RAG | 46 KB |
| 11 | [ReTool](https://zhangshuibai.github.io/paper-notes/agents/notes/11_ReTool_2504.11536.html) | code-integrated RL / cold-start SFT + outcome RL / AIME 67% (vs text-RL 40%) | 60 KB |
| 12 | [LLM Memory 演化合集 (MemoryBank → Mem0 → MEM1 → Memory-R1)](https://zhangshuibai.github.io/paper-notes/agents/notes/12_Memory_evolution.html) | 四篇串读 / heuristic→CRUD→RL 演化 / external vs internal 路线对比 | 70 KB |
| 13 | [RLAnything](https://zhangshuibai.github.io/paper-notes/agents/notes/13_RLAnything_2602.02488.html) | closed-loop RL: env + policy + reward 联合优化 / +9.1% OSWorld / ICML 2026 | 38 KB |
| 14 | [ClawGUI](https://zhangshuibai.github.io/paper-notes/agents/notes/14_ClawGUI_2604.11784.html) | GUI agent 全栈框架 / RL + Eval + Deploy 三件套 / MobileWorld 17.1% | 50 KB |
| 15 | [PinchBench (Kilo Code)](https://zhangshuibai.github.io/paper-notes/agents/notes/15_PinchBench.html) | OpenClaw agent benchmark 调研 / 120+ task / 自托管模型完整接入流程 + 提交流程 | 55 KB |
| 16 | [🖥️ 桌面 GUI / CLI Agent 开源生态全景](https://zhangshuibai.github.io/paper-notes/agents/notes/16_DesktopAgents_landscape.html) | Win/macOS/Linux 桌面 + CLI 生态调研 / 14+ repo / 仿真器+评测+训练数据+infra | 50 KB |
| 17 | [UI-TARS-2 (ByteDance Seed)](https://zhangshuibai.github.io/paper-notes/agents/notes/17_UITARS2_2509.02544.html) | 230B MoE GUI agent / data flywheel + 多轮 PPO + GUI+SDK 混合环境 / OSWorld 47.5 / 主线权重未开源 | 56 KB |
| 18 | [Agent World Model (Snowflake)](https://zhangshuibai.github.io/paper-notes/agents/notes/18_AgentWorldModel_2602.10090.html) | 全合成 code-driven env / 1,000 envs · 35,062 tools / Qwen3-thinking 4/8/14B GRPO / BFCLv3 8B 53.83→65.94 OOD / 全开源 | 60 KB |
| 19 | [MCP-Atlas (Scale AI)](https://zhangshuibai.github.io/paper-notes/agents/notes/19_MCPAtlas_2602.00933.html) | 36 real MCP server · 220 tool · 1,000 task (500 公开 + 500 hold-out) / claims-based Gemini-2.5-Pro judge / Live leaderboard / 被 Claude Opus 4.7 system card 引用 77.3% | 50 KB |
| 20 | [SETA (CAMEL-AI / Eigent.AI)](https://zhangshuibai.github.io/paper-notes/agents/notes/20_SETA_camel.html) | Terminal agent 训练 env / 400+ Docker 合成任务 / AReaL GRPO + RLVR / Qwen3-8B / Claude Sonnet 4.5 + CAMEL = TB2.0 #1 (46.5%) / 全 Apache-2.0 开源 | 50 KB |
| 21 | [4 个 MCP Benchmark 横向对比](https://zhangshuibai.github.io/paper-notes/agents/notes/21_MCPBenchmarks_compare.html) | MCP-Universe / MCP-Atlas / Toolathlon / MCPMark 调研 / GitHub 实时 star / frontier model card 引用 / Toolathlon-Gym 唯一 RL gym / 4 bench 提交流程对比 + 选型决策树 | 55 KB |
| 22 | [TOUCAN (MIT-IBM + UW)](https://zhangshuibai.github.io/paper-notes/agents/notes/22_TOUCAN.html) | arXiv:2510.01179 v1 2025-10-01 / 1.5M tool-agentic SFT 数据(精确 1,527,259 traj) / 495 真实 MCP server · 2,000+ tools / HF 4 subset 精确: Kimi-K2 518,516 + OSS 457,130 + Qwen3 551,613 + **SFT 119,287** / **SFT 内部拆分**: 28.3K original + 40K Ext.1 Irrelevance + 15.8K Ext.2 Diversify + 35.2K Ext.3 Multi-Turn / **3 件 contribution**(Dataset + Pipeline + Checkpoints) / 5-LLM 出题 (Mistral-S/DevStral-S/GPT-OSS/Kimi-K2/Qwen3-32B) × 3 策略 (Single/Multi/Featured-25) + 3-teacher × 2-framework distill + 6-维 Likert task filter + 双层 rule+LLM-as-judge post-filter / **BFCL V3 全 5 子项**: 32B+TOUCAN 70.45 vs GPT-4.5 70.32(Overall 险胜)· Multi-Turn 46.50 vs 45.38(**也胜**)· Non-Live AST 7B 反退步 -5.67 / **τ-Bench / τ²-Bench airline+retail+telecom 全 4 域**: 32B 42.33/31.60 · Telecom 域 7B 反退 -6.20 暴露 Communication server 仅 7 个的覆盖偏置 / MCP-Universe Pareto 推进但无绝对数(~25-30%) / **Table 6 消融**: 单训 Single-Turn 把 Irrelevance 砸到 46.88,Ext.1 一举修到 77.85 (+30.97) / 数据 Apache-2.0 + 代码 MIT + 权重跟 Qwen2.5 Apache-2.0 = **全栈商用 friendly** / 27 个 HF ckpt(3 官方 + 15 量化 + 9 衍生) / **校订**: V3≠V4,V4 Agentic 40% 重排后 TOUCAN 不直接可比,需补 SETA/EnvScaler/EnvTuning 类 long-horizon 数据 / 链 #03 #18 #20 #28 #29 #31 | 76 KB |
| 23 | [EnvScaler (RUC NLPIR)](https://zhangshuibai.github.io/paper-notes/agents/notes/23_EnvScaler.html) | 程序化合成 tool-interactive env / Python class = env / dual-agent 100 轮质量门 / 191 env · ~7K scen · ~9K traj / Qwen3-Thinking 1.7B/4B/8B + Reinforce++ / Qwen3-8B BFCL-MT 41.88 超 GPT-4.1 / MIT 全开源 | 50 KB |
| 24 | [🏭 Smithery 调研 (Industry Analysis)](https://zhangshuibai.github.io/paper-notes/agents/notes/24_Smithery.html) | MCP 生态的 Docker Hub / 7,300+ servers (2026-05) / Henry Mao 2024-12 创立 / South Park Commons Seed / Registry 免费 + Hosting 2026-03 转付费 / Connect managed OAuth / #03 #22 #23 三篇 paper 的 MCP 主题源 | 50 KB |
| 25 | [MCP-Universe (Salesforce AI Research)](https://zhangshuibai.github.io/paper-notes/agents/notes/25_MCPUniverse.html) | framework 而非 benchmark / 11 MCP server · 6 domain · 231 task / format+static+dynamic 三层评测拒绝 LLM judge / SOTA GPT-5 43.72% · Grok-4 33.33% · Claude-4-Sonnet 29.44% / <strong>真有 GRPO+verl RL 训练栈</strong> (Hybrid + Fully-Async + TITO + docker_pool) / 内嵌 Deep Research W&D + MCP+ token 压缩 CLI + MCPMark runner / Apache-2.0 585★ / 但 0 frontier model card 引用 | 60 KB |
| 26 | [4 MCP Bench 代码级深潜 — 一个模型能 SOTA 4 个吗](https://zhangshuibai.github.io/paper-notes/agents/notes/26_MCPBenchmarks_codedive.html) | #21 的代码级 follow-up / 实地 ls 4 repo (MCPMark/Universe/Atlas/Toolathlon) / server 重叠矩阵 (仅 GitHub 4-bench 共享 · Notion/Filesystem/Playwright 3-bench · 长尾 ~45) / 4 套 task schema verbatim (verify.py / func-chain DSL / Gemini judge claim / 真 GCP main.py) / 4 verifier 风味互斥 (严断言 / DSL / LLM judge / 真副作用) / 联合训 recipe: TOUCAN 冷启 + MCPMark+Universe RLVR + Toolathlon long-horizon SFT + Atlas LoRA 隔离 / 诚实结论: 不能一 ckpt SOTA 全部, 可以打到各 80% | 60 KB |
| 27 | [≤40B 小模型 MCP 能力训练 landscape](https://zhangshuibai.github.io/paper-notes/agents/notes/27_SmallModelMCP_landscape.html) | 复用导向 survey / 14+ 相关工作每个含完整开源清单 (Code/Data/Model/Pipeline/Eval/License) / 工业线: xLAM (Apache, 619⭐, 60K NC-data) · Hammer (Apache, ICLR 2025, function masking) · Functionary (MIT, 1.6K⭐) · NexusRaven (Apache 13B) · Granite 4.1 8B (IBM 企业) / 学术线 cross-link 5 篇: TOUCAN/EnvScaler/SETA/AWM/Agent-World / 训练框架: ⭐ART+MCP•RL (Apache, 9.5K⭐, 单 H100 / 1 小时 / $5) · Magnet (Google paper-only) · smolagents (27K⭐) · ml-intern · NeMo Toolkit / 4 条 recipe + 决策树 SVG + 开源复用矩阵 / 一句话: TOUCAN SFT 冷启 + ART MCP•RL 在线 = 单卡 H100 / 2 周 / $250 当前 ceiling | 50 KB |
| 28 | [BFCL (Berkeley Function-Calling Leaderboard)](https://zhangshuibai.github.io/paper-notes/agents/notes/28_BFCL.html) | function-calling 事实标准精读 / UC Berkeley Sky Computing Lab Gorilla 团队 / V1 2024-02-26 → V2 2024-08-19 → V3 2024-09-19 → V4 2025-07-17 / V4 重排公式 Agentic 40%+Multi-Turn 30%+Live 10%+Non-Live 10%+Irrelevance 10% / 25 个 individual category (V1 AST · V2 Live · V3 1,000 multi-turn · V4 memory_kv/vector/rec_sum + web_search + format_sensitivity) / AST checker dispatch 代码 + state-based eval / 当前 SOTA: GLM-4.5 V4 70.9% · GPT-5 V4 59.2% · Qwen3-32B V3 75.7% (≤40B ceiling) · Claude Opus 4 V3 仅 25.3 但 MCP-Atlas 77.3 (schema 不兼容) / Apache-2.0 全套 · HF 49,556 下载/月 / 唯一在 GPT-5.5 system card 显式引用的 function-call bench / 与 #19 #21 #22 #23 #26 #27 cross-link 完整 | 60 KB |
| 29 | [Don't Just Fine-tune the Agent, Tune the Environment (ICLR 2026)](https://zhangshuibai.github.io/paper-notes/agents/notes/29_TuneTheEnvironment.html) | 蚂蚁 AWorld + 浙大 + 西湖大学 + 南大 / ICLR 2026 / "tune env 不 tune agent" 范式 / <strong>3 件套</strong>: 4-stage curriculum + Actionable Env Augmentation(把 "No available route" 改成 "Invalid airport code[s]:...") + Fine-grained Progress Reward(r_t^state · r_t^exec dense per-turn)/ <strong>只用 BFCL V3 400 条样本</strong>(4 split×100) / Qwen2.5-7B 7.00→36.92 · Llama-3.1-8B 5.48→28.25 · watt-tool-8B 35.74→54.34(超 GPT-4o 51 / o3 49.25, 仍输 xLAM-2 70.50)/ OOD BFCL V4 Web Search Llama 1.00→15.00 · ACEBench ToolACE-2 8.34→15.00 / direct GRPO baseline 17.42 vs full curriculum 36.92 = <strong>+19.50 pp 纯课程效益</strong> / code: github.com/inclusionAI/AWorld-RL/EnvTuning (MIT, v2 后才放) / 局限: augmentation 字典手写不 scalable · 未评 MCP-Universe / 链 #06 #13 #18 #22 #23 #25 #26 #28 | 60 KB |
| 30 | [ACEBench (EMNLP 2025 Findings)](https://zhangshuibai.github.io/paper-notes/agents/notes/30_ACEBench.html) | USTC + 华为诺亚方舟实验室 / arXiv:2501.12851 v1 2025-01-22 → v8 2025-11-20 / EMNLP 2025 Findings, Suzhou (pages 12970–12998) / 中英双语 tool-use eval (~2,000 entries × 2 lang · 4,538 APIs · 8 domain · 68 sub-domain) / <strong>三大类八子类</strong>: Normal (Atom/SingleTurn/MultiTurn/SimilarAPI/Preference) + Special (Incomplete/Error/Irrelevant 异常输入) + Agent (Multi-Turn user-repeatedly / Multi-Step user-once) / 评测 AST + binary + sandbox state diff + Process Acc (n/m), <strong>无 LLM judge</strong> / overall acc = √n 加权抑制大类支配 / Top5 paper Table 2: GPT-4o 85.4 · GPT-4-Turbo 84.5 · Qwen2.5-Coder-32B 79.6 · Qwen-Max 78.4 · DeepSeek-V3 74.8 / Kimi K2 自报 ACEBench(En) 76.5 vs GPT-4.1 80.1 · Claude Sonnet 4 76.2 / EnvTuning #29 当 OOD: ToolACE-2 Multi-Step 6.67→20.00 / MIT license · 无 HF dataset 镜像 · leaderboard 自 2025-07-21 静默 / 与 ToolACE(2409.00920, SFT 数据集)同源不同物 / 链 #22 #23 #28 #29 | 65 KB |
| 31 | [🏭 Prime Intellect Environments Hub (Industry Analysis)](https://zhangshuibai.github.io/paper-notes/agents/notes/31_PrimeIntellectHub.html) | agentic RL 的 GitHub / 2025-08-27 launch / <strong>1,000+ env · 250+ creator · 100,000+ download</strong> (2026-05 官方) / 三层栈: verifiers SDK (MIT 4,113★ · SingleTurnEnv/MultiTurnEnv/ToolEnv/StatefulToolEnv/BrowserEnv/OpenEnv 桥接 · v1 Env(taskset,harness) API) + Hub 分发 (env 打成 Python wheel via pyproject.toml + hatchling) + prime-rl 训练器 (Apache 1,379★ · async · FSDP2+vLLM+FP8+EP+PD-disagg · INTELLECT-2/3 同栈) / <code>prime env init/install/push</code> CLI 5 行上手 / 2026-02-10 Lab GA: hosted training agentic RL + LoRA · NVIDIA Dynamo · <strong>per-token 计费</strong> · SFT/GEPA/GKD/DPO 列为 near future / Wordle/AIME-25/terminal-bench/alphabet-sort 教科书 env (HF blog walkthrough: 2×A6000 8h GRPO Qwen3-0.6B +43% reward) / 诚实警示: <strong>verifiers 主线无 MCPEnv</strong> · Hub MCP 数量未在公开来源确认 · 1,000 env 质量方差大 · Lab beta 仅 LoRA · 链 models/#07 #08 + agents/#06 #18 #20 #22 #23 #24 #25 #27 #29 | 50 KB |

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
| CoPD (Co-Evolving Policy Distillation) | — | 2026-04 | [2604.27083](https://arxiv.org/abs/2604.27083) |
| Prism (test-time scaling for dLLM) | — | 2026-02 | [2602.01842](https://arxiv.org/abs/2602.01842) |
| veRL/HybridFlow | ByteDance | 2024-09 | [2409.19256](https://arxiv.org/abs/2409.19256) |
| AReaL | 清华 + 蚂蚁 | 2025-05 | [2505.24298](https://arxiv.org/abs/2505.24298) |
| LlamaRL | Meta | 2025-05 | [2505.24034](https://arxiv.org/abs/2505.24034) |
| Laminar | — | 2025-10 | [2510.12633](https://arxiv.org/abs/2510.12633) |
| Retrofitting Recurrence | UMD / NYU / LLNL et al. | 2025-11 | [2511.07384](https://arxiv.org/abs/2511.07384) |

### Agent 训练 / 环境 / 内存

| 论文 | 团队 | 日期 | arXiv |
|---|---|---|---|
| LiteResearcher | — | 2026-04 | [2604.17931](https://arxiv.org/abs/2604.17931) |
| Agent-World | — | 2026-04 | [2604.18292](https://arxiv.org/abs/2604.18292) |
| DR-Venus | inclusionAI | 2026-04 | [2604.19859](https://arxiv.org/abs/2604.19859) |
| MemPalace 审视 | — | 2026-04 | [2604.21284](https://arxiv.org/abs/2604.21284) |
| Search-R1 | UIUC + Meta | 2025-03 | [2503.09516](https://arxiv.org/abs/2503.09516) |
| ReTool | ByteDance Seed | 2025-04 | [2504.11536](https://arxiv.org/abs/2504.11536) |
| MemoryBank | Sun Yat-Sen U + HIT + KTH | 2023-05 | [2305.10250](https://arxiv.org/abs/2305.10250) |
| Mem0 | mem0.ai | 2025-04 | [2504.19413](https://arxiv.org/abs/2504.19413) |
| MEM1 | MIT + NUS + SMART | 2025-06 | [2506.15841](https://arxiv.org/abs/2506.15841) |
| Memory-R1 | LMU Munich + TUM | 2025-08 | [2508.19828](https://arxiv.org/abs/2508.19828) |
| RLAnything | Gen-Verse | 2026-02 | [2602.02488](https://arxiv.org/abs/2602.02488) |
| ClawGUI | — | 2026-04 | [2604.11784](https://arxiv.org/abs/2604.11784) |
| UI-TARS-2 | ByteDance Seed | 2025-09 | [2509.02544](https://arxiv.org/abs/2509.02544) |
| Agent World Model | Snowflake AI Research | 2026-02 | [2602.10090](https://arxiv.org/abs/2602.10090) |
| MCP-Atlas | Scale AI + NUS | 2026-02 | [2602.00933](https://arxiv.org/abs/2602.00933) |
| SETA | CAMEL-AI + Eigent.AI + SambaNova + KAUST 等 | 2026-01 | [CAMEL Blog](https://www.camel-ai.org/blogs/seta-scaling-environments-for-terminal-agents) / [GitHub](https://github.com/camel-ai/seta) |
| TOUCAN | MIT-IBM Watson AI Lab + UW | 2025-10 | [2510.01179](https://arxiv.org/abs/2510.01179) |
| EnvScaler | RUC NLPIR (Gaoling 高瓴) | 2026-01 | [2601.05808](https://arxiv.org/abs/2601.05808) |
| Smithery (industry analysis, not a paper) | Smithery AI (Henry Mao et al.) | 2024-12 至今 | [smithery.ai](https://smithery.ai/) · [GitHub](https://github.com/smithery-ai) |
| MCP-Universe | Salesforce AI Research | 2025-08 | [2508.14704](https://arxiv.org/abs/2508.14704) |
| BFCL (Berkeley Function-Calling Leaderboard) | UC Berkeley Sky Computing Lab (Patil, Mao, Yan, Ji, Suresh, Stoica, Gonzalez) | 2024-02 (V1) → 2025-07 (V4) · ICML 2025 paper | [OpenReview](https://openreview.net/forum?id=2GmDdhBdDk) · [Leaderboard](https://gorilla.cs.berkeley.edu/leaderboard.html) · [GitHub](https://github.com/ShishirPatil/gorilla/tree/main/berkeley-function-call-leaderboard) |
| Don't Just Fine-tune the Agent, Tune the Environment | Zhejiang U + Shanghai Innovation Inst + Westlake U + AWorld Team Inclusion AI + Nanjing U | 2025-10 (v1) · 2026-01 (v2) · **ICLR 2026** | [2510.10197](https://arxiv.org/abs/2510.10197) · [code (AWorld-RL/EnvTuning)](https://github.com/inclusionAI/AWorld-RL/tree/main/EnvTuning) |
| ACEBench: A Comprehensive Evaluation of LLM Tool Usage | USTC + Huawei Noah's Ark Lab (Chen Chen, Xinlong Hao, Weiwen Liu, Xu Huang, Xingshan Zeng et al.) | 2025-01 (v1) → 2025-11 (v8) · **EMNLP 2025 Findings** | [2501.12851](https://arxiv.org/abs/2501.12851) · [GitHub](https://github.com/ACEBench/ACEBench) · [ACL Anthology](https://aclanthology.org/2025.findings-emnlp.697/) · [Leaderboard](https://chenchen0103.github.io/ACEBench/) |
| Prime Intellect Environments Hub (industry analysis, not a paper) | Prime Intellect (Vincent Weisser CEO / Johannes Hagemann CTO / Will Brown 研究) | 2025-08-27 launch · 2026-02-10 Lab GA | [Hub](https://app.primeintellect.ai/dashboard/environments) · [Blog](https://www.primeintellect.ai/blog/environments) · [verifiers](https://github.com/PrimeIntellect-ai/verifiers) · [prime-rl](https://github.com/PrimeIntellect-ai/prime-rl) · [prime CLI](https://github.com/PrimeIntellect-ai/prime) |

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
