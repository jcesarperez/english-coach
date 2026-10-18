# Changelog

All notable changes to this project are documented here.
The format follows [Keep a Changelog](https://keepachangelog.com/en/1.1.0/), and the project uses [Semantic Versioning](https://semver.org/).

## [1.1.0] - 2026-10-17

### Added
- "¿Cómo se dice…?" mode: ask how to say a Spanish phrase in English and get what a native would say, by register (Slack to formal), plus the literal translation to avoid.
- Support for any tool that implements Agent Skills (Claude Code, OpenAI Codex, Cursor, GitHub Copilot, Gemini CLI, and others), with a one-command install: `npx skills add jcesarperez/english-coach -g`.
- README: per-tool install paths and a "How to use it" section.

### Changed
- The skill no longer loads on its own (`disable-model-invocation: true`), so it costs no tokens in unrelated conversations. Start it by name, for example `/english-coach`.
- `SKILL.md` is about 20% shorter, with the same rules.

## [1.0.0] - 2026-07-06

### Added
- First release of the english-coach skill for Spanish-speaking engineers: short lessons ("teach me something") and natural-sounding review of your own writing, with pronunciation and a focus on register over grammar.
- Packaged as a Claude Code plugin, installable from the `jcesarperez-plugins` marketplace.

[1.1.0]: https://github.com/jcesarperez/english-coach/compare/v1.0.0...v1.1.0
[1.0.0]: https://github.com/jcesarperez/english-coach/releases/tag/v1.0.0
