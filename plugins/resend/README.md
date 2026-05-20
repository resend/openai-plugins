# Resend Plugin

Use Resend in Codex to send transactional and marketing email, receive inbound email, build React Email templates, manage domains and templates, inspect delivery events, and follow deliverability best practices.

## Included skills

- `resend`
- `agent-email-inbox`
- `resend-cli`
- `react-email`
- `email-best-practices`

## What it covers

- Send transactional and batch email with Resend
- Receive inbound email with webhooks and safe processing patterns
- Build and render React Email templates
- Manage domains, templates, broadcasts, contacts, webhooks, logs, and automations
- Improve deliverability, compliance, and sending reliability

## Plugin structure

- `.codex-plugin/plugin.json` - plugin manifest with metadata and skill discovery
- `skills/` - the bundled Resend skill set used by Codex
- `assets/` - plugin-level icon referenced by the manifest

## Setup

Bundled skills are available after install. For live API calls, set your API key in the environment where Codex runs:

```bash
export RESEND_API_KEY=re_xxxxxxxxxxxxxxxxx
```

Codex uses that key through the Resend SDK, CLI, or API. No additional server or dependency needs to start.

## Notes

- The skills can still help with planning and code review when `RESEND_API_KEY` is not set.
- Sending, receiving, template management, and other live Resend API actions require `RESEND_API_KEY`.
