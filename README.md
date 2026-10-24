# Cold Email Hall of Fame

A Claude skill and open database of **43 documented cold emails** (plus a few famous cold calls and letters) that got replies from people who weren't supposed to answer: Bill Gates, Mark Cuban, Marc Benioff, Elon Musk, Sundar Pichai, Jason Lemkin and more.

**Browse the archive:** https://elo252.github.io/cold-email-hall-of-fame/

Each entry records who sent it, what made it work, the ask, how fast the reply came, what happened next, the tactics used, an evidence level and source links. Emails are paraphrased from public sources, not reproduced.

## The skill

`cold-email-hall-of-fame/` is a Claude skill that turns the archive into a working playbook. It:

- asks five intake questions (who, what, why them, your proof, what they get)
- researches the recipient when web search is available
- drafts the email with three subject-line options, a follow-up and the closest real case
- critiques any draft against a 10-point checklist
- refuses to fabricate credentials or help with harassing follow-ups

### Install

- **Claude apps:** download [`cold-email-hall-of-fame-skill.zip`](https://github.com/elo252/cold-email-hall-of-fame/raw/main/dist/cold-email-hall-of-fame-skill.zip), then Settings → Capabilities → Skills → upload.
- **Claude Code:** `git clone https://github.com/elo252/cold-email-hall-of-fame && cp -r cold-email-hall-of-fame/cold-email-hall-of-fame ~/.claude/skills/`

### Try it

- "Help me cold email Jason Lemkin about my SaaS startup. We're at $40K MRR."
- "Critique this cold email to a hiring manager at Stripe: ..."
- "I got rejected from an accelerator. Should I reply, and what do I say?"

## Repo layout

| Path | What it is |
|---|---|
| `cold-email-hall-of-fame/SKILL.md` | The skill: workflow, playbooks by goal, checklist, 43-entry casebook |
| `cold-email-hall-of-fame/references/` | Full database bundled with the skill |
| `data/emails.json` | Database with tactic glossary and evidence definitions |
| `data/emails.csv` | Same data for spreadsheets |
| `docs/index.html` | The searchable archive page (served by GitHub Pages) |
| `dist/cold-email-hall-of-fame-skill.zip` | Ready-to-upload skill package |

## What the winners have in common

1. One ask, small and specific. Never "pick your brain."
2. Credibility in the first line.
3. Short enough to read on a phone.
4. Research that proves it isn't spam.
5. Arrive when they're primed: a new fund, a new company, a public request.
6. Give before you take: a demo, an essay, free strategy.
7. Follow up with something new each time.

## About the data

Evidence labels: **primary** (told by the sender or recipient), **multi-source** (two or more outlets), **single-source**, **self-reported** (the sender's own claim) and **gated** (featured in a newsletter that requires signup; linked, not summarized). Treat single-source and self-reported numbers as directional. Compiled October 2026.

Inspired by Siddharth Haldar's [Cold Email Hall of Fame newsletter](https://cold-email-hall-of-fame.beehiiv.com/). Corrections and new entries welcome: open an issue or a pull request with a public source link.

## License

MIT. The summaries are original; linked sources belong to their authors.
