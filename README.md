# Grok Skills 2.0

A Ko-fi-ready giveaway pack of **copy-paste Grok Bot skills and routines**. Teach the Bot once. Reuse it. Every new skill is ask-first: it drafts the work, then stops before send, post, buy, delete, or publish.

Skills say **how**. Routines say **when**. Templates are the shareable Bot (identity + skills + routines) with secrets stripped.

## What it is

34 paste-ready skills, 10 routines, plus a tiny static marketplace. Open a card, copy the prompt, paste it into Grok Bot, then say:

> Save this as a skill named [Name]. Ask me before you send, post, buy, delete, or publish.

For a routine:

> Create this as a routine on the [Bot] that owns this job. Show me the next run. Do not enable until I confirm.

Next time, type `/` or say the skill name. Use `@` for Bots, groups, routines, and connectors.

The previous think/write pack lives at [skills-4-grok](https://github.com/rachel-nocode/skills-4-grok).

## How to add a skill to Grok Bot

1. In the marketplace, click a skill, then **Copy Skill**.
2. Paste it into Grok Bot (or the Grok Bot app).
3. Tell the Bot to save it as a skill with that name.
4. Or paste the raw file: `skills/<skill-id>/SKILL.md`

Each `SKILL.md` has YAML frontmatter (`name`, `description`) and the verbatim prompt body. The description includes when to use it so Grok Bot can pick the skill up again.

## How to add a routine

1. Run the matching skill once on a real, safe input.
2. Copy the routine card (or `workflows/<id>/WORKFLOW.md`).
3. Paste it into the Bot that should own the job.
4. Confirm Bot, schedule or event, source, result, approval boundary, and missing-source policy.
5. Use **Test run**. A test run does real work.
6. Enable only after it stops at the approval point.

Routines can run while your laptop is closed. Keep send, buy, delete, and publish behind approval. If source data is missing, the routine must report the failure instead of using old data.

## How to share a template

Grok Bot can share a Bot as a public template. The link exposes configuration (identity, description, skills, routines). It does not give anyone your computer, logins, or conversation history.

1. Get the Bot working on real tasks.
2. Run **Template Packager** (`skills/template-packager/SKILL.md`).
3. Strip API keys, internal URLs, customer data, and private emails.
4. Copy the share link from the Bot. Recipients preview on x.ai and choose Add to Grok Bot.

Do not share a template until the secret-strip list is empty.

## How to run the marketplace

    npm install && npm run dev

Then open the local URL Astro prints (usually http://localhost:4321). Search, filter by category, and click a skill or routine card.

    npm run build
    npm run preview

## Skills vs routines vs templates

| Piece | Owns | File |
| --- | --- | --- |
| Skill | How to do the job | `skills/<id>/SKILL.md` |
| Routine | When to run it (schedule or event) | `workflows/<id>/WORKFLOW.md` |
| Template | Shareable Bot: description + skills + routines | Built in Grok Bot after you strip secrets |

A useful skill still states: when to use it, inputs and access, sequence, how to validate, what to return, and what requires approval. This pack also adds a fail / no-stale-data rule so scheduled runs do not hallucinate from last week.

## The 10 Twitter-now skills

Pulled from what people are actually running: xAI's "Jobs Bots are doing today" list, the official [Grok Bot use cases](https://docs.x.ai/grok-bot/use-cases), and the launch-week threads (inbox first, then sales, then a chief-of-staff brief).

- skills/inbox-manager/SKILL.md -- Inbox Manager -- Inbox -- Inbox Sweep
- skills/sales-prospector/SKILL.md -- Sales Prospector -- Sales -- Nightly Outbound Research
- skills/digital-declutter/SKILL.md -- Digital Declutterer -- Ops -- Subscription Watchdog
- skills/customer-support/SKILL.md -- Customer Support -- Ops -- Support Triage
- skills/office-manager/SKILL.md -- Office Manager -- Ops
- skills/meeting-stand-in/SKILL.md -- Meeting Stand-in -- Ops
- skills/refunds-manager/SKILL.md -- Refunds Manager -- Money
- skills/morning-brief/SKILL.md -- Morning Brief -- Inbox -- Weekday Morning Brief
- skills/website-shipper/SKILL.md -- Website Shipper -- Build
- skills/talent-scout/SKILL.md -- Talent Scout -- Jobs

Approval on all ten: ask first. If you approve one item, the Bot does only that item.

## Official-job skills (added after templates shipped)

xAI's use-case page names jobs this pack did not cover. These fill that hole.

- skills/paid-media/SKILL.md -- Paid Media -- Growth -- Paid Media Pulse
- skills/expense-manager/SKILL.md -- Expense Manager -- Money -- Weekly Expense Reconcile
- skills/account-health/SKILL.md -- Account Health -- Sales -- Weekly Account Health
- skills/product-performance/SKILL.md -- Product Performance -- Build
- skills/bug-reproduction/SKILL.md -- Bug Reproduction -- QA -- Slack Needs Repro

## Template-era skills

Jobs people are actually packaging as shareable Bots: a beat brief, an outer loop above coding agents, a decision register, deal prep, growth drafts, compounding research, and a secret-safe share checklist.

- skills/x-brief/SKILL.md -- X Brief -- Growth -- Weekday X Brief
- skills/engineering-loop/SKILL.md -- Engineering Loop -- Build
- skills/decision-witness/SKILL.md -- Decision Witness -- Ops
- skills/deal-prep/SKILL.md -- Deal Prep -- Money
- skills/growth-desk/SKILL.md -- Growth Desk -- Growth
- skills/research-dossier/SKILL.md -- Research Dossier -- Research
- skills/template-packager/SKILL.md -- Template Packager -- Automation

## The original 12 action skills

Same jobs as 2.0 launch. Now they use the same when / input / access / sequence / validate / fail / return / approval shape as the rest of the pack.

- skills/audio-plugin-builder/SKILL.md -- Audio Plugin Builder -- Music
- skills/vibe-code-tiny-tool/SKILL.md -- Vibe-Code a Tiny Tool -- Build
- skills/job-apply/SKILL.md -- Job Apply -- Jobs
- skills/qa-live-url/SKILL.md -- QA a Live URL -- QA
- skills/broken-repo-medic/SKILL.md -- Broken-Repo Medic -- Build
- skills/plugin-reskin/SKILL.md -- Plugin Reskin -- Music
- skills/store-listing-pack/SKILL.md -- Store-Listing Pack -- Shipping
- skills/cheap-model-crew/SKILL.md -- Cheap-Model Crew -- Automation
- skills/lofi-radio-page/SKILL.md -- Lofi Radio Page -- Music
- skills/interview-drill/SKILL.md -- Interview Drill -- Jobs
- skills/cover-letter-in-their-voice/SKILL.md -- Cover Letter in Their Voice -- Jobs
- skills/should-i-buy-this/SKILL.md -- Should I Buy This -- Money

## Routines

- workflows/weekday-morning-brief/WORKFLOW.md -- Weekday Morning Brief
- workflows/nightly-outbound-research/WORKFLOW.md -- Nightly Outbound Research
- workflows/weekly-account-health/WORKFLOW.md -- Weekly Account Health
- workflows/weekly-expense-reconcile/WORKFLOW.md -- Weekly Expense Reconcile
- workflows/weekday-x-brief/WORKFLOW.md -- Weekday X Brief
- workflows/inbox-sweep/WORKFLOW.md -- Inbox Sweep
- workflows/support-triage/WORKFLOW.md -- Support Triage
- workflows/subscription-watchdog/WORKFLOW.md -- Subscription Watchdog
- workflows/paid-media-pulse/WORKFLOW.md -- Paid Media Pulse
- workflows/slack-needs-repro/WORKFLOW.md -- Slack Needs Repro (event)

## Previous pack

1.0 was the think/write pack: https://github.com/rachel-nocode/skills-4-grok
