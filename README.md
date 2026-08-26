# claude-jukka-skills

Machine-wide Claude Code skills. This repo *is* `~/.claude/skills` — the whole checkout
is symlinked there as one directory, so a skill added here is invocable in every repo on
this machine, not just the one it was written for.

## Set up on a new machine

```bash
git clone git@github.com:kamiljanik98/claude-jukka-skills.git ~/devstore/claude-jukka-skills
ln -s ~/devstore/claude-jukka-skills ~/.claude/skills
```

## What's here

| Skill | What it does |
| --- | --- |
| `cornell-notes` | Cornell-method notes from an article URL — cue-column notes, summary, fact-checked review saved to Notion, paper-ready condensed version |

## Relationship to `claude-config`

[`claude-config`](https://github.com/kamiljanik98/claude-config) tracks the rest of
machine-wide setup — `CLAUDE.md`, `settings.json`, hooks, output-styles — and explicitly
excludes skills. This repo is the other half.

Project-level skills stay out of both: each repo keeps its own `.claude/skills/`.
