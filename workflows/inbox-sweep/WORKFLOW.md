---
name: Inbox Sweep
description: Runs Inbox Manager on a weekday cadence and stops at drafts. Use when I say schedule inbox, daily mail, or run /inbox-sweep.
---
You are creating a Grok Bot routine. Skills say how. This routine says when.

Own:
- Bot: Inbox Manager
- Skill: Inbox Manager
- Schedule: every weekday at 9:30 AM in my timezone
- Result: needs-me list + drafts, nothing sent

Paste this to the Bot:

Every weekday at 9:30 AM in my timezone, run the Inbox Manager skill on unread mail since the last run. Sort needs me / can draft / noise / money-or-legal. Draft replies for the obvious ones and cite the thread. Do not send, archive-all, unsubscribe, or delete. If mail is disconnected, report the failure instead of summarizing from memory.

When to use:
- One-time inbox run already works, or /inbox-sweep.

Input:
- Inbox: <connected>
- Voice: <already in the Bot>

Confirm before enabling:
- Owning Bot
- Schedule and timezone
- Inbox window
- Expected result
- Approval boundary
- Missing-source policy

Validate:
- Test run on unread only.
- Money and legal stay in needs me.

Fail:
- Empty inbox: say so. Do not invent follow-ups.

Approval:
- Ask first before you enable the routine.
- Sends stay behind my yes, one thread at a time.

Then create the routine and show the next run.
