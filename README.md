# PostHog dotfiles

An index of personal dotfiles repos from people at PostHog. Personal setups, not official PostHog config.

## Adopting pieces

You don't need to clone anyone's whole setup. A few common shapes:

- **A single Claude skill or command**: copy the file from someone's `ai/skills/` or `.claude/commands/` into your own.
- **A bash helper**: grab the script and any `bin/lib/` helpers it sources.
- **The whole `.claude/` directory**: fork someone's, then adapt.

Or tell your agent: *"look at PostHog/dotfiles, find a triage-issues command, copy it into my .claude/commands"*.

## The index

| Person | Repo | Highlights |
| --- | --- | --- |
| Matt Brooker | [MattBro/dotfiles-ai](https://github.com/MattBro/dotfiles-ai) | Modular `CLAUDE.md` (engineering, git-workflow, secrets, disagreement), commands, skills |
| Dylan Martin | [dmarticus/dotfiles](https://github.com/dmarticus/dotfiles) | `ai/skills` with MCP-aware skill patterns |
| Phil Haack | [haacked/dotfiles](https://github.com/haacked/dotfiles) | `ai/` folder with `CLAUDE.md`, sub-agents, `/triage-issues` command, Grafana MCP wrappers |

Push to main to add yours.

## Make your own from scratch

Paste in your agent:

> Scan my `~/.claude/`, shell rc files, git/tmux config. Make a public github repo with what's shareable, scrubbing tokens, keys, and private hostnames. Then add a row to PostHog/dotfiles.

---

For official PostHog Claude Code skills: `claude plugin install posthog`.
