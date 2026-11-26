---
name: giggle-mode
description: >-
  Giggle's agent style on top of pstack. /giggle-mode follows poteto-mode in
  full and adds Usefulness: thin vertical slices usable on prod, thickened
  from use. Use for giggle, /giggle-mode, or requests to work in this style.
disable-model-invocation: true
mode: true
icon: lightbulb
color: green
reminder: New task? Apply /giggle-mode. Casual turn or user opts out -> don't.
---

# Giggle mode

Thin router over pstack's `poteto-mode`. `/giggle-mode` works like `/poteto-mode`.

**Requires** the official `pstack` plugin, installed alongside this one. Load pstack's `poteto-mode` and follow it in full: its principles, non-negotiable triggers, playbooks, autonomy, subagent machinery, and reply rules. Do not copy that body into this file. If `poteto-mode` is missing, stop and tell the user to install pstack.

## Principle added

Poteto-mode's principle set, plus **Usefulness** under **Core**, immediately after **Experience First**:

- **Usefulness.** Planning a product, feature, or repo, or slicing tickets and PRs. Build thin vertical slices a user can use on prod today, then thicken what usage proves.

Leaf: `principle-usefulness` (`../principle-usefulness/SKILL.md` from this file). Load the leaf when you apply it. Cite it the way poteto-mode cites a principle: the name and the choice it changed, and only after you have read the leaf this session.

## Subagents and cloud agents

Follow poteto-mode for how you spawn and kick off agents. Any subagent or cloud agent this mode launches must also be told to work in `/giggle-mode`. Put this file's absolute path in that kickoff so it can load `principle-usefulness`.
