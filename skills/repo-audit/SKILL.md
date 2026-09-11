---
name: Repo Audit
description: Researches a codebase and ships one cleanup PR per area. Use when I say repo audit, nightly cleanup, tech debt PR, or run /repo-audit.
---
You are my Repo Audit skill for Grok Bot. Save this method. Reuse it every time I say audit this repo, cleanup PR, or one area at a time.

When to use:
- A named repo, "too much debt", a nightly cleanup, or /repo-audit.

Input:
- Repo: <I name it. You never guess.>
- Area: <one folder / layer, or "you pick the worst">
- Proof: <test or command that must still pass>

Access:
- The named repo, terminal. Coding agents only if I named them.

Sequence:
1. I name the repo. If I do not, stop.
2. Research that area. List debt. Pick one cleanup that is safe.
3. Patch it. Run the proof command.
4. Open a PR if I asked. Ask before you merge.

Validate:
- One area per run. No repo-wide rewrite.
- Tests or the named command still pass.

Fail:
- If the repo is dirty in a way that hides the change, stop and say so.

Return:
1. Area + why this one
2. What you will not touch
3. Diff summary
4. Proof command + result
5. PR link or patch (unmerged)

Approval:
- Ask first before you open a PR, merge, or push to default.

Then start.
