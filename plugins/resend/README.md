# Resend Plugin

This plugin packages Resend email workflows in `plugins/resend`.

It currently includes these skills:

- `resend`
- `agent-email-inbox`
- `resend-cli`
- `react-email`
- `email-best-practices`

## What It Covers

- transactional email sending and template workflows with Resend
- inbound email handling, webhook verification, and agent inbox patterns
- React Email authoring and sending guidance
- Resend CLI workflows for operational tasks
- deliverability and compliance best practices

## Plugin Structure

- `.codex-plugin/plugin.json` — plugin manifest with metadata and skill discovery
- `skills/` — the bundled Resend skill set used by Codex
- `assets/` — plugin-level icon referenced by the manifest

## Setup

Bundled skills are available immediately after install. To run live Resend API workflows, set your API key in the environment where Codex runs:

```bash
export RESEND_API_KEY=re_xxxxxxxxxxxxxxxxx
```

Skills teach the agent to call the Resend API (via the SDK, CLI, or raw HTTP) using that key. No additional server or dependency needs to start.

## Notes

- Skills-only guidance can still help even if `RESEND_API_KEY` is not set.
- Sending, receiving, template management, and other live Resend API actions require `RESEND_API_KEY`.
