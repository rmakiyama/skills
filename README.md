# skills

Agent skills I use every day. Install them as Claude Code plugins, or as
standalone skills for any agent.

| plugin | contents |
| --- | --- |
| `development` | Git conventions for commits, branches, and pull requests, and code comment principles |
| `productivity` | General workflow tools, not code-specific |

## Install

As Claude Code plugins:

```
/plugin marketplace add rmakiyama/skills
/plugin install <plugin>@rmakiyama
```

As standalone skills (Claude Code, Cursor, Codex, Gemini CLI, and others):

```
# a single skill
gh skill install rmakiyama/skills productivity/imakita3 --agent claude-code --scope user

# every skill in this repository
gh skill install rmakiyama/skills --all --agent claude-code --scope user

# list what is available
gh skill install rmakiyama/skills
```

Skills live under `skills/<plugin>/<skill>/SKILL.md`.

## License

MIT
