---
name: giggle-mode
description: >-
  NJ's agent style on top of pstack. /giggle-mode follows poteto-mode in
  full and adds Usefulness: thin vertical slices usable on prod, thickened
  from use. Use for /giggle-mode or requests to work in this style.
disable-model-invocation: true
mode: true
icon: lightbulb
color: green
reminder: New task? Apply /giggle-mode. Casual turn or user opts out -> don't.
---

# Giggle mode

Thin router over pstack's `poteto-mode`. `/giggle-mode` works like `/poteto-mode`.

**Requires** `pstack` and `cursor-team-kit`. `poteto-mode` is slash-only and hidden from the skill list. Find the visible `setup-pstack` skill, read `../poteto-mode/SKILL.md` relative to its directory, and keep that path for its bundled playbooks (`../poteto-mode/playbooks/<name>.md`). Follow that file in full. Tell the user to run `/add-plugin pstack` only if that file is missing. `/deslop` comes from `cursor-team-kit`. It is installed when `deslop` is in the skill list. If it is missing, stop and tell the user to run `/add-plugin cursor-team-kit`.

## Principle added

Poteto-mode's principle set, plus **Usefulness** under **Core**, immediately after **Experience First**:

- **Usefulness.** Planning a product, feature, or repo, or slicing tickets and PRs. Build thin vertical slices a user can use on prod today, then thicken what usage proves.

Leaf: `principle-usefulness` (`../principle-usefulness/SKILL.md` from this file). Load the leaf when you apply it. Cite it the way poteto-mode cites a principle: the name and the choice it changed, and only after you have read the leaf this session.

## Gate

Plan each day's work, PR, or stack as one usable thread, and finish that thread in as few changes as possible. Before opening a PR or ending the day's work, answer: can the user do the thread's outcome on prod now? If not, the next change finishes the thread rather than starting a new layer.

## Subagents and cloud agents

Follow poteto-mode for how you spawn and kick off agents. Every subagent or cloud agent kickoff says to work in `/giggle-mode`. If the receiving agent may not have giggle-stack installed (any cloud agent), paste the full body of `principle-usefulness` into the kickoff so it applies the principle anyway.
