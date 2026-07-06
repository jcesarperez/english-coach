# english-coach

A [Claude Code](https://claude.com/claude-code) skill that helps you go from "people understand me in Enlgish" to "I sound like the senior person I actually am".

It's built specifically for **Spanish speakers**: experienced engineers and engineering leaders who already work in English every day, and want to close the gap in phrasing, confidence, and register — not grammar. It knows the specific habits Spanish speakers carry into English (over-hedging, over-apologizing, literal translations) and corrects for those directly, instead of giving you generic language-learning advice.

## Two ways to use it

**🎓 "Teach me something"** → a short, 5-minute lesson on language you'll actually use this week — pushing back without sounding junior, softening bad news without sounding weak. Pronunciation included.

> Topic: **leverage**. There's no clean Spanish equivalent, so it gets skipped or replaced with something clunky — but it's one of the highest-signal words in tech leadership. The lesson covers what it actually means, how natives use it in planning and negotiation, and a pattern you can reuse right away.

**🔍 Paste a Slack message / RFC / comment** → get it rewritten the way a senior native speaker would say it, plus the *why*.

> **You:** "I am agree with the plan, we only need to make a meeting with the client"
> **Coach:** two calques from Spanish in one sentence. Try: *"I agree with the plan — we just need to set up a meeting with the client."* "I am agree" copies *estoy de acuerdo*; English uses "agree" as a verb, not "be + agree." And "make a meeting" should be "set up" or "schedule."

## Install in 1 minute

**Option A — plugin (recommended):**

```
/plugin marketplace add jcesarperez/english-coach
/plugin install english-coach@jcesarperez-plugins
```

Then use it with `/english-coach:english-coach`, or just talk naturally — say *"teach me something"* or paste a Slack message and ask *"does this sound natural?"*.

**Option B — skill file only:**

```bash
mkdir -p ~/.claude/skills/english-coach
curl -o ~/.claude/skills/english-coach/SKILL.md \
  https://raw.githubusercontent.com/jcesarperez/english-coach/main/skills/english-coach/SKILL.md
```

(Prefer project-only scope? Copy the file into `.claude/skills/english-coach/` inside your repo instead of `~/.claude/skills/`.)

## Why this exists

You already work in English every day. Nobody struggles to understand you anymore.

But you still hesitate before sending an RFC, over-soften feedback that needed to be direct, or write sentences that are grammatically perfect but don't sound like how a senior engineer actually communicates. Nobody corrects this, because your English is already "good enough." That's exactly where most people stop improving.

This project is for what comes after. Not another English course — it doesn't teach grammar. It teaches how experienced engineers actually phrase things, so the tiny language signals stop distracting from your ideas.

## Why a Claude Code skill, not another app

Because it lives where you already write: Slack drafts, RFCs, design docs, PR comments. Instead of opening a separate tool to ask "does this sound okay?", you ask right where you're already working, mid-task.

It also means you set the pace, no pressure to keep a streak or finish a course. One or two lessons a day, a couple of Slack conversations pasted in for review, or a meeting transcript you want cleaned up — however much time you have, whenever you have it.

## License

MIT — see [LICENSE](LICENSE).
