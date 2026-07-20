# AntiLink

AntiLink is a Discord Server Security Center built to protect communities from
phishing, malicious URLs, spam links, unwanted Discord invites, raids, and
other common abuse.

AntiLink combines real-time protection in Discord with a web dashboard,
moderation visibility, public documentation, and service status reporting.

## Get started

| Resource | Link |
| --- | --- |
| Website | [antil.ink](https://antil.ink) |
| Add AntiLink | [invite.antil.ink](https://invite.antil.ink) |
| Dashboard | [dashboard.antil.ink](https://dashboard.antil.ink) |
| Documentation | [docs.antil.ink](https://docs.antil.ink) |
| Commands | [antil.ink/commands](https://antil.ink/commands) |
| Service status | [status.antil.ink](https://status.antil.ink) |
| Support | [support.antil.ink](https://support.antil.ink) |

## Protection at a glance

- Real-time phishing, malicious URL, spam-link, and invite protection
- Link reputation checks with `/checklink`
- User, domain, role, channel, and category whitelists
- Custom Automod filters for spam, bad words, duplicated text, repeated messages,
  caps, emoji spam, and mass mentions
- Native Discord AutoMod rules, added as a server-side layer alongside AntiLink's
  own filters
- Emergency Lockdown, Scam Guard, Honeypot, and Member Defense
- Verification with an optional captcha step and an optional account-age gate
- Anti-Nuke protection and Server Backup and Restore
- User Logs: server event logging across every major server event type, into the
  channels you choose
- Moderation logs, appeals, and security audit visibility
- Per-server security analytics, with CSV export
- Community Health: opt-in activity trends built from aggregate counts only,
  never message content
- Custom Bot: run AntiLink under your own bot identity, including name, avatar,
  banner, status, and description
- AI Chat: a natural-language security assistant that checks links, explains your
  configuration, and can propose changes for an admin to approve. AI Chat is sold
  as a separate AI Membership, not as part of a server plan.
- Weekly AI Security Digest: an opt-in weekly recap of your server's protection
- Dashboard management through Discord OAuth
- Bot and dashboard localization across 24 languages
- Public status reporting and incident history

AntiLink never describes a link as guaranteed safe. A clean `/checklink`
result means that no known threat was found at the time of the check.

## Plans

Server plans apply to a single server.

- **AntiLink Basic** - Essential protection for free
- **AntiLink Plus** - Full link protection and expanded controls
- **AntiLink Premium** - Advanced server defense and the full security suite

### AI Membership

AI Chat runs on an AI Membership, which is separate from the server plans above.
A membership is held by a user, is metered in monthly tokens, and is linked to
one server at a time. It is offered in Silver, Gold, and Platinum tiers, monthly
or yearly.

Current server plan details and pricing are on the
[AntiLink pricing page](https://antil.ink/premium). Current AI Membership tiers
and pricing are on the [AntiLink AI page](https://antil.ink/ai).

## Trust and transparency

- Dashboard access uses Discord OAuth. AntiLink never asks for your Discord password.
- AI Chat proposes changes. Nothing is applied until a human who holds the matching
  Discord permission approves it.
- Community Health records aggregate activity counts only, never message content.
- Public legal documents are available in the
  [AntiLink documentation](https://docs.antil.ink/legal/privacy).
- Live service information is published at
  [status.antil.ink](https://status.antil.ink).
- Security reports should follow the instructions in
  [SECURITY.md](SECURITY.md).

## Repository scope

This public repository contains product information and public documentation
only. AntiLink's bot, dashboard, infrastructure, detection logic, and other
implementation source code are proprietary and maintained in private
repositories.

Public access to this repository does not grant permission to copy, reproduce,
redistribute, reverse engineer, or operate the private AntiLink software.

## Support

For setup help, bug reports, account questions, or service assistance, read
[SUPPORT.md](SUPPORT.md) or join the
[AntiLink support server](https://support.antil.ink).

Copyright 2026 AntiLink. All rights reserved.
