> **Moved:** this skill now lives in [cbzehner/skills](https://github.com/cbzehner/skills) under `skills/spike/`. This repo is archived and read-only.

# Spike

Run a disposable experiment before committing to a plan. The skill keeps uncertainty small by testing API shape, library behavior, performance, UI ideas, or integration risk directly.

## Use It For

- Answering “will this even work?”
- Trying a library before designing around it
- Reducing implementation risk with a timeboxed prototype

## Install

Clone the repo and run the installer:

```bash
git clone https://github.com/cbzehner/skill-spike.git
cd skill-spike
./install.sh all
```

Install targets:

- `./install.sh claude` installs to `~/.claude/skills/spike`
- `./install.sh codex` installs to `~/.codex/skills/spike`
- `./install.sh agents` installs to `~/.agents/skills/spike`
- `./install.sh opencode` installs to `~/.config/opencode/skills/spike`
- `./install.sh all --copy` copies files instead of symlinking

Manual install works too: symlink or copy `skills/spike` into your agent's skills directory.

## Agent Support

This repo uses the plain `skills/spike/SKILL.md` layout. Claude Code and Codex also get small plugin manifests at `.claude-plugin/plugin.json` and `.codex-plugin/plugin.json`.

Other agents can read the same `SKILL.md` file. If a host does not support a frontmatter field or tool name, ignore that field and follow the workflow text.

## Layout

```text
.claude-plugin/plugin.json
.codex-plugin/plugin.json
install.sh
skills/spike/SKILL.md
README.md
LICENSE
```

## Public Notes

These repos are public. Keep private repo names, secrets, customer data, raw logs, cookies, and absolute filesystem paths out of examples.

## License

MIT