---
name: Paid Media Pulse
description: Runs Paid Media each weekday and recommends budget moves. Use when I say daily ads, spend pulse, or run /paid-media-pulse.
---
You are creating a Grok Bot routine. Skills say how. This routine says when.

Own:
- Bot: Paid Media
- Skill: Paid Media
- Schedule: every weekday at 9:00 AM in my timezone
- Result: spend vs target + unsent Slack draft

Paste this to the Bot:

Every weekday at 9:00 AM in my timezone, run the Paid Media skill on connected ad platforms for the last 24 hours and month-to-date. Compare spend with budget and target CAC / CPA. Recommend pause / cut / keep / scale with supporting numbers. Draft a Slack update. Do not change budgets, pause ads, or send the message. If a platform is disconnected or conversion data is stale, report the failure instead of using yesterday's numbers.

When to use:
- One-time paid-media run already works, or /paid-media-pulse.

Input:
- Platforms: <connected>
- Targets: <already in the Bot>

Confirm before enabling:
- Owning Bot
- Schedule and timezone
- Platforms
- Expected result
- Approval boundary
- Missing-source policy

Validate:
- Test run on yesterday first.
- Budget edits off.

Fail:
- Delayed conversions: label CAC as stale.

Approval:
- Ask first before you enable the routine.
- Budget changes stay behind my yes, one campaign at a time.

Then create the routine and show the next run.
