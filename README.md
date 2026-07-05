# english-coach

A [Claude Code](https://claude.com/claude-code) skill that helps you break through the English plateau — the point where you're fluent enough to get by, but not fluent enough to sound senior.

## Install in 1 minute

```bash
mkdir -p ~/.claude/skills/english-coach
curl -o ~/.claude/skills/english-coach/SKILL.md \
  https://raw.githubusercontent.com/jcesarperez/english-coach/main/.claude/skills/english-coach/SKILL.md
```

That's it. Open Claude Code and say something like *"teach me something"* or paste a Slack message you just wrote and ask *"does this sound natural?"*.

(Prefer project-only scope? Copy the file into `.claude/skills/english-coach/` inside your repo instead of `~/.claude/skills/`.)

## The plateau nobody warns you about

You move to an international company. Your English is good — good enough to get hired, good enough to survive standups, good enough to write a Jira ticket nobody misunderstands. For a while, you keep improving just by being immersed.

And then you stop.

You're still translating in your head half the time. You over-apologize before asking a question. You say "I think maybe we could..." when a native colleague would just say "I'd suggest...". You can *understand* a Staff Engineer effortlessly, but when you write your own RFC, something about it reads like it was translated — because it was, just inside your own head. Nobody corrects you, because your English is "good enough." So you plateau there, sounding capable but not quite senior, for years.

That plateau is the whole problem this skill exists to solve. Not grammar — you're past grammar. The gap is **nuance, register, and the small tells that reveal a non-native writer** to anyone who's a native speaker.

## What it actually does

Two modes, both built around one idea: teach concepts you'll use *this week*, not abstract vocabulary lists.

**🎓 Short, practical lessons on real engineering-leadership topics.**
You ask for a lesson — or just say "teach me something" and it picks a high-value topic for you — and get a focused, ~5-minute lesson on one concept that actually comes up in your job: how to push back on a decision without sounding junior, what "let's not boil the ocean" really signals, the difference between "I think we should" and "I'd push back on this," how natives soften bad news without sounding weak. Every lesson includes pronunciation guidance with links so you can hear the word or phrase used in context, not just read it.

Example:
> **You:** teach me something
> **Coach:** Topic of the day: **blast radius**. Engineers use it constantly outside of actual incidents — "what's the blast radius of this change?" — and it signals you're thinking about consequences before someone asks you to...
> *(continues into how natives use it, what Spanish speakers say instead, a mini pattern, pronunciation, and a short exercise)*

**🔍 Corrections based on what you actually wrote.**
This is the part that makes it compound. You paste a real Slack message, a paragraph from an RFC, a comment you left on a design doc — and the coach rewrites it the way a native EM at your level would, then explains *why*: what you over-hedged, which phrase was a literal calque from Spanish, where you buried the ask instead of leading with it. It's not "here's the correct grammar." It's "here's what a director reads when they see this, and here's the version that reads as senior."

Example:
> **You:** "I think maybe we should consider to migrate the service, sorry if this is a bad moment to ask"
> **Coach:** **How it lands right now:** the apology and the hedging bury the ask — a director has to dig to find out what you actually want.
> **Native/senior rewrite:** "I'd like to propose migrating the service — here's why, and here's the trade-off if we wait."
> **Why:** dropped the pre-emptive apology, swapped "I think maybe... consider to" for a direct stance verb, led with the ask instead of the disclaimer.

Every review also closes with one mini-lesson on the *recurring* pattern behind the mistake — so the correction generalizes instead of just fixing that one sentence.

## Who this is for

Built for a senior software engineering leader (roughly B2/C1) working daily in English at an international company — but the mode detection and lesson format work for any technical professional past the beginner stage who wants to close the gap between "understood" and "sounds like one of us."

## License

MIT — see [LICENSE](LICENSE).
