# Grok Skills 2.0

A Ko-fi-ready giveaway pack of **copy-paste Grok Bot skills**. Teach the Bot once. Reuse it. Every new skill is ask-first: it drafts the work, then stops before send, post, buy, delete, or publish.

## What it is

22 paste-ready skills plus a tiny static marketplace. Open a skill, copy the prompt, paste it into Grok Bot, then say:

> Save this as a skill named [Name]. Ask me before you send, post, buy, delete, or publish.

Next time, type `/` or say the skill name. No leftover 1.0 think/write skill names.

The previous think/write pack lives at [skills-4-grok](https://github.com/rachel-nocode/skills-4-grok).

## How to add a skill to Grok Bot

1. In the marketplace, click a skill, then **Copy Skill**.
2. Paste it into Grok Bot (or https://grok.com/).
3. Tell the Bot to save it as a skill with that name.
4. Or paste the raw file: `skills/<skill-id>/SKILL.md`

Each `SKILL.md` has YAML frontmatter (`name`, `description`) and the verbatim prompt body. The description includes when to use it so Grok Bot can pick the skill up again.

## How to run the marketplace

    npm install && npm run dev

Then open the local URL Astro prints (usually http://localhost:4321). Search, filter by category, and click a skill card.

    npm run build
    npm run preview

## The 10 Twitter-now skills (August 2026)

Pulled from what people are actually running: xAI's Aug 26 "Jobs Bots are doing today" list, the official [Grok Bot use cases](https://docs.x.ai/grok-bot/use-cases), and the launch-week threads (inbox first, then sales, then a chief-of-staff brief).

- skills/inbox-manager/SKILL.md -- Inbox Manager -- Inbox
- skills/sales-prospector/SKILL.md -- Sales Prospector -- Sales
- skills/digital-declutter/SKILL.md -- Digital Declutterer -- Ops
- skills/customer-support/SKILL.md -- Customer Support -- Ops
- skills/office-manager/SKILL.md -- Office Manager -- Ops
- skills/meeting-stand-in/SKILL.md -- Meeting Stand-in -- Ops
- skills/refunds-manager/SKILL.md -- Refunds Manager -- Money
- skills/morning-brief/SKILL.md -- Morning Brief -- Inbox
- skills/website-shipper/SKILL.md -- Website Shipper -- Build
- skills/talent-scout/SKILL.md -- Talent Scout -- Jobs

Approval on all ten: ask first. If you approve one item, the Bot does only that item.

## The original 12 action skills

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

## Previous pack

1.0 was the think/write pack: https://github.com/rachel-nocode/skills-4-grok
