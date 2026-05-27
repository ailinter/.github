<div align="center">

<img alt="ailinter" src="./profile/wordmark.png" width="400">

# ailinter

### AI Code. Human Standards.

The open-source safety visor for AI-assisted development — scanning code quality, secrets, and vulnerabilities before and after every AI edit.

```bash
go install github.com/ailinter/ailinter/cmd/ailinter@latest
```

[![Go Version](https://img.shields.io/badge/Go-1.25+-00ADD8?logo=go)](https://go.dev/)
[![License: MIT](https://img.shields.io/badge/license-MIT-blue.svg)](https://github.com/ailinter/ailinter/blob/main/LICENSE)
[![MCP Compatible](https://img.shields.io/badge/MCP-Compatible-6e41e2)](https://modelcontextprotocol.io)

---

</div>

## What ailinter Does

Your AI coding assistant goes into every file blind. ailinter gives it a pre-flight checklist — scanning for complexity traps, hardcoded secrets, and vulnerability patterns before and after every AI edit.

**One tool. Five shields:**

| | | |
|---|---|---|
| **Code Quality** | 17 detectors, 0–100 score | Catches brain methods, deep nesting, god classes |
| **Secret Detection** | 269 rules, 100+ providers | 203% more secrets found than gitleaks alone |
| **Vulnerability** | 25 OWASP patterns | Deserialization, injection, XSS, weak crypto |
| **Refactoring** | 8 step-by-step patterns | Exact instructions AI can follow to fix issues |
| **Hotspots** | Churn × complexity | Find the files most likely to break next |

### The Traffic-Light System

Every file gets a score that tells AI when to back off:

| 95–100 Go Ahead | 75–94 Proceed with Care | 0–74 Stop & Refactor |
|:---:|:---:|:---:|
| Safe to modify | Small changes only | Refactor first |

---

## Works With

<p>
  <img src="https://img.shields.io/badge/Cursor-000?logo=cursor&logoColor=white" alt="Cursor">
  <img src="https://img.shields.io/badge/Claude%20Code-D97757?logo=anthropic&logoColor=white" alt="Claude Code">
  <img src="https://img.shields.io/badge/GitHub%20Copilot-181717?logo=github&logoColor=white" alt="Copilot">
  <img src="https://img.shields.io/badge/OpenCode-1a1a2e?logo=terminal&logoColor=white" alt="OpenCode">
</p>

MCP-compatible. Single binary. Zero dependencies. Under 15MB.

---

## Get Started

- **Install**: `go install github.com/ailinter/ailinter/cmd/ailinter@latest`
- **Quick Start**: `ailinter check src/main.go`
- **Source**: [github.com/ailinter/ailinter](https://github.com/ailinter/ailinter)
- **Website**: [ailinter.dev](https://ailinter.dev)

---

<p align="center">
  Created by <a href="https://github.com/IvanBern">Ivan Bernikov</a>
  &nbsp;·&nbsp;
  <a href="https://www.linkedin.com/in/ivanbernikov/">LinkedIn</a>
</p>
