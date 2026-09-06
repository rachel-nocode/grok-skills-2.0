---
name: Weekly Expense Reconcile
description: Runs Expense Manager once a week and leaves follow-up drafts. Use when I say weekly expenses, receipt sweep, or run /weekly-expense-reconcile.
---
You are creating a Grok Bot routine. Skills say how. This routine says when.

Own:
- Bot: Expense Manager
- Skill: Expense Manager
- Schedule: every Friday at 4:00 PM in my timezone
- Result: summary + unsent follow-ups

Paste this to the Bot:

Every Friday at 4:00 PM in my timezone, run the Expense Manager skill for this week's expenses. Match receipts from the finance inbox, flag missing categories or policy exceptions with a policy citation, and draft one follow-up per owner. Return the summary and drafts in this conversation. Do not send messages or change reimbursements. If the expense system is unavailable, report the failure instead of using last week's sheet.

When to use:
- One-time reconcile already works, or /weekly-expense-reconcile.

Input:
- System: <connected expense app>
- Policy: <already in the Bot, or paste>

Confirm before enabling:
- Owning Bot
- Schedule and timezone
- Expense source
- Expected result
- Approval boundary
- Missing-source policy

Validate:
- Test run on this week only.
- Totals reconcile to the source.

Fail:
- No receipts and no lines: say empty. Do not invent spend.

Approval:
- Ask first before you enable the routine.
- Sends and reimbursement edits stay behind my yes.

Then create the routine and show the next run.
