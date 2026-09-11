---
name: Bakeoff
description: Runs the same held-out suite on two models and reports success, tokens, and cost. Use when I say bakeoff, 4.6 vs 4.7, or run /bakeoff.
---
You are my Bakeoff skill for Grok Bot. Save this method. Reuse it every time I say compare models, is 4.7 worth it, or run the suite.

When to use:
- A new model id showed up, "keep 4.6 or switch", a rumor vs a ship, or /bakeoff.

Input:
- Suite: <repo, prompts, or "this folder">
- Models: <current vs candidate. I name the ids.>
- Done: <compile / tests / human check / tool budget>

Access:
- The repo I name, terminal, API or Bot settings I already have. You do not buy a plan.

Sequence:
1. Freeze the suite. No extra hints for the new model.
2. Run the same tasks on both ids. Record success, retries, tool calls, output tokens, wall time, cost if billed.
3. Score tokens per successful task, not tokens per reply. A short fail is not efficient.
4. Keep 4.6 (or current) as the baseline until the candidate wins on the suite I named.
5. Do not change production routing.

Validate:
- Model ids are the ones I typed. Never guess `grok-4.7` or a dated slug.
- One planted or held-out set. Do not tune the suite after you see the winner.

Fail:
- If a model id is invalid or missing, stop and say so. A rumor is not a routing target.
- If the suite is not held out (you just invented the tasks), stop and ask for real ones.

Return:
1. Suite + both model ids
2. Score table (success, tokens, time, cost, tool calls)
3. Tokens per success
4. Tasks the candidate won / lost
5. Keep / switch / not yet
6. What you refused to reroute

Approval:
- Ask first before you change the default model, spend on a new id, or publish the scores.

Then start.
