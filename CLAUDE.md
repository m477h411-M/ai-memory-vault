# Repo Boot — AI Memory Vault

<!-- This is the REPOSITORY's own boot file, loaded by Claude Code when `claude`
     runs inside a clone of this repo. It is NOT the boot-config template that
     ships to users — that one is templates/CLAUDE.md and belongs in the working
     folder the person runs their own agent from. Don't confuse the two. -->

You are running inside a clone of the **ai-memory-vault** repository.

Unless the person says otherwise, assume they are here for one reason: to build their memory vault.

**Do this first.** Read `ai-memory-vault.md` at the root of this repo and execute it. It is a system builder, written to be followed step by step with the person — not summarized, not described, not skimmed for highlights. Start at Part 1, Step 1 and work through every phase in order. Do not skip phases. Do not improvise.

Open with one line so they know what is about to happen, then wait for a yes. Something like: "I've got the AI Memory Vault builder loaded — want me to start the setup? It's about ten minutes of questions."

If they say they are only looking around, or ask a question about the repo, answer it normally and leave the build alone until they ask for it.

## Two things to know before you open the builder

- It runs in two parts. Part 1 gets Obsidian installed and connected; Part 2 is the interactive build. **Being in a Claude Code session proves neither** — run Part 1's install check anyway; it takes seconds.
- Part 1, Step 5 hand-edits `obsidian.json`, the registry of every Obsidian vault on the machine. Back it up before writing, build the JSON in a script file rather than through shell quoting, and verify the written path actually exists on disk. The builder explains why at length. Read that section before acting on it.

## What's in here

- `ai-memory-vault.md` — the builder. The whole system, start to finish.
- `templates/` — the starter files the build hands to the person: `CLAUDE.md` (their boot config), `VAULT-INDEX.md`, `DAILY-NOTE.md`, `MEMORY.md`.
- `TROUBLESHOOTING.md` — fixes, and the free backup options.
- `skills/ai-memory-vault/SKILL.md` + `.claude-plugin/` — the same builder, packaged so it can be installed as a Claude Code plugin.

## If you are editing this repo

`ai-memory-vault.md` embeds its own copies of `templates/CLAUDE.md` and `templates/VAULT-INDEX.md`. Each pair is one document written for two audiences: the embedded copy gets filled in by the interview, the template by hand with `[FILL IN: ...]` markers. Placeholder text and audience framing legitimately differ. Everything else — every rule, every sentence that is not a placeholder — must stay word-for-word identical. Change one, change the other in the same commit.
