# Vault — Instructions for Claude Code

## What is this vault
Centralized knowledge base for all projects.
Persistent memory across sessions.

## Project stacks
- claude-code: Claude Code reverse engineering & analysis
- kata-benchmark-v2: Kata Containers benchmarking (Go, Shell, fio, stress-ng)
- openclaw-on-eks-graviton: OpenClaw on EKS Graviton deployment (Kubernetes, Terraform, AWS)

## Zettelkasten Rules

### Note creation
- Use wikilinks: [[note-name]] (not markdown links)
- Mandatory YAML frontmatter on every note
- Filenames in kebab-case: `auth-flow.md`, not `Auth Flow.md`
- 1 concept per permanent note (atomicity)
- Minimum 2 wikilinks per note (dense linking)

### Standard frontmatter
```yaml
---
title: Note Name
tags: [project, topic]
created: YYYY-MM-DD
updated: YYYY-MM-DD
status: active
type: permanent
---
```

### Never do
- Don't delete notes without asking
- Don't use markdown links for internal notes (use wikilinks)
- Don't create notes without frontmatter
- Don't change folder structure without documenting it

## Session Commands

### /resume
When you receive this command:
1. Read the 3 most recent session logs in logs/
2. Read architecture/decisions.md for the current project
3. Summarize current state and what's left to do

### /save
When you receive this command:
1. Create a session log in logs/YYYY-MM-DD-description.md
2. Record: what was done, decisions made, pending items
3. Add wikilinks to created/modified notes
4. Run git commit + push if in a repository

## Context Navigation (Graphify)

### 3-Layer Query Rule
1. **First:** query `graphify-out/graph.json` or `graphify-out/wiki/index.md`
   to understand code structure and connections
2. **Second:** query the Obsidian vault for decisions, progress, and project context
3. **Third:** only read raw code files when editing
   or when the first two layers don't have the answer

### When to rebuild the graph
- After structural changes (new modules, major refactors)
- Command: `graphify update . --obsidian --obsidian-dir ~/vault/graphify/<project>`
- The graph is persistent — NO need to rebuild every session

### Do NOT
- Don't manually modify files inside `graphify-out/`
- Don't re-read the entire codebase if the graph already has the information

## Graphify (Codebase Maps)

### Structure
- `graphify/<project-name>/` → knowledge graph for each project
- Notes are auto-generated — do NOT edit manually

### In Graph View
- Filter by `path:graphify` to see only code nodes
- Filter by `-path:graphify` to hide code nodes

## Chat Import Pipeline

### Structure
- `chats/code/` → imported Claude Code conversations
- `chats/web/` → imported Claude Web/App conversations
- All chats get frontmatter with `type: chat` and `chat-import` tag

### Filter in Graph View
- `tag:chat-import` → chats only
- `-path:chats` → hide chats
