# giggle-stack

Thin overlay on [pstack](https://github.com/cursor/plugins/tree/main/pstack). `/giggle-mode` follows pstack's `/poteto-mode`, and adds one principle, Usefulness.

Official pstack stays installed. This repo does not copy pstack's principles, playbooks, or other skills.

## Requires

The official `pstack` plugin. Without it, `/giggle-mode` has nothing to route to.

## Install

Install pstack from the Cursor marketplace, and leave it installed:

```text
/add-plugin pstack
```

Import this repo as a Team Marketplace (Teams or Enterprise). On Enterprise, a team admin does this.

1. Open Dashboard → Plugins & MCPs.
2. Under Team Marketplaces, click Add Marketplace.
3. Choose Import from Repo and paste `https://github.com/nessamurmur/giggle-stack`.
4. Review the detected plugin, `giggle-stack`.
5. Under Marketplace Settings, set Marketplace Access. Turn on Auto Refresh if you want pushes to `main` to update the listing. Save.
6. Set the plugin to Default Off, Default On, or Required.

Default Off: each person installs `giggle-stack` from the team marketplace. Default On and Required install it for the group.

Grok Bot uses that same team marketplace.

## Use

In chat:

```text
/giggle-mode
```

The agent loads pstack's `poteto-mode` and follows it (principles, triggers, playbooks, subagents). It adds Usefulness under Core, after Experience First. Subagents and cloud agents it launches are told to work in `/giggle-mode`.

## Usefulness

Build a skateboard, then a bicycle, then a car. The first slice is something a user can use on prod that day. Thicken what people touch. Cut what they never reach.

A chat app's first thread is one hardcoded room, no auth, and a posted message visible on prod. Plan tickets as threads, not layers. Each day's work, PR, or stack is one thread, and it is finished before a new layer starts.

## Layout

```text
.cursor-plugin/marketplace.json
giggle-stack/.cursor-plugin/plugin.json
giggle-stack/skills/giggle-mode/SKILL.md
giggle-stack/skills/principle-usefulness/SKILL.md
```

Same split as [cursor/plugins](https://github.com/cursor/plugins): marketplace manifest at the repo root, plugin manifest inside the plugin directory, skills at `skills/<name>/SKILL.md`.

## License

MIT. New material copyright NJ. pstack-derived material remains copyright Lauren Tan. See [LICENSE](LICENSE).
