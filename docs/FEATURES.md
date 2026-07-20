# AntiLink features

AntiLink is organized around a Discord security workflow: detect threats,
enforce server policy, give moderators visibility, and provide recovery tools.

This page is a public overview. Availability varies by plan and by how a
server is configured. The
[current plan comparison](https://antil.ink/premium) and the
[official documentation](https://docs.antil.ink) are always the current source
for prices, options, and defaults.

## Link protection

- Phishing and malicious URL detection
- Discord invite and external-link controls
- Spam-link protection
- Link reputation checks through `/checklink`
- User, domain, role, channel, and category whitelists
- Configurable enforcement, warning escalation, and moderation logging

AntiLink never describes a link as guaranteed safe. A clean `/checklink` result
means that no known threat was found at the time of the check.

## Server defense

- **Emergency Lockdown** - tighten link and invite rules server-wide in one
  step, with an optional automatic unlock timer and an option to trigger on a
  detected raid
- **Scam Pattern Guard** - opt-in detection of common scam and impersonation
  phrasing that appears alongside a link, with a choice between flagging and
  removing
- **Member Defense** - protection at join time, covering join spikes, account
  screening, new-member link restrictions, and quarantine handling
- **Honeypot trap channels** - channels marked as traps, where posting is
  treated as suspicious. Defaults are deliberately conservative
- **Anti-Nuke** - protection against damage caused by a compromised or rogue
  administrator
- **Server Backup and Restore** - snapshots of your server structure and
  settings, restored additively so a restore never deletes what already exists.
  A backup can also be restored into another server you manage

You decide which roles and channels are exempt from automated action.

## Verify

A verification gate for new members.

- A button-based verification step that grants a verified role
- An optional captcha step
- An optional minimum account-age requirement

Configure it with `/verify` or on the dashboard.

## Custom Automod and native Discord AutoMod

AntiLink includes its own moderation filters and also configures Discord's
native AutoMod on your behalf.

Custom Automod preset filters, configured on the dashboard:

- Spam
- Bad words
- Duplicated text
- Repeated messages
- Caps
- Emoji spam
- Mass mentions

Each filter has its own response and its own channel and role exemptions, on
top of the global ignore lists. There is no slash command for Custom Automod;
it is configured entirely on the dashboard.

AntiLink also creates and maintains real Discord AutoMod rules as an additional
server-side layer, including Discord's own spam detection and its curated word
lists.

## AI assistant

AI Chat is a natural-language security assistant. Members talk to it in a
channel you choose. It answers questions about your configuration, blocked
events, suspicious links, permission problems, and general server security.

### What the AI can propose

The AI proposes. A human with the matching Discord permission approves. The AI
never applies anything by itself, and that approval step is the core safety
property of the feature.

- **Configuration changes** - protection toggles, and pointing a setting at a
  specific channel, role, mode, or number from a fixed list of settable fields
- **Whitelist changes** - adding or removing an entry
- **Moderation actions** - timeout, kick, ban, or clearing messages
- **Creating roles and channels**, including setting up log channels

Each proposal can only be approved by someone who already holds the Discord
permission for that action. A role created this way receives only permissions
the approving admin already holds, and Administrator is never grantable through
the AI.

### What the AI can do on its own

These are read-only or advisory and involve no server changes.

- Look up live security information on request
- Read a screenshot you attach, as text extraction only
- Follow server guidance you write for it, which shapes how it answers
- **Weekly AI Security Digest** - an opt-in weekly recap posted to a channel
  you choose

### AI Membership

AI Chat is not part of a server plan. It runs on an AI Membership, which is
owned by a user, is metered in tokens, and is linked to one server at a time.
The link can be changed, and one user may hold more than one membership.

Memberships are offered in Silver, Gold, and Platinum tiers, monthly or yearly.
Yearly billing is ten times the monthly price, so two months are free.

- The token pool resets on the 1st of each month
- Chat history retention is 3 days on Silver, 7 days on Gold, and 30 days on
  Platinum
- General, non-security conversation is available on Platinum only

Current tiers, token allowances, and prices are on the
[AntiLink AI page](https://antil.ink/ai).

## User Logs

Server event logging across every major server event type, covering messages,
members, roles, channels, threads, moderation, voice, invites, and server
settings.

- Each event type has its own toggle, its own destination channel, and its own
  embed color
- Configured on the dashboard

## Analytics

Per-server security analytics built from the activity AntiLink already records.

- Blocked activity over time, with a selectable period
- Breakdown by risk level and top blocked domains
- Member Defense activity
- CSV export

## Community Health

An opt-in view of how active your community is.

- Aggregate activity counts only. Message content is never stored or analyzed
- Message volume trends, member-count trends, and voice activity
- Most active and quietest channels, and busiest days
- An optional weekly report posted to a channel you choose

Community Health is available on AntiLink Plus.

## Custom Bot

Run AntiLink under your own bot identity, included with AntiLink Premium.

- Your own bot name, avatar, banner, description, and status
- The same protection engine and the same dashboard
- Configured from the dashboard once assigned

## Dashboard and visibility

- Discord OAuth authentication. AntiLink never asks for your Discord password
- Per-server security console covering every module above
- Protection logs, moderation actions, and a security audit log
- A record of configuration changes made from the dashboard
- Appeals management
- Public service status and incident reporting at
  [status.antil.ink](https://status.antil.ink)

## Commands

The public command set:

`/setup` `/config` `/notify` `/whitelist` `/language` `/premium` `/redeem`
`/antilink` `/checklink` `/lockdown` `/scamguard` `/guard` `/verify`
`/antinuke` `/backup` `/ai` `/chat`

Each command's options, permissions, and plan requirements are listed on the
[commands page](https://antil.ink/commands).

## Languages

AntiLink is localized into 24 languages across the bot, dashboard, website,
status page, and documentation.

English, Español, Français, Deutsch, Português (Brasil), Русский, 日本語, 한국어,
简体中文, Italiano, Türkçe, Polski, Nederlands, العربية, עברית, Svenska, Română,
Čeština, Ελληνικά, Magyar, Tiếng Việt, Українська, ไทย, 繁體中文.

Arabic and Hebrew are right-to-left. Set a server's bot language with
`/language` or on the dashboard. The websites choose a language per visitor,
separately from the server setting.

## Plans

- **AntiLink Basic** - free
- **AntiLink Plus**
- **AntiLink Premium** - the top tier, includes everything in Plus

Yearly billing is available. Payments are processed by Paddle as merchant of
record. Current plan details and prices are on the
[AntiLink pricing page](https://antil.ink/premium).

For detailed and current behavior, use the
[official documentation](https://docs.antil.ink).
