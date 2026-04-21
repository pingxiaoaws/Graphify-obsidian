---
title: Graphify + Obsidian 知识库搭建记录
tags: [ai-frontier, tools, graphify, obsidian, claude-code, setup]
created: 2026-04-21
updated: 2026-04-21
status: active
type: permanent
---

# Graphify + Obsidian 知识库搭建记录

## 架构

```
Obsidian Vault (~/vault/)
├── permanent/     ← 手动笔记 (Zettelkasten)
├── ai-frontier/   ← AI 前沿研究
│   ├── digests/   ← 每日速报
│   ├── research/  ← 深度分析
│   ├── tools/     ← 工具评测
│   └── trends/    ← 趋势追踪
├── graphify/      ← 代码知识图谱 (自动)
├── chats/         ← Claude 对话记录
└── CLAUDE.md      ← Claude Code 指令
```

## 技术栈
- **Graphify**: v0.4.23, Python 3.10, tree-sitter AST
- **Obsidian**: 桌面端 (Mac)
- **Claude Code**: Terminal agent
- **同步**: GitHub repo (pingxiaoaws/Graphify-obsidian)

## 实测数据
| 项目 | 节点 | 边 | 社区 | 笔记 | Token 节省 |
|------|------|-----|------|------|-----------|
| openclaw-on-eks-graviton | 298 | 414 | 23 | 292 | 8.6x~18.7x |
| kata-benchmark-v2 | 14 | 15 | 3 | 17 | N/A |

## 灵感来源
- Andrej Karpathy 的 [[ai-twitter-hotposts-2026-04-14|LLM Knowledge Bases 推文]] (55k 赞)
- Skool CC Strategic AI 社区的教程
- 参考 repo: lucasrosati/claude-code-memory-setup (⭐279)

## 工作流
1. 开 Claude Code session → `/resume` 加载上下文
2. 工作中 Claude 查询 graph.json（不重读文件）
3. 结束时 `/save` 保存 session log
4. git commit 触发 hook 自动更新图谱
5. `~/scripts/sync_claude_obsidian.sh` 刷新 Obsidian

## Related
- [[ai-coding-tools]]
- [[ai-twitter-hotposts-2026-04-14]]
