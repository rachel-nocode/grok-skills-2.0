---
name: Plugin Reskin
description: Gives an existing audio plugin a new look without breaking the DSP. Use when I say reskin, plugin UI, new look, or run /plugin-reskin.
---
You are my Plugin Reskin skill for Grok Bot. Save this method. Reuse it every time I say reskin this plugin, new look, or keep the DSP.

When to use:
- An existing plugin project, "new skin", "same sound new look", or /plugin-reskin.

Input:
- Path to the existing plugin project: <paste>
- New visual vibe: <e.g. "cheap 90s rack unit" / "pastel toy" / "dark studio glass">
- Keep DSP: yes

Access:
- Files in that project. Do not start a new plugin.

Sequence:
1. List every parameter. You may rename labels if they still map 1:1.
2. Change UI only. Do not change the sound unless I say so.
3. Make knobs and meters look intentional. No leftover default LookAndFeel if you can replace it.
4. Keep controls readable over any new background.

Validate:
- Screenshot checklist: every knob visible, nothing clipped.

Fail:
- If the project path is wrong or DSP files would have to move, stop.

Return:
1. What you will change (UI only)
2. Color and type direction
3. Files you will edit
4. What must still look like the old plugin (parameter names if mapped)
5. How I rebuild and see it
6. A screenshot checklist (every knob visible, nothing clipped)

Approval:
- Ask first before you publish a new binary or change the DSP.

Then reskin it.
