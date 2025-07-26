# 🤖 glitchtrail-curator-agent

> The first experiment under the [glitchtrail](https://glitchtrail.dev) project:  
> A local-first agent that scans GitHub repos to **curate fixable bugs and code smells** — not fix them, just find the ones worth your time.

---

## 🧠 What It Does

`glitchtrail-curator-agent` is a self-hostable pipeline that:
- 🕵️ Searches open-source GitHub repositories by language, activity, and size
- 🧪 Runs static analysis tools (like `ruff`, `flake8`, or `bandit`)
- 🧠 Optionally summarizes findings with a local LLM
- 🧾 Outputs structured suggestions (JSON/Markdown) for humans or downstream agents

This is **step one** in a larger journey:  
**Curate what’s worth fixing.** Not everything. Just the worthwhile stuff.

---

## ⚙️ Features

- No paid APIs or cloud dependencies
- Works entirely offline (after repo fetch)
- Easy to extend with new analyzers or models
- Human-readable Markdown summaries
- Machine-friendly JSON outputs
- Optional LLM support (StarCoder2, CodeGemma, etc.)

---

## 🏁 Quick Start

### 1. Clone the repo
```bash
git clone https://github.com/YOUR_ORG/glitchtrail-curator-agent.git
cd glitchtrail-curator-agent

