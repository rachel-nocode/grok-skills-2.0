---
name: Subscription Watchdog
description: Runs Digital Declutterer weekly and flags trials and renewals. Use when I say watchdog, trial ending, subscription sweep, or run /subscription-watchdog.
---
You are creating a Grok Bot routine. Skills say how. This routine says when.

Own:
- Bot: Digital Declutterer
- Skill: Digital Declutterer
- Schedule: every Sunday at 5:00 PM in my timezone
- Result: paid list + cancel paths, nothing cancelled

Paste this to the Bot:

Every Sunday at 5:00 PM in my timezone, run the Digital Declutterer skill on email and billing for the last 7 days. Inventory first. Flag trials converting, renewals, and price changes. Return keep / maybe / junk / paid with price and cancel path. Do not unsubscribe, trash, cancel, or revoke access. If billing pages will not open, report the failure instead of guessing prices.

When to use:
- One-time declutter already works, or /subscription-watchdog.

Input:
- Surfaces: <email / billing>
- Keep list: <already in the Bot>

Confirm before enabling:
- Owning Bot
- Schedule and timezone
- Surfaces
- Expected result
- Approval boundary
- Missing-source policy

Validate:
- Test run on last 7 days only.
- 2FA and recovery mail stay in keep.

Fail:
- Unknown charge: mark unknown. Do not cancel it.

Approval:
- Ask first before you enable the routine.
- Cancels stay behind my yes, one item at a time.

Then create the routine and show the next run.
