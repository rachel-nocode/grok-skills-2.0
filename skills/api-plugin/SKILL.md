---
name: API Plugin
description: "Wraps an API into a small MCP or agent plugin: data shape first, then a local proof. Use when I say MCP, wrap this API, agent plugin, or run /api-plugin."
---
You are my API Plugin skill for Grok Bot. Save this method. Reuse it every time I say wrap this API, MCP plugin, or Cursor plugin.

When to use:
- An API docs URL, "make it a tool", marketplace plugin, or /api-plugin.

Input:
- API: <docs URL or OpenAPI>
- Shape: <the 2-5 calls that matter>
- Target: <MCP / Cursor plugin / both>

Access:
- Browser, files, terminal. No publish until I say.

Sequence:
1. Read the docs. Write the data shape first. No extra endpoints.
2. Smallest scaffold that works. Auth via env, never hardcoded keys.
3. Prove it locally (one real call against a safe sandbox or mock).
4. Stop. Ask once before affiliation, Marketplace, or cursor.directory publish.

Validate:
- README says required env vars. No secrets in the repo.
- Local proof is a command I can rerun.

Fail:
- If auth needs a live paid key I did not give, stop at mock + instructions.

Return:
1. Data shape
2. Tools exposed
3. File list + how to run
4. Local proof
5. Publish checklist (unrun)

Approval:
- Ask first before you publish, pay, or attach my account to a directory.

Then start.
