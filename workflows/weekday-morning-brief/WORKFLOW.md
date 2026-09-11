---
name: Weekday Morning Brief
description: Runs Morning Brief every weekday and posts a source-linked digest. Use when I say schedule the brief, every morning, or run /weekday-morning-brief.
---
You are creating a Grok Bot routine. Skills say how. This routine says when.

Own:
- Bot: Chief of Staff / Morning Brief
- Skill: Morning Brief
- Schedule: every weekday at 8:00 AM in my timezone
- Result: source-linked digest in this conversation

Paste this to the Bot:

Every weekday at 8:00 AM in my timezone, run the Morning Brief skill against my connected inbox, calendar, and chat since the last run. Post a linked digest in this conversation. Return only items that map to my current priorities. For each item include the source, why it matters, the next step, and whether I owe a yes/no. Do not send messages, accept meetings, or change the calendar. If a source is disconnected or empty, report the failure instead of using old data.

When to use:
- The skill already works on a one-time run, or /weekday-morning-brief.

Input:
- Timezone: <mine>
- Sources: <inbox / calendar / Slack, already connected>
- Priorities: <locked 3, or "use what you already know">

Confirm before enabling:
- Owning Bot
- Schedule and timezone
- Input source
- Expected result
- Approval boundary
- Missing-source policy

Validate:
- Test run uses real tools. Use a quiet morning first.
- Stop at the digest. No outbound send.

Fail:
- No current data: say so. Do not reuse yesterday's brief.

Approval:
- Ask first before you enable the routine.
- Sending, booking, and calendar edits stay off unless I approve one item.

Then create the routine and show the next run.
