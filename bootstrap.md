# Bootstrap your dotfiles

Paste the prompt below into your agent.

---

I want to create a public dotfiles repo to add to [PostHog/dotfiles](https://github.com/PostHog/dotfiles).

1. **Reference**: look at the existing entries in PostHog/dotfiles for structure ideas (most have an `ai/` or `.claude/` dir, shell rc files, `bin/` helpers, and an install script).

2. **Scan my home** for shareable config:
   - `~/.claude/` (CLAUDE.md, skills, commands, agents, hooks)
   - Shell rc (`~/.zshrc`, `~/.bashrc`, `~/.bash_profile`, `~/.config/fish/`)
   - Git (`~/.gitconfig`, `~/.gitignore_global`)
   - Tmux / editor (`~/.tmux.conf`, `~/.vimrc`, `~/.config/nvim/`)
   - Personal scripts on my `PATH` (`~/bin/`, `~/.local/bin/`)

3. **Filter out** before including a file:
   - PostHog-internal references (work email, internal hostnames, customer names, internal project paths)
   - Machine-specific absolute paths (`/Users/<me>/...`) — replace with `$HOME` or relative
   - Anything I'd be uncomfortable with a coworker reading

4. **Scrub secrets**. Grep each file and the git history of each file for:
   - API tokens, OAuth client secrets, access keys (look for `sk_`, `pk_`, long base64 blobs, `ghp_`, `xoxb-`)
   - SSH host blocks with internal hostnames (check `~/.ssh/config`)
   - Kubeconfigs, AWS/GCP creds
   - Anything matching common secret patterns

5. **Repo shape**:
   - Mirror my home layout (`zshrc` at root, `claude/`, `git/`, etc.)
   - `install.sh` that symlinks each file/dir into the right place
   - Short README explaining what's in it, how to install, and what's general-purpose vs PostHog-specific

6. **Push** public as `<my-github-username>/dotfiles` (or your preferred name).

7. **Add a row** to PostHog/dotfiles: clone the repo, add a row to the table in the README (`| Name | [repo link] | 1-line highlights |`), push to main.
