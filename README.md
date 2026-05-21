# PostHog dotfiles

An index of personal dotfiles repos from people at PostHog. Personal setups, not official PostHog config.

Point your agent at this repo and grab what looks useful. e.g. "look at PostHog/dotfiles and pull haacked's triage-issues command into my .claude/commands".

For official PostHog Claude Code skills: `claude plugin install posthog`.

| Person | Repo | Highlights |
| --- | --- | --- |
| Matt Brooker | [MattBro/dotfiles-ai](https://github.com/MattBro/dotfiles-ai) | Modular `CLAUDE.md` (engineering, git-workflow, secrets, disagreement), commands, skills |
| Dylan Martin | [dmarticus/dotfiles](https://github.com/dmarticus/dotfiles) | `ai/skills` with MCP-aware skill patterns |
| Phil Haack | [haacked/dotfiles](https://github.com/haacked/dotfiles) | `ai/` folder with `CLAUDE.md`, sub-agents, `/triage-issues` command, Grafana MCP wrappers |

Push to main to add yours. To bootstrap one from scratch, paste in your agent:

> Scan my `~/.claude/`, shell rc files, git/tmux config. Make a public github repo with what's shareable, scrubbing tokens, keys, and private hostnames. Then add a row to PostHog/dotfiles.
