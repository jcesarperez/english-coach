# english-coach

An AI agent skill that helps you go from "people understand me in English" to "I sound like the senior person I actually am".

It's built specifically for **Spanish speakers**: experienced engineers and engineering leaders who already work in English every day, and want to close the gap in phrasing, confidence, and register — not grammar. It knows the specific habits Spanish speakers carry into English (over-hedging, over-apologizing, literal translations) and corrects for those directly, instead of giving you generic language-learning advice.

## Three ways to use it

**🎓 "Teach me something"** → a short, 5-minute lesson on language you'll actually use this week — pushing back without sounding junior, softening bad news without sounding weak. Pronunciation included.

> Topic: **leverage**. There's no clean Spanish equivalent, so it gets skipped or replaced with something clunky — but it's one of the highest-signal words in tech leadership. The lesson covers what it actually means, how natives use it in planning and negotiation, pronunciation examples, and a pattern you can reuse right away.

**🔍 Paste a Slack message / RFC / meeting transcript** → get it rewritten the way a senior native speaker would say it, plus the *why* and pronunciation tips.

> **You:** "I am agree with the plan, we only need to make a meeting with the client"
> **Coach:** two calques from Spanish in one sentence. Try: *"I agree with the plan — we just need to set up a meeting with the client."* "I am agree" copies *estoy de acuerdo*; English uses "agree" as a verb, not "be + agree." And "make a meeting" should be "set up" or "schedule."

**💬 "¿Cómo se dice…?"** → ask how to say a Spanish phrase in English and get what a native would actually say, from Slack to formal, plus the literal translation to avoid.

> **You:** "How do I say *ponerse las pilas*?"
> **Coach:** it means "pick up the pace / get serious". Slack: *"We need to step it up this sprint."* Meeting: *"We need to raise our game here."* Avoid *"put the batteries on"* — nobody says it, and it sounds like a joke.

## Install in 1 minute

It's a standard [`SKILL.md`](skills/english-coach/SKILL.md) skill, so it works in any AI tool that supports Agent Skills: Claude Code, OpenAI Codex, Cursor, GitHub Copilot, Gemini CLI, and others.

**Any tool — one command:**

```bash
npx skills add jcesarperez/english-coach -g
```

It asks which tools you use and installs the skill in the right folder for each one. `-g` makes it available in all your projects; leave it out to install it only in the current project.

**Claude Code — as a plugin:**

```
/plugin marketplace add jcesarperez/english-coach
/plugin install english-coach@jcesarperez-plugins
```

**Manual install:** copy the `skills/english-coach/` folder into your tool's skills directory:

| Tool | Personal (all projects) | Project only |
|---|---|---|
| Claude Code | `~/.claude/skills/` | `.claude/skills/` |
| OpenAI Codex | `~/.agents/skills/` | `.agents/skills/` |
| Cursor | `~/.cursor/skills/` | `.cursor/skills/` |
| GitHub Copilot | `~/.copilot/skills/` | `.github/skills/` |
| Gemini CLI | `~/.gemini/skills/` | `.gemini/skills/` |

For example, for Claude Code:

```bash
mkdir -p ~/.claude/skills/english-coach
curl -o ~/.claude/skills/english-coach/SKILL.md \
  https://raw.githubusercontent.com/jcesarperez/english-coach/main/skills/english-coach/SKILL.md
```

Folder names change between tool versions. If the skill doesn't load, check your tool's docs on skills.

## How to use it

Start the skill by name, then talk naturally: say *"teach me something"*, paste a Slack message and ask *"does this sound natural?"*, or ask *"¿cómo se dice 'quedamos en eso'?"*.

- Claude Code: `/english-coach` (or `/english-coach:english-coach` if you installed the plugin)
- Other tools: use their skill command, or mention the skill by name

**Why you have to start it yourself:** the skill sets `disable-model-invocation: true`, so the AI never loads it on its own. That means it costs no tokens in your other conversations. The trade-off is that it won't start automatically when you ask "does this sound natural?" without starting it first. If you prefer that, delete the line from `SKILL.md`. Tools that don't support this setting ignore it and may start the skill automatically.

## Why this exists

You already work in English every day. Nobody struggles to understand you anymore.

But you still hesitate before sending an RFC, over-soften feedback that needed to be direct, or write sentences that are grammatically perfect but don't sound like how a senior engineer actually communicates. Nobody corrects this, because your English is already "good enough." That's exactly where most people stop improving.

This project is for what comes after. Not another English course — it doesn't teach grammar. It teaches how experienced engineers actually phrase things, so the tiny language signals stop distracting from your ideas.

## Why a skill, not another app

Because it lives in the AI assistant you already use, next to where you write: Slack drafts, RFCs, design docs, PR comments. Instead of opening a separate tool to ask "does this sound okay?", you ask right where you're already working, mid-task.

It also means you set the pace, no pressure to keep a streak or finish a course. One or two lessons a day, a couple of Slack conversations pasted in for review, or a meeting transcript you want cleaned up — however much time you have, whenever you have it.

## License

MIT — see [LICENSE](LICENSE).
