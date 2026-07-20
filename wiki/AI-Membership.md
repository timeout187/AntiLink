# AI Membership

The AI Membership is how AntiLink's natural-language security assistant is
provided. It is separate from the AntiLink server plans.

A server plan (Basic, Plus, Premium) belongs to a server. An AI Membership
belongs to a **person**, is **token-metered**, and is **linked to one server at
a time**. A server does not need a paid plan to use the assistant, and a paid
plan does not include the assistant.

## Tiers

| Tier | Tokens per month | Monthly | Yearly |
| --- | --- | --- | --- |
| Silver | 2,500,000 | $5 | $50 |
| Gold | 5,000,000 | $10 | $100 |
| Platinum | 15,000,000 | $30 | $300 |

Yearly billing is ten times the monthly price, so a yearly membership is two
months free.

Prices and allowances can change. The [AntiLink AI page](https://antil.ink/ai) is
the current source for what a membership costs and includes. Memberships are
bought and managed on the [dashboard](https://dashboard.antil.ink).

## How the token pool works

- Every membership carries a monthly token allowance.
- Conversations with the assistant draw from that allowance.
- The pool **resets on the 1st of each month**.
- Current usage for the linked server is shown on the dashboard and through the
  `/ai` and `/chat` commands.

## Ownership and linking

- A membership is held by a Discord user, not by a server.
- A membership is linked to **one server at a time**, and the link can be
  changed later.
- One person may hold more than one membership, for example one per community
  they run.

Purchase, linking, and relinking are all done from the
[dashboard](https://dashboard.antil.ink). Payments run through Paddle as
merchant of record.

## Chat history retention

The assistant keeps recent conversation context so a discussion can continue
across messages. How long that history is retained depends on the tier.

| Tier | Chat history retained |
| --- | --- |
| Silver | 3 days |
| Gold | 7 days |
| Platinum | 30 days |

## General chat is Platinum only

On Silver and Gold, the assistant stays focused on AntiLink and server security.
**General, non-security conversation is available on Platinum only.**

## What the assistant can do

- Answer questions about your AntiLink configuration, protection posture, and
  recent security activity in the linked server.
- Explain security recommendations and why a setting matters.
- Look up live security information on request. These lookups are read-only and
  change nothing in your server.
- Read an attached **screenshot** of your settings. It extracts text from the
  image so it can answer questions about what it shows.
- Follow **server guidance** you give it ("teach the bot"), which shapes how it
  answers.
- Post an opt-in **Weekly AI Security Digest**: a weekly recap of your server's
  protection, sent to a channel you choose.

AntiLink never describes a link as guaranteed safe. A clean result means that no
known threat was found at the time of the check.

## The approval model

**The AI proposes. A human approves. The AI never applies anything by itself.**

When the assistant decides an action would help, it does not perform it. It
presents the proposed action with an approval control. Nothing happens until a
person clicks approve, and the approval is checked against that person's own
Discord permissions.

### What it can propose

- Protection toggles and other configuration changes, including pointing a
  setting at a specific channel, role, mode, or number
- Whitelist additions and removals
- Moderation actions: timeout, kick, ban, or clearing messages
- Creating a role or a channel, including setting up log channels

Each proposal can only be approved by someone who already holds the Discord
permission for that action.

Configuration proposals are limited to a fixed set of settable fields. The
assistant cannot invent a new setting to change.

### Created roles

When a role is created through an approved proposal, it receives only
permissions the **approving admin already holds**. Administrator is never
grantable through the AI.

## Commands

| Command | Who uses it |
| --- | --- |
| `/ai` | Server admins: set up the AI channel, review status and usage |
| `/chat` | Anyone: reset their own conversation, view privacy and usage, send feedback |

Once an admin has set up an AI channel, members talk to the assistant by simply
writing in that channel. No command is needed for normal conversation.

The full, current command list is on
[antil.ink/commands](https://antil.ink/commands).

## Where to go next

- [Open the dashboard](https://dashboard.antil.ink) to buy, link, or manage a
  membership
- [Read the documentation](https://docs.antil.ink) for setup guidance
- [Join support](https://support.antil.ink) with questions about a membership
