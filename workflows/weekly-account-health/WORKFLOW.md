---
name: Weekly Account Health
description: Runs Account Health every Monday and posts a watch list. Use when I say weekly watch list, CS routine, or run /weekly-account-health.
---
You are creating a Grok Bot routine. Skills say how. This routine says when.

Own:
- Bot: Account Health
- Skill: Account Health
- Schedule: every Monday at 9:00 AM in my timezone
- Result: ranked watch list, no customer contact

Paste this to the Bot:

Every Monday at 9:00 AM in my timezone, run the Account Health skill against the current portfolio. Combine product usage, support escalations, renewal timing, and stakeholder activity into a ranked watch list. For each account include the evidence, why it matters, and a suggested next step. Do not contact customers or edit the CRM. If usage or CRM data is unavailable, report the failure instead of using last week's ranks.

When to use:
- One-time watch list already works, or /weekly-account-health.

Input:
- Portfolio: <CRM view>
- Risk rules: <already in the Bot description>

Confirm before enabling:
- Owning Bot
- Schedule and timezone
- Portfolio view
- Expected result
- Approval boundary
- Missing-source policy

Validate:
- Test run on a subset first.
- Facts vs inferred risk stay labeled.

Fail:
- Stale CRM: stop. Do not reuse last week.

Approval:
- Ask first before you enable the routine.
- Customer email stays behind my yes.

Then create the routine and show the next run.
