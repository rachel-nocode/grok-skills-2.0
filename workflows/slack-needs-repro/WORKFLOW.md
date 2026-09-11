---
name: Slack Needs Repro
description: Starts Bug Reproduction when a Slack message needs a staging repro. Use when I say needs repro, Slack trigger, or run /slack-needs-repro.
---
You are creating a Grok Bot event routine. Skills say how. This routine says when.

Own:
- Bot: Bug Reproduction
- Skill: Bug Reproduction
- Trigger: Slack message in a named channel with a ticket link and "needs repro"
- Result: staging repro pack in this conversation, not posted back yet

Paste this to the Bot:

When a message in #customer-escalations contains a support ticket link and the phrase "needs repro," run the Bug Reproduction skill. Open the ticket, reproduce it in staging with a fresh test account, and post a repro pack in this conversation. Include exact steps, expected vs actual, screenshots, browser and OS, and console or network notes. Do not use production customer data. Never post back to Slack without approval. If staging is down or login is missing, report the failure instead of guessing a repro.

When to use:
- One-time staging repro already works, or /slack-needs-repro.

Input:
- Channel: <#customer-escalations or the one I name>
- Staging: <connected>
- Test account: <secure handoff, never in the routine text>

Confirm before enabling:
- Owning Bot
- Matching rule (narrow)
- Staging source
- Expected result
- Approval boundary
- Missing-source policy

Validate:
- Avoid "every new message." That burns usage.
- Test run with a fake ticket in a private channel first.

Fail:
- Broad listeners are a no. Narrow match or do not enable.

Approval:
- Ask first before you enable the routine.
- Slack posts and ticket status changes stay behind my yes.

Then create the routine and show how I test it.
