# ClaudeSkills

Personal collection of Claude Code skills. Not a git repo, no build step.

## Layout

- `skills/<name>/SKILL.md` — one skill per folder. Frontmatter needs `name` and `description`; the description decides when the skill triggers, so name the concrete trigger phrases.
- `skills/<name>/references/` — longer docs the skill loads on demand. Keep SKILL.md short and point here.
- `skills/<name>/assets/` — templates and files the skill copies or fills in.
- `skills/<name>/facts/` — source data the skill draws from (e.g. resume facts). Never invent facts not in here.
- `coverage/` — reserved; currently empty.

## Skills

- `resume-builder` — builds resumes from `facts/` using templates in `assets/`.

## Rules

- New skill = new folder under `skills/`; copy the layout above, skip folders it doesn't need.
- Keep personal data inside `facts/`; don't copy it into SKILL.md or references.
