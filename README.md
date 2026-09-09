# AI Memory Vault 

## Templates

Starter files for the system. Every spot that needs your information is marked `[FILL IN: ...]`. Drop a template in and tell your AI "fill this in for me," and it will interview you and write it in your voice (each template carries that instruction for the AI). Or fill them out by hand if you prefer.

- **[CLAUDE.md](templates/CLAUDE.md):** the boot config. Goes in the folder you run Claude Code from (your **working directory**), kept **out of your vault** so the vault stays pure notes and doesn't get tangled once you have more than one project. Claude Code auto-loads it every session and points the AI to your vault. Holds your agent's identity (its name, role, and personality) plus your startup sequence and the rules that can't lapse. **This one arrives working:** my own agent's identity is already filled in, clearly marked as the one section to swap if you'd rather have your own.
- **[VAULT-INDEX.md](templates/VAULT-INDEX.md):** the operating manual. This one lives **inside your vault** (it's a note, not config). Your profile, your projects, the full vault rules, and how you like to work with the AI.
- **[DAILY-NOTE.md](templates/DAILY-NOTE.md):** the daily-note template. Goes **inside your vault** at `01 - Daily Notes/Daily Note Template.md`. Every daily note gets created from it, so the log keeps one consistent, scannable shape.
- **[MEMORY.md](templates/MEMORY.md):** the pointer for Claude Code's own memory. Goes in **Claude Code's project folder** (`~/.claude/projects/...`, not your vault). It redirects the native memory back into the vault so you never end up with two memory layers that drift apart.

## Updating

The build script, the templates, and the wizard improve continuously. If you keep a copy of this repo on disk, say to your agent: **"pull the latest ai-memory-vault and tell me what changed."** Updates only ever touch the repo's own files. Your vault, your notes, and your CLAUDE.md are yours and are never inside this repo, so nothing you built can be overwritten. Installed through fullstack-agent? `./fullstack-agent/update.sh` updates every piece at once and prints what changed.


## License

Copyright (c) 2026 Jared Rhodenizer.

Licensed under Creative Commons Attribution-ShareAlike 4.0 International (CC BY-SA 4.0). **Use it in your business, commercially, for free.** Copy it, adapt it, and build your own system on it. Two rules: credit me, and license your own adapted version the same way so the next person gets what you got. Full terms are in the LICENSE file and at https://creativecommons.org/licenses/by-sa/4.0/
