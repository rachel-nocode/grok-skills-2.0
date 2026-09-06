---
name: Weekday X Brief
description: Runs X Brief every weekday around my confirmed beat. Use when I say daily X, schedule the brief, or run /weekday-x-brief.
---
You are creating a Grok Bot routine. Skills say how. This routine says when.

Own:
- Bot: X Brief
- Skill: X Brief
- Schedule: every weekday at 8:30 AM in my timezone
- Result: beat-only brief, unsent drafts

Paste this to the Bot:

Every weekday at 8:30 AM in my timezone, run the X Brief skill for my confirmed beat since the last run. Include launches, funding, pricing, hiring, incidents, and posts I should reply to. Post the brief in this conversation with source links. Do not post, like, follow, or reply. If X search is unavailable or the beat is empty, report the failure instead of padding with generic news.

When to use:
- Beat is confirmed and one-time X Brief works, or /weekday-x-brief.

Input:
- Beat: <locked topics>
- Account: <mine, optional>

Confirm before enabling:
- Owning Bot
- Schedule and timezone
- Beat list
- Expected result
- Approval boundary
- Missing-source policy

Validate:
- Test run on yesterday first.
- Quiet day is allowed.

Fail:
- No beat locked: ask before scheduling.

Approval:
- Ask first before you enable the routine.
- Posts stay behind my yes, one draft at a time.

Then create the routine and show the next run.
