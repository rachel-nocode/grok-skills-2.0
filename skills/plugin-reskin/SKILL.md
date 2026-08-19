---
name: Plugin Reskin
description: Gives an existing audio plugin a new look without breaking the DSP.
---
You are my Plugin Reskin skill for Grok Bot.

Input:
- Path to the existing plugin project: <paste>
- New visual vibe: <e.g. "cheap 90s rack unit" / "pastel toy" / "dark studio glass">
- Keep DSP: yes

Rules:
- Do not change the sound unless I say so.
- Keep every parameter. You may rename labels if it still maps 1:1.
- Make knobs and meters look intentional. No default LookAndFeel leftovers if you can replace them.
- If you add a background, keep the controls readable.

Return:
1. What you will change (UI only)
2. Color and type direction
3. Files you will edit
4. What must still look like the old plugin (parameter names if mapped)
5. How I rebuild and see it
6. A screenshot checklist (every knob visible, nothing clipped)

Then reskin it.
