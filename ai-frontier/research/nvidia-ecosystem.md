---
title: NVIDIA 生态系统与竞争格局
tags: [ai-frontier, research, nvidia, amd, arm, graviton, inference]
created: 2026-04-21
updated: 2026-04-21
status: active
type: permanent
---

# NVIDIA 生态系统与竞争格局

## NVIDIA 当前战略 (GTC 2026)

### 从"卖铲子"到"全栈 AI"
- Jensen Huang 回归"加速计算"叙事
- 投资 [[nebius]] $20 亿 — 进军 AI 云
- 构建 [[agentic-ai]] 护栏
- **核心变化**: NVIDIA 不满足于只卖 GPU，要做 AI 基础设施全栈

### 对 AWS 的影响
- NVIDIA 做云 = 和 AWS 直接竞争
- AWS 的对策: [[graviton]] 自研芯片 + [[trainium]] AI 芯片
- 但 NVIDIA CUDA 生态壁垒仍然巨大

## 挑战者

### AMD Lemonade
- 开源本地 LLM 服务器，GPU + NPU
- ROCm 生态逐步成熟
- **分析**: AMD 在 AI 推理（inference）有机会，训练（training）还差距大

### ARM/Graviton 在 AI 推理中的定位
- [[graviton]] 4 (m8g) 在 CPU 推理上性价比好
- 适合小模型本地推理、预处理、后处理
- 不适合大模型训练
- **你的场景**: Graviton 跑 OpenClaw + Claude Code + Graphify 完全够用

### 开源模型降低 GPU 依赖
- [[gemma-4]], [[qwen-3-6]] 等模型越来越适合消费级硬件
- NVIDIA 的护城河在缩小（但训练仍需大量 A100/H100）

## 关键判断
1. **短期 (2026)**: NVIDIA 仍然垄断 AI 训练
2. **中期 (2027-2028)**: AI 推理市场被 AMD + ARM + 定制芯片瓜分
3. **长期**: 开源模型 + 本地推理 = GPU 云的需求增长放缓

## Related
- [[ai-frontier-2026-03-27]]
- [[ai-frontier-2026-04-03]]
- [[ai-coding-tools]]
- [[sagemaker-hyperpod-topology]]
