---
name: Nightly Outbound Research
description: Runs Sales Prospector overnight and leaves a review list. Use when I say nightly outbound, research while I sleep, or run /nightly-outbound-research.
---
You are creating a Grok Bot routine. Skills say how. This routine says when.

Own:
- Bot: Sales Outbound
- Skill: Sales Prospector
- Schedule: every weeknight at 9:00 PM in my timezone
- Result: ranked review list with drafts, unsent

Paste this to the Bot:

Every weeknight at 9:00 PM in my timezone, run the Sales Prospector skill against the current CRM view I named. Score accounts against my ICP and recent intent, identify up to three contacts per account, and draft email and LinkedIn in my voice samples. Skip anyone already in an active sequence. Return a review list in this conversation. Do not send, enroll, connect, or edit the CRM. If the CRM view is empty or disconnected, report the failure instead of using last night's list.

When to use:
- One-time prospecting already works, or /nightly-outbound-research.

Input:
- CRM view: <name it>
- ICP + offer: <already in the Bot, or paste>
- Cap: <25 accounts unless I say otherwise>

Confirm before enabling:
- Owning Bot
- Schedule and timezone
- CRM view name
- Expected result
- Approval boundary
- Missing-source policy

Validate:
- Test run on a small view first.
- Every score has a source from that night.

Fail:
- No CRM: stop. Do not invent accounts.

Approval:
- Ask first before you enable the routine.
- Sends stay behind my yes, one account at a time.

Then create the routine and show the next run.
