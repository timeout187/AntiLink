# Security Suite

AntiLink is organized as a set of security modules. Each one is optional, each one
is turned on per server, and most have a free tier with additional controls on a
paid plan.

This page is a public overview: what each module protects against, and roughly
which plan it needs. It does not describe how detection works.

Plan availability changes as AntiLink evolves. The
[pricing page](https://antil.ink/premium) is the authoritative comparison, and
[docs.antil.ink](https://docs.antil.ink) has the configuration instructions for
every module below.

## Link and content protection

**Link protection**
Phishing, malicious URLs, spam links, unwanted Discord invites, and external links
you do not want posted in your server. This is the core of AntiLink.
Plan: AntiLink Basic, with expanded enforcement and controls on paid plans.

**Whitelists**
Exemptions for the people, places, and domains you trust: users, domains, roles,
channels, and categories.
Plan: AntiLink Basic, with more entry types and larger lists on paid plans.

**Scam Guard**
Scam and phishing message patterns that accompany links, including impersonation
and reward or giveaway bait. Opt in.
Plan: AntiLink Basic, with additional controls on paid plans.

**Link reputation checks**
`/checklink` returns a reputation assessment for a URL or domain on demand.
AntiLink never describes a link as guaranteed safe. A clean result means that no
known threat was found at the time of the check.
Plan: AntiLink Basic.

## Join and raid defense

**Member Defense**
Suspicious joins and coordinated raids, with screening at the moment members
arrive and restrictions on brand new accounts.
Plan: AntiLink Premium.

**Honeypot**
Trap channels that a genuine member has no reason to post in. Anyone who does is
treated as suspicious.
Plan: AntiLink Basic, with additional controls on paid plans.

**Emergency Lockdown**
One command that tightens link and invite enforcement across the whole server
while an incident is in progress. It only tightens; it never loosens anything you
already have on.
Plan: AntiLink Basic, with additional controls on paid plans.

**Verify**
Drive-by spam accounts and raid bots that join and immediately post. New members
confirm themselves before gaining access, with an optional captcha step and an
optional minimum account age.
Plan: AntiLink Basic, with additional verification options on paid plans.

## Insider threat and recovery

**Anti-Nuke**
A compromised or rogue administrator: mass channel and role deletion, mass bans
and kicks, and untrusted bots being added. Trusted people can be exempted, and
configuration is restricted to the server owner rather than any administrator.
Plan: AntiLink Premium.

**Server Backup and Restore**
Recovery after damage. Snapshots the parts of the server you select and restores
what is missing, including into a different server you also manage. A restore only
adds back what is gone; it does not delete or overwrite what is already there.
Plan: AntiLink Premium.

## Message moderation

**Custom Automod**
General message abuse beyond links: spam, banned words, duplicated text, repeated
messages, caps, emoji spam, and mass mentions. Each filter is separate and
configured on the dashboard. There is no slash command for it.
Plan: AntiLink Basic, with additional filters and responses on paid plans.

**Native Discord AutoMod**
AntiLink also creates real Discord AutoMod rules on your behalf, adding a
server-side layer alongside AntiLink's own filters.
Plan: AntiLink Basic.

## Visibility

**User Logs**
A record of what happens in your server across every major server event type, sent
to the channels you choose. Passive logging only; it never moderates.
Plan: AntiLink Basic.

**Analytics**
Per-server security analytics: what was blocked, when, and by which module, with
CSV export.
Plan: AntiLink Basic.

**Community Health**
Community activity trends rather than threats: message and voice activity, member
counts, quiet channels, and a weekly summary report. Aggregate counts only.
AntiLink never stores message content for this. Opt in.
Plan: AntiLink Plus.

**Moderation logs, appeals, and audit history**
What AntiLink acted on, who changed the configuration, and a queue for members
appealing an action.
Plan: AntiLink Basic.

## Configuration

Modules are configured with slash commands in Discord or on the
[dashboard](https://dashboard.antil.ink). Configuration stays in sync between the
two, so a change made in one place appears in the other.

Full setup instructions for every module are in the
[official documentation](https://docs.antil.ink). The command reference is at
[antil.ink/commands](https://antil.ink/commands).
