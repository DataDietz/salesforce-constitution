# Changelog

All notable changes to the AI Agent Constitution and dual-agent architecture are documented here.

## [2026-09-02] - Dual-Agent Architecture and Shared Skills Hub

### Added
- Created `~/.gemini/config/skills.json` to link Google Antigravity into the shared skills repository at `C:\Users\DataD\.agents\skills`.
- Configured exclusion patterns in Antigravity (`claude-.*`, `git-guardrails-claude-code`, duplicate `grill.*` skills) to keep Antigravity clean while sharing all Salesforce DX and productivity skills.

### Architecture Clarification
- Persona and Rule Layer (Independent):
  - Antigravity (Gemini): Maintained in `~/.gemini/config/rules/salesforce_constitution.md` (incorporates Gemini quota preservation and Section 8.1 scratch file offloading).
  - Claude Code: Maintained in `~/.claude/CLAUDE.md` (incorporates Claude-specific CLI notes, hooks, and subagent routing).
- Skills Layer (Shared):
  - Single source of truth: `C:\Users\DataD\.agents\skills` (contains ~180 Salesforce DX skills and Matt Pocock skills).
  - Claude accesses skills via symlinks in `~/.claude/skills/`.
  - Antigravity accesses skills via `~/.gemini/config/skills.json`.
