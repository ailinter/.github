<div align="center">

<picture>
  <source media="(prefers-color-scheme: dark)" srcset="./profile/logo-icon-dark.svg">
  <img alt="ailinter" src="./profile/logo-icon-dark.svg" width="120">
</picture>

# ailinter

### AI Code. Human Standards.

The open-source safety visor for AI-assisted development — scanning code quality, secrets, and vulnerabilities before and after every AI edit.

---

</div>

## What It Does

ailinter sits between your AI assistant and your codebase. Before the LLM generates a line, ailinter scans the file. After the LLM makes changes, ailinter checks again.

**Five pillars of protection:**

| Pillar | Tool | What It Catches |
|--------|------|----------------|
| Code Quality Radar | `analyze_code` | 17 structural detectors — nesting, complexity, bloat, duplication |
| Secret Scanning | `scan_for_secrets` | 269 rules — AWS keys, API tokens, private keys, JWT |
| Vulnerability Detection | `scan_for_secrets` | 25 deterministic patterns — OWASP Top 10 |
| Refactoring Guide | `get_refactoring_strategy` | 8 step-by-step patterns — guard clauses, extract method, SRP |
| Hotspot Analysis | `list_hotspots` | Frequently-changed files with low quality scores |

## Quick Preview

```bash
# Install
go install github.com/ailinter/ailinter/cmd/ailinter@latest

# Scan a file — quality score + secrets + vulnerabilities
ailinter check src/main.go

# Initialize a project
ailinter init

# Run as an MCP server for your AI assistant
ailinter mcp
```

### Quality Score

Every file gets a **0–100 score** that tells AI assistants whether it's safe to modify:

| Score | Label | What It Means |
|-------|-------|---------------|
| 95–100 | **Go Ahead** | Safe for AI modification |
| 75–94 | **Proceed with Care** | Use small changes, re-check after each edit |
| 0–74 | **Stop & Refactor** | Refactor BEFORE AI touches this file |

## Works With

Cursor · Claude Code · GitHub Copilot · OpenCode · Codex · Gemini CLI · Windsurf · Continue.dev

MCP-compatible. Single Go binary. Zero dependencies.

---

## Get Started

- **Source**: [github.com/ailinter/ailinter](https://github.com/ailinter/ailinter)
- **Website**: [ailinter.dev](https://ailinter.dev)
- **Docs**: See the [README](https://github.com/ailinter/ailinter#readme)

---

<p align="center">
  Created by <a href="https://github.com/IvanBern">Ivan Bernikov</a>
</p>
