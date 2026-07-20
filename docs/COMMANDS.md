# Command overview

The public AntiLink command set includes:

- `/setup`
- `/config`
- `/notify`
- `/whitelist`
- `/language`
- `/premium`
- `/redeem`
- `/antilink`
- `/checklink`
- `/lockdown`
- `/scamguard`
- `/guard`
- `/verify`
- `/antinuke`
- `/backup`
- `/ai`
- `/chat`

Commands have different Discord permission and AntiLink plan requirements.
Several security modules are opt-in and are set up by a server administrator.

Use the live [command reference](https://antil.ink/commands) for current
subcommands, options, permissions, plan requirements, and examples.

## Not every feature has a command

Some parts of AntiLink are configured on the
[dashboard](https://dashboard.antil.ink) rather than in Discord. Custom Automod
is one of them: its preset filters, including spam, bad words, duplicated text,
repeated messages, caps, emoji spam, and mass mentions, are set up on the
dashboard and have no slash command. User Logs, Analytics, and Community Health
are also dashboard features.

## Notes on individual commands

`/checklink` performs a link reputation check. A clean result means no known
threat was found at the time of the check. AntiLink never describes a link as
guaranteed safe.

`/language` sets the language AntiLink replies in for your server, and offers
24 choices. The same setting is available on the dashboard. The AntiLink
websites choose a language per visitor, separately from the server setting.

`/ai` and `/chat` are not gated on a server plan. AI Chat runs on an AI
Membership, which is owned by a user, is token-metered, and is linked to one
server at a time. Current tiers, token allowances, and prices are listed on the
[AntiLink AI page](https://antil.ink/ai).

The AI proposes changes; a human with the matching Discord permission approves
them. It never applies anything on its own.

For detailed and current behavior, use the
[official documentation](https://docs.antil.ink).
