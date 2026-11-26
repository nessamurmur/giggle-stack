---
name: principle-usefulness
description: "Apply when planning a product, feature, or repo, or when slicing tickets or PRs. Build thin vertical slices a user can use on prod today, then thicken what usage proves."
disable-model-invocation: true
---

# Usefulness

Build a skateboard, then a bicycle, then a car. Ship it to prod first, and thicken it from use.

- Name the thread as a user outcome, not as a layer
- The first PR is usable on prod that day
- Hardcode, stub, or skip a layer until a thread needs it
- Keep every slice usable on prod. If not, finish the thread, not a new layer.
- Thicken what people touch. Cut what they never reach.

A chat app's first thread is one hardcoded room, no auth, and a posted message visible on prod. Plan tickets as threads, not layers. Sequence work into verifiable units checks that a step is green. Usefulness checks that the green step is usable on prod.

Red flags:

- Layer-by-layer or "infra first" plans with no user path
- Deploy or a demo left off prod
- Features nobody can reach
- A rewrite that drops the old working path first
