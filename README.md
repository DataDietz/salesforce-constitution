# Salesforce AI Agent Constitution & Architecture Rules

A battle-tested constitution and ruleset for AI Coding Assistants (Gemini, Claude, Cursor, ChatGPT, Copilot) operating on Salesforce orgs (Apex, LWC, Flows, Admin, and Data Operations).

## 📄 Contents
- **[CONSTITUTION.md](./CONSTITUTION.md)**: Full text of Version 2.0.

## 🚀 Quick Start for AI Agents

- **Antigravity / Gemini**: Place in `~/.gemini/config/rules/salesforce_constitution.md`
- **Claude Code**: Place or reference in `CLAUDE.md` or `~/.claude/CLAUDE.md`
- **Cursor**: Place in `.cursorrules` or `.cursor/rules/salesforce.mdc`
- **GitHub Copilot**: Place in `.github/copilot-instructions.md`

## 🛡️ Core Highlights
- **Hard Safety Gates**: Explicit `CONFIRM` required for production deploys, mass DML (>50 records), and destructive changes.
- **Downstream Awareness**: Blast radius checks for Fivetran -> BigQuery -> Sigma Computing -> Account Engagement.
- **Modern Apex Standards**: User mode execution, Queueable + Finalizers, Assert class.
- **Tiered Output**: Tier 1 (Full 4-part plan) for production vs Tier 2 (Short form) for rapid sandbox iteration.