# Contributing

Keep changes small. Match pstack skill layout and frontmatter. Do not copy pstack playbooks or principle bodies into this repo.

## Ready to merge

- JSON valid. `.cursor-plugin/marketplace.json` and `giggle-stack/.cursor-plugin/plugin.json` parse as JSON and match the Cursor schemas in [cursor/plugins](https://github.com/cursor/plugins) (`schemas/marketplace.schema.json`, `schemas/plugin.schema.json`). `name` is kebab-case. `source` is `giggle-stack`. Paths are relative.
- Skills follow pstack conventions. Each skill is `giggle-stack/skills/<name>/SKILL.md` with `name` and `description` frontmatter. Principle skills set `disable-model-invocation: true`. `giggle-mode` only routes to `poteto-mode` and adds Usefulness under Core after Experience First.
- README accurate. It says this requires pstack, how to import and install the team marketplace, how to run `/giggle-mode`, and the Usefulness principle.
