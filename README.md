# Hey, I'm Som Samantray

[![X](https://img.shields.io/badge/X-@raazor5050-black?style=flat&logo=x)](https://x.com/raazor5050)
[![LinkedIn](https://img.shields.io/badge/LinkedIn-som--samantray-blue?style=flat&logo=linkedin)](https://linkedin.com/in/som-samantray)
[![Email](https://img.shields.io/badge/Email-som.samantray@gmail.com-red?style=flat&logo=gmail)](mailto:som.samantray@gmail.com)

Tinkering with AI and building skills

## Building:

- [dwnld-any](https://github.com/SomSamantray/dwnld-any) ![stars](https://img.shields.io/github/stars/SomSamantray/dwnld-any?style=flat&label=stars&color=yellow) - Agent skill + local CLI for downloading videos from 8 platforms (YouTube, Instagram, X, Reddit, and more) via yt-dlp, no cloud deploy.
- [tidbits](https://github.com/SomSamantray/tidbits) ![stars](https://img.shields.io/github/stars/SomSamantray/tidbits?style=flat&label=stars&color=yellow) - Bite-sized trivia website built with Next.js 16 and Turso/libSQL.
- [airesearch](https://github.com/SomSamantray/airesearch) ![stars](https://img.shields.io/github/stars/SomSamantray/airesearch?style=flat&label=stars&color=yellow) - Claude Code/Codex research skill that runs a deterministic engine (not the LLM) to pull evidence-led findings across X, Reddit, arXiv, GitHub, HN, and YouTube.
- [Claude-Dashboard](https://github.com/SomSamantray/Claude-Dashboard) ![stars](https://img.shields.io/github/stars/SomSamantray/Claude-Dashboard?style=flat&label=stars&color=yellow) - Local analytics dashboard for Claude Code usage — tokens, costs, sessions, heatmaps.
- [Claude-Code-Token-Limit](https://github.com/SomSamantray/Claude-Code-Token-Limit) ![stars](https://img.shields.io/github/stars/SomSamantray/Claude-Code-Token-Limit?style=flat&label=stars&color=yellow) - Claude Code plugin that shows context window %, turns remaining, and daily/weekly token budgets after every response.

## Opensource Contributions:

### [Printing Press Library](https://github.com/mvanhorn/printing-press-library) ![stars](https://img.shields.io/github/stars/mvanhorn/printing-press-library?style=flat&label=stars&color=yellow)
- [Screener CLI](https://github.com/mvanhorn/printing-press-library/pull/1715) - Indian stock market fundamental analysis, screening, and market pulse, with company compare, quarterly trend detection, screen overlap/ranking, and insider buy/sell flow tracking
- [Pinecone CLI](https://github.com/mvanhorn/printing-press-library/pull/1710) - Every Pinecone API feature, plus local sync, snapshot history, and text-first search no other Pinecone tool has
- [Browserbase CLI](https://github.com/mvanhorn/printing-press-library/pull/1711) - Every Browserbase cloud feature, plus session lifecycle control, local history, and usage analytics no other tool has
- [Algolia CLI](https://github.com/mvanhorn/printing-press-library/pull/1712) - Manages indices, records, search, rules, synonyms, API keys, and settings from the terminal, with a local SQLite mirror, cross-index search, settings diffing, and relevance regression checks the official CLI can't offer
- [Sarvam AI CLI](https://github.com/mvanhorn/printing-press-library/pull/1718) - Wraps chat, speech-to-text/text-to-speech, translation, transliteration, and document intelligence across 22+ Indian languages, with local history, offline search, and 8 novel commands
- [Exa CLI](https://github.com/mvanhorn/printing-press-library/pull/1682) - Search API (web search, content retrieval, cited answers, similarity) across 58 endpoints, with spend tracking, monitor diffing, and entity timeline reports
- [Weaviate CLI](https://github.com/mvanhorn/printing-press-library/tree/main/cli-skills) - Vector database CLI with Get/Store/Shard/Search and other operations
- [Parallel.ai CLI](https://github.com/mvanhorn/printing-press-library/tree/main/cli-skills) - Web research with a local SQLite memory
- [v0 CLI](https://github.com/mvanhorn/printing-press-library/pull/1657) - Generate/stream app builds, sync history offline, and track AI credit spend across models
- [NotebookLM CLI](https://github.com/mvanhorn/printing-press-library/pull/1562) - Manage notebooks, chat with sources, generate Studio artifacts, and search offline

### [CLI Printing Press](https://github.com/mvanhorn/cli-printing-press) ![stars](https://img.shields.io/github/stars/mvanhorn/cli-printing-press?style=flat&label=stars&color=yellow)
- [#4049](https://github.com/mvanhorn/cli-printing-press/pull/4049) - A passing local check still let an unrewritten module path slip into a packaged CLI; added a module-path check and surfaced the review-gate rules agents were missing
- [#3855](https://github.com/mvanhorn/cli-printing-press/pull/3855) - Windows credential tests failed because sandbox test folders had overly loose permissions, now locked to owner-only
- [#3856](https://github.com/mvanhorn/cli-printing-press/pull/3856) - A Windows test failure showed the wrong folder path, making the real problem hard to track down
- [#3857](https://github.com/mvanhorn/cli-printing-press/pull/3857) - Generated export/sync tools could report "success" even when saving the file actually failed

### [Last30Days Skill](https://github.com/mvanhorn/last30days-skill) ![stars](https://img.shields.io/github/stars/mvanhorn/last30days-skill?style=flat&label=stars&color=yellow)
- [#911](https://github.com/mvanhorn/last30days-skill/pull/911) - Windows setup silently failed to auto-install `npx` because the resolved path wasn't passed to the install command
- [#912](https://github.com/mvanhorn/last30days-skill/pull/912) - Four bugs: `--web-backend=keyless` flag was rejected by the CLI, arXiv searches returned nothing for normal phrases, source links showed as plain text instead of clickable links, and Truth Social requests were blocked by Cloudflare
- [#955](https://github.com/mvanhorn/last30days-skill/pull/955) - GitHub searches for a topic could silently return zero results because the tool's own date filter clashed with search filters already baked into the query

### [Compound Engineering Plugin](https://github.com/EveryInc/compound-engineering-plugin) ![stars](https://img.shields.io/github/stars/EveryInc/compound-engineering-plugin?style=flat&label=stars&color=yellow)
- [#1292](https://github.com/EveryInc/compound-engineering-plugin/pull/1292) - On Windows, background AI workers could quietly launch on the wrong bash (WSL instead of Git Bash) and skip work without any error
- [#1291](https://github.com/EveryInc/compound-engineering-plugin/pull/1291) - Renamed a confusing internal flag (`mode:headless` → `mode:non-interactive`) across skills, keeping the old name working temporarily so nothing breaks

### [plano](https://github.com/katanemo/plano) ![stars](https://img.shields.io/github/stars/katanemo/plano?style=flat&label=stars&color=yellow)
- Fixed [#1018](https://github.com/katanemo/plano/pull/1018): fast, short streaming responses could crash the LLM gateway worker with a divide-by-zero error while recording throughput metrics, taking down other requests sharing that worker

### [openstreetmap-website](https://github.com/openstreetmap/openstreetmap-website) ![stars](https://img.shields.io/github/stars/openstreetmap/openstreetmap-website?style=flat&label=stars&color=yellow)
- Fixed [#7297](https://github.com/openstreetmap/openstreetmap-website/pull/7297): future-tense block-expiry text ("in 3 days") bypassed the app's own translation file and fell back to an English-only default

### [loopx](https://github.com/huangruiteng/loopx) ![stars](https://img.shields.io/github/stars/huangruiteng/loopx?style=flat&label=stars&color=yellow)
- Fixed [#2801](https://github.com/huangruiteng/loopx/pull/2801): repeated `/loopx` calls picked a random agent each time instead of remembering which one a conversation was already using

### [AgentMemory](https://github.com/rohitg00/agentmemory) ![stars](https://img.shields.io/github/stars/rohitg00/agentmemory?style=flat&label=stars&color=yellow)
- Fixed [#1132](https://github.com/rohitg00/agentmemory/pull/1132): deleting a memory could falsely say "deleted" when nothing was actually removed, and there was no way to delete a saved lesson at all — both now fixed

### [qm](https://github.com/yc-software/qm) ![stars](https://img.shields.io/github/stars/yc-software/qm?style=flat&label=stars&color=yellow)
- Fixed [#149](https://github.com/yc-software/qm/pull/149): a brief database hiccup while waiting for a job to finish could crash the whole process instead of just timing out safely

### [Buzz](https://github.com/block/buzz) ![stars](https://img.shields.io/github/stars/block/buzz?style=flat&label=stars&color=yellow)
- Fixed [#4500](https://github.com/block/buzz/pull/4500): docs told users to import agent packs via a "zip file + Install Pack button" that doesn't exist anymore in the app, now corrected to match the real import flow

### [planning-with-files](https://github.com/OthmanAdi/planning-with-files) ![stars](https://img.shields.io/github/stars/OthmanAdi/planning-with-files?style=flat&label=stars&color=yellow)
- Audited [#216](https://github.com/OthmanAdi/planning-with-files/pull/216): found 5 duplicate language skills had silently drifted out of sync (missing bug fixes, missing features)

### [gstack](https://github.com/garrytan/gstack) ![stars](https://img.shields.io/github/stars/garrytan/gstack?style=flat&label=stars&color=yellow)
- Fixed [#2409](https://github.com/garrytan/gstack/pull/2409): setup docs told agents to run two memory-sync scripts as bare commands, which fail with "No such file or directory" since they're plain `.ts` files with no bin alias — corrected to the proper `bun run` invocation
- Audited and help fix [#2409](https://github.com/garrytan/gstack/pull/2409): setup docs told agents to run two memory-sync scripts as bare commands, which fail with "No such file or directory" since they're plain `.ts` files with no bin alias — corrected to the proper `bun run` invocation
