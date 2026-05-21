# PostHog dotfiles

An index of personal dotfiles repos from people at PostHog. Personal setups, not official PostHog config.

## Adopting pieces

Tell your agent:

> Look at PostHog/dotfiles, find a triage-issues command, copy it into my `.claude/commands`.

## The index

| Person | Repo | Highlights |
| --- | --- | --- |
| Matt Brooker | [MattBro/dotfiles-ai](https://github.com/MattBro/dotfiles-ai) | Modular `CLAUDE.md` (engineering, git-workflow, secrets, disagreement), commands, skills |
| Dylan Martin | [dmarticus/dotfiles](https://github.com/dmarticus/dotfiles) | `ai/skills` with MCP-aware skill patterns |
| Phil Haack | [haacked/dotfiles](https://github.com/haacked/dotfiles) | `ai/` folder with `CLAUDE.md`, sub-agents, `/triage-issues` command, Grafana MCP wrappers |

Push to main to add yours.

## Make your own from scratch

Paste the contents of [bootstrap.md](bootstrap.md) into your agent.

---

For official PostHog Claude Code skills: `claude plugin install posthog`.
