# Hey, I'm Som Samantray

[![X](https://img.shields.io/badge/X-@raazor5050-black?style=flat&logo=x)](https://x.com/raazor5050)
[![LinkedIn](https://img.shields.io/badge/LinkedIn-som--samantray-blue?style=flat&logo=linkedin)](https://linkedin.com/in/som-samantray)
[![Email](https://img.shields.io/badge/Email-som.samantray@gmail.com-red?style=flat&logo=gmail)](mailto:som.samantray@gmail.com)

Tinkering with AI and building skills and CLIs!

## Building:

- [dwnld-any](https://github.com/SomSamantray/dwnld-any) ![stars](https://img.shields.io/github/stars/SomSamantray/dwnld-any?style=flat&label=stars&color=yellow) - Agent skill + local CLI for downloading videos from 8 platforms (YouTube, Instagram, X, Reddit, and more) via yt-dlp, no cloud deploy.
- [tidbits](https://github.com/SomSamantray/tidbits) ![stars](https://img.shields.io/github/stars/SomSamantray/tidbits?style=flat&label=stars&color=yellow) - Bite-sized trivia website built with Next.js 16 and Turso/libSQL.
- [airesearch](https://github.com/SomSamantray/airesearch) ![stars](https://img.shields.io/github/stars/SomSamantray/airesearch?style=flat&label=stars&color=yellow) - Claude Code/Codex research skill that runs a deterministic engine (not the LLM) to pull evidence-led findings across X, Reddit, arXiv, GitHub, HN, and YouTube.
- [Claude-Dashboard](https://github.com/SomSamantray/Claude-Dashboard) ![stars](https://img.shields.io/github/stars/SomSamantray/Claude-Dashboard?style=flat&label=stars&color=yellow) - Local analytics dashboard for Claude Code usage — tokens, costs, sessions, heatmaps.
- [Claude-Code-Token-Limit](https://github.com/SomSamantray/Claude-Code-Token-Limit) ![stars](https://img.shields.io/github/stars/SomSamantray/Claude-Code-Token-Limit?style=flat&label=stars&color=yellow) - Claude Code plugin that shows context window %, turns remaining, and daily/weekly token budgets after every response.

## Opensource Contributions:

- [Printing Press Library - Parallel.ai CLI](https://github.com/mvanhorn/printing-press-library/tree/main/cli-skills) ![stars](https://img.shields.io/github/stars/mvanhorn/printing-press-library?style=flat&label=stars&color=yellow) - Added agent-native Parallel web research with a local SQLite memory
- [Last30Days Skill](https://github.com/mvanhorn/last30days-skill) ![stars](https://img.shields.io/github/stars/mvanhorn/last30days-skill?style=flat&label=stars&color=yellow) - Fixed [#911](https://github.com/mvanhorn/last30days-skill/pull/911): Windows setup silently failed to auto-install `npx` because the resolved path wasn't passed to the install command
- [Last30Days Skill](https://github.com/mvanhorn/last30days-skill) ![stars](https://img.shields.io/github/stars/mvanhorn/last30days-skill?style=flat&label=stars&color=yellow) - Fixed [#912](https://github.com/mvanhorn/last30days-skill/pull/912): four bugs — `--web-backend=keyless` flag was rejected by the CLI, arXiv searches returned nothing for normal phrases, source links showed as plain text instead of clickable links, and Truth Social requests were blocked by Cloudflare
- [Compound Engineering Plugin](https://github.com/EveryInc/compound-engineering-plugin) ![stars](https://img.shields.io/github/stars/EveryInc/compound-engineering-plugin?style=flat&label=stars&color=yellow) - Fixed [#1292](https://github.com/EveryInc/compound-engineering-plugin/pull/1292): on Windows, background AI workers could quietly launch on the wrong bash (WSL instead of Git Bash) and skip work without any error
- [Compound Engineering Plugin](https://github.com/EveryInc/compound-engineering-plugin) ![stars](https://img.shields.io/github/stars/EveryInc/compound-engineering-plugin?style=flat&label=stars&color=yellow) - Fixed [#1291](https://github.com/EveryInc/compound-engineering-plugin/pull/1291): renamed a confusing internal flag (`mode:headless` → `mode:non-interactive`) across skills, keeping the old name working temporarily so nothing breaks
- [CLI Printing Press](https://github.com/mvanhorn/cli-printing-press) ![stars](https://img.shields.io/github/stars/mvanhorn/cli-printing-press?style=flat&label=stars&color=yellow) - Fixed [#3855](https://github.com/mvanhorn/cli-printing-press/pull/3855): Windows credential tests failed because sandbox test folders had overly loose permissions, now locked to owner-only
- [CLI Printing Press](https://github.com/mvanhorn/cli-printing-press) ![stars](https://img.shields.io/github/stars/mvanhorn/cli-printing-press?style=flat&label=stars&color=yellow) - Fixed [#3856](https://github.com/mvanhorn/cli-printing-press/pull/3856): a Windows test failure showed the wrong folder path, making the real problem hard to track down
- [CLI Printing Press](https://github.com/mvanhorn/cli-printing-press) ![stars](https://img.shields.io/github/stars/mvanhorn/cli-printing-press?style=flat&label=stars&color=yellow) - Fixed [#3857](https://github.com/mvanhorn/cli-printing-press/pull/3857): generated export/sync tools could report "success" even when saving the file actually failed
