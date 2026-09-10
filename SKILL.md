---
name: ai-memory-vault
description: Build a complete AI-operated memory vault in Obsidian — install and connect Obsidian, interview the person, then write the boot config, root index, folder structure, daily notes, living profile, and the Jobs that let the agent load exactly the right context for any task. Use when someone asks to set up an AI memory vault, a second brain, an Obsidian vault their agent can read and write, persistent memory for their AI, or says "run the ai-memory-vault build".
---

# AI Memory Vault

The entire builder lives in one file: `${CLAUDE_PLUGIN_ROOT}/ai-memory-vault.md`.

**Read that file now, in full, and execute it.** It is a system builder written to be followed step by step with the person — not summarized, not described, not skimmed for highlights. Start at Part 1, Step 1 and work through every phase in order. Do not skip phases. Do not improvise.

Before you open it, know two things:

- It runs in two parts. Part 1 gets Obsidian installed and connected; Part 2 is the interactive build. **Being in a Claude Code session proves neither** — run Part 1's install check anyway; it takes seconds, and skipping it is how setups end without Obsidian.
- Part 1, Step 5 hand-edits `obsidian.json`, the registry of every Obsidian vault on the machine. Back it up before writing, build the JSON in a script file rather than through shell quoting, and verify the written path exists on disk afterwards. The builder explains why at length; read that section before acting on it.

Supporting files, all relative to `${CLAUDE_PLUGIN_ROOT}`:

- `templates/` — the starter files the build refers to: `CLAUDE.md`, `VAULT-INDEX.md`, `DAILY-NOTE.md`, `MEMORY.md`.
- `TROUBLESHOOTING.md` — fixes, and the free backup options to offer once a fresh vault exists.
