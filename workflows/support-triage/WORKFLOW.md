---
name: Support Triage
description: Runs Customer Support on new tickets and leaves policy-safe drafts. Use when I say schedule support, ticket routine, or run /support-triage.
---
You are creating a Grok Bot routine. Skills say how. This routine says when.

Own:
- Bot: Customer Support
- Skill: Customer Support
- Schedule: every weekday at 10:00 AM and 3:00 PM in my timezone
- Result: triaged tickets + unsent drafts

Paste this to the Bot:

Every weekday at 10:00 AM and 3:00 PM in my timezone, run the Customer Support skill on new tickets since the last run. Sort answer / refund-or-replace / escalate / spam. Draft policy-safe replies using only facts in the thread. Quote the policy line. Draft refund actions but do not run them. Do not send, refund, cancel, or change an order. If the inbox or policy is missing, report the failure instead of guessing.

When to use:
- One-time support run already works, or /support-triage.

Input:
- Inbox: <connected>
- Policy: <already in the Bot>

Confirm before enabling:
- Owning Bot
- Schedule and timezone
- Ticket source
- Expected result
- Approval boundary
- Missing-source policy

Validate:
- Test run on a small unread set.
- Refunds stay drafted.

Fail:
- No new tickets: say idle. Do not re-triage old ones.

Approval:
- Ask first before you enable the routine.
- Sends and refunds stay behind my yes.

Then create the routine and show the next run.
