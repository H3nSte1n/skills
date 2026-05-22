<div align="center">

# 🛠️ H3nSte1n / skills

**Agent skills for AI assistants. Safe, expert-level automation in plain English.**

[![skills.sh](https://img.shields.io/badge/skills.sh-registry-orange?logo=data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHZpZXdCb3g9IjAgMCAyNCAyNCI+PHBhdGggZmlsbD0id2hpdGUiIGQ9Ik0xMiAyQzYuNDggMiAyIDYuNDggMiAxMnM0LjQ4IDEwIDEwIDEwIDEwLTQuNDggMTAtMTBTMTcuNTIgMiAxMiAyem0tMSAxNXYtNEg3bDUtOXY0aDVsLTUgOXoiLz48L3N2Zz4=)](https://skills.sh)
[![MIT License](https://img.shields.io/badge/License-MIT-green.svg)](LICENSE)
[![Claude Code](https://img.shields.io/badge/Claude%20Code-compatible-blueviolet)](https://claude.ai/code)
[![Cursor](https://img.shields.io/badge/Cursor-compatible-blue)](https://cursor.com)

_Works with Claude Code · Cursor · VS Code Copilot · Codex · and any [skills.sh](https://skills.sh)-compatible agent_

</div>

---

## What are skills?

Skills are instruction packages that give AI assistants deep, domain-specific knowledge. Install once and your agent instantly knows how to perform complex tasks safely, following expert workflows you didn't have to write yourself.

```bash
npx skills add H3nSte1n/skills --skill <name>
```

---

## Available Skills

| Skill | Description | Install |
|-------|-------------|---------|
| [🖥️ devops](skills/devops/) | Expert DevOps engineer on demand: security audits, service health, nginx & SSL, Docker, auto-rollback | `npx skills add H3nSte1n/skills --skill devops` |

---

## 🖥️ devops — Highlights

> Full documentation: [skills/devops/README.md](skills/devops/README.md)

Manage a Debian/Ubuntu server over SSH in plain English. Every change goes through a **diff → confirm → backup → apply → validate → rollback** workflow, so you stay in full control at every step.

```
/devops
```

```
📊 Server Health — myserver — 2026-05-22

⚠ Issues Found:
  1. [CRITICAL] SSL cert for api.example.com expires in 5 days
  2. [WARNING]  Container "my-app" exited 3h ago
  3. [INFO]     8 security updates pending

✓ All good: nginx, sshd, fail2ban, memory (38% used), disk
```

**What it covers:**

🔒 SSH hardening · UFW firewall · fail2ban · CVE audit  
🌐 Nginx vhosts · Let's Encrypt SSL renewal  
🐳 Docker container lifecycle · Compose · logs · stats  
💾 Auto-backup with rollback on failure  
⏱ Cron & systemd timer inspection  

---

## Quick Start

```bash
# 1. Install the devops skill
npx skills add H3nSte1n/skills --skill devops

# 2. Set your server (add to ~/.zshrc or ~/.bashrc)
export DEVOPS_HOST=agentops@your-server-ip

# 3. Run the setup wizard
/devops setup
```

See [skills/devops/README.md](skills/devops/README.md) for the full setup guide, including how to create a dedicated `agentops` user with a separate SSH key for safe agent access.

---

## Platform Support

| Agent | Install method |
|-------|---------------|
| **Claude Code** | `npx skills add H3nSte1n/skills --skill devops` |
| **Cursor** | `npx skills add H3nSte1n/skills --skill devops` |
| **VS Code Copilot** | `npx skills add H3nSte1n/skills --skill devops` |
| **OpenAI Codex** | `npx skills add H3nSte1n/skills --skill devops` |
| **Manual** | Clone repo and copy `devops/` to `~/.agents/skills/devops/` |

---

## License

MIT · see [LICENSE](LICENSE).
