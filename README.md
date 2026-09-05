# Hey, I'm Som Samantray

[![X](https://img.shields.io/badge/X-@raazor5050-black?style=flat&logo=x)](https://x.com/raazor5050)
[![LinkedIn](https://img.shields.io/badge/LinkedIn-som--samantray-blue?style=flat&logo=linkedin)](https://linkedin.com/in/som-samantray)
[![Email](https://img.shields.io/badge/Email-som.samantray@gmail.com-red?style=flat&logo=gmail)](mailto:som.samantray@gmail.com)

Tinkering with AI and building skills

## Building:

- [mac-storage-doctor](https://github.com/SomSamantray/mac-storage-doctor) ![stars](https://img.shields.io/github/stars/SomSamantray/mac-storage-doctor?style=flat&label=stars&color=yellow) - A Claude skill that audits a Mac's disk usage — orphaned app data, dev-tool caches, git repo bloat, rarely-used apps — and reports exactly what's safe to delete, with nothing ever removed without explicit per-item confirmation
- [dwnld-any](https://github.com/SomSamantray/dwnld-any) ![stars](https://img.shields.io/github/stars/SomSamantray/dwnld-any?style=flat&label=stars&color=yellow) - Agent skill + local CLI for downloading videos from 8 platforms (YouTube, Instagram, X, Reddit, and more) via yt-dlp, no cloud deploy.
- [tidbits](https://github.com/SomSamantray/tidbits) ![stars](https://img.shields.io/github/stars/SomSamantray/tidbits?style=flat&label=stars&color=yellow) - Bite-sized trivia website built with Next.js 16 and Turso/libSQL.
- [airesearch](https://github.com/SomSamantray/airesearch) ![stars](https://img.shields.io/github/stars/SomSamantray/airesearch?style=flat&label=stars&color=yellow) - Claude Code/Codex research skill that runs a deterministic engine (not the LLM) to pull evidence-led findings across X, Reddit, arXiv, GitHub, HN, and YouTube.
- [Claude-Dashboard](https://github.com/SomSamantray/Claude-Dashboard) ![stars](https://img.shields.io/github/stars/SomSamantray/Claude-Dashboard?style=flat&label=stars&color=yellow) - Local analytics dashboard for Claude Code usage — tokens, costs, sessions, heatmaps.
- [Claude-Code-Token-Limit](https://github.com/SomSamantray/Claude-Code-Token-Limit) ![stars](https://img.shields.io/github/stars/SomSamantray/Claude-Code-Token-Limit?style=flat&label=stars&color=yellow) - Claude Code plugin that shows context window %, turns remaining, and daily/weekly token budgets after every response.


## Opensource Contributions:

### [Printing Press Library](https://github.com/mvanhorn/printing-press-library) ![stars](https://img.shields.io/github/stars/mvanhorn/printing-press-library?style=flat&label=stars&color=yellow)
- [Screener](https://github.com/mvanhorn/printing-press-library/pull/1715) - Indian stock market fundamental analysis, screening, and market pulse, with company compare, quarterly trend detection, screen overlap/ranking, and insider buy/sell flow tracking
- [Pinecone](https://github.com/mvanhorn/printing-press-library/pull/1710) - Every Pinecone API feature, plus local sync, snapshot history, and text-first search no other Pinecone tool has
- [Browserbase](https://github.com/mvanhorn/printing-press-library/pull/1711) - Every Browserbase cloud feature, plus session lifecycle control, local history, and usage analytics no other tool has
- [Algolia](https://github.com/mvanhorn/printing-press-library/pull/1712) - Manages indices, records, search, rules, synonyms, API keys, and settings from the terminal, with a local SQLite mirror, cross-index search, settings diffing, and relevance regression checks the official CLI can't offer
- [Sarvam](https://github.com/mvanhorn/printing-press-library/pull/1718) - Wraps chat, speech-to-text/text-to-speech, translation, transliteration, and document intelligence across 22+ Indian languages, with local history, offline search, and 8 novel commands
- [Exa](https://github.com/mvanhorn/printing-press-library/pull/1682) - Search API (web search, content retrieval, cited answers, similarity) across 58 endpoints, with spend tracking, monitor diffing, and entity timeline reports
- [Weaviate](https://github.com/mvanhorn/printing-press-library/tree/main/cli-skills) - Vector database CLI with Get/Store/Shard/Search and other operations
- [Parallel](https://github.com/mvanhorn/printing-press-library/tree/main/cli-skills) - Web research with a local SQLite memory
- [v0](https://github.com/mvanhorn/printing-press-library/pull/1657) - Generate/stream app builds, sync history offline, and track AI credit spend across models
- [NotebookLM](https://github.com/mvanhorn/printing-press-library/pull/1562) - Manage notebooks, chat with sources, generate Studio artifacts, and search offline
- [iHatePDF](https://github.com/mvanhorn/printing-press-library/pull/1785) - Local-first PDF CLI: privacy scanning, hashing/fingerprinting, merge/split/rotate/encrypt, text extraction, and a local SQLite catalog for offline search — no uploads, unlike the source website
- [is-agentic](https://github.com/mvanhorn/printing-press-library/pull/1810) - Turns Is Agentic readiness reports into durable, scriptable evidence, with local audit history, score/finding diffing, CI-gating policy checks, portfolio-wide scoring across a fleet of sites, issue lifecycle tracking, and portable evidence packaging
- [QuickCommerce](https://github.com/mvanhorn/printing-press-library/pull/1835) - Compares live Indian product prices, stock, and delivery ETAs across platforms, with a local SQLite mirror for price-history tracking, field-level diffing, fastest-delivery ranking, and per-unit price comparisons
- [Keenable](https://github.com/mvanhorn/printing-press-library/pull/1832) - Reproducible web research with citations, backed by a local evidence trail: immutable search/fetch snapshots, run replay with change detection, source-linked citation export, and offline local search over saved results
- [AgentMail](https://github.com/mvanhorn/printing-press-library/pull/1834) - AgentMail operations with local memory, safe sends, and fleet-wide insight: unresolved-conversation triage across inboxes, pre-send risk checks (recipient/attachment/schedule/duplicate/idempotency), thread handoff rollups, and fleet-wide health/delivery reconciliation
- [Flighty](https://github.com/mvanhorn/printing-press-library/pull/1847) - Live airport intelligence CLI scraped straight from Flighty's public airport map (no login/API key), adding network-wide rankings, cross-airport airline/route comparisons, and change diffs that the website itself can't show
- [RapidAPI](https://github.com/mvanhorn/printing-press-library/pull/1850) - Full CLI for the RapidAPI Hub marketplace (79k+ APIs) — search, categories, collections, account/subscription management, and offline sync/export — wrapping the hub's own GraphQL gateway with a Chrome-fingerprint transport to get past its bot gate
- [mcpmarket](https://github.com/mvanhorn/printing-press-library/pull/1843) - CLI for the 45,000+ server MCP Market catalog (no official CLI existed) — adds trending deltas, snapshot diffing, author portfolios, and time-travel leaderboards by tracking history locally, which the live site itself can't show
- [Groq](https://github.com/mvanhorn/printing-press-library/pull/1854) - Full Groq Cloud inference CLI, plus a local ledger tracking token cost and rate-limit budget, multi-model prompt comparison (latency/cost/tokens-per-sec), and batch-file validation before upload

### [CLI Printing Press](https://github.com/mvanhorn/cli-printing-press) ![stars](https://img.shields.io/github/stars/mvanhorn/cli-printing-press?style=flat&label=stars&color=yellow)
- [#4049](https://github.com/mvanhorn/cli-printing-press/pull/4049) - A passing local check still let an unrewritten module path slip into a packaged CLI; added a module-path check and surfaced the review-gate rules agents were missing
- [#3855](https://github.com/mvanhorn/cli-printing-press/pull/3855) - Windows credential tests failed because sandbox test folders had overly loose permissions, now locked to owner-only
- [#3856](https://github.com/mvanhorn/cli-printing-press/pull/3856) - A Windows test failure showed the wrong folder path, making the real problem hard to track down
- [#3857](https://github.com/mvanhorn/cli-printing-press/pull/3857) - Generated export/sync tools could report "success" even when saving the file actually failed
- [#1890](https://github.com/mvanhorn/printing-press-library/pull/1890) - Google Search Console CLI's `sitemaps-submit`/`get`/`delete` 404'd whenever a feedpath was an absolute URL, since the raw `https://` slashes split the REST path; now percent-encoded as a single path segment so it routes correctly
- [#1893](https://github.com/mvanhorn/printing-press-library/pull/1893) - Movie Goat CLI's local/offline search silently returned zero results (exit 0) because the untyped search branch never assigned results, and separately crashed on FTS5-syntax queries like `Space: 1999`; both fixed with real FTS hits and per-token query sanitization

### [Last30Days Skill](https://github.com/mvanhorn/last30days-skill) ![stars](https://img.shields.io/github/stars/mvanhorn/last30days-skill?style=flat&label=stars&color=yellow)
- [#911](https://github.com/mvanhorn/last30days-skill/pull/911) - Windows setup silently failed to auto-install `npx` because the resolved path wasn't passed to the install command
- [#912](https://github.com/mvanhorn/last30days-skill/pull/912) - Four bugs: `--web-backend=keyless` flag was rejected by the CLI, arXiv searches returned nothing for normal phrases, source links showed as plain text instead of clickable links, and Truth Social requests were blocked by Cloudflare
- [#955](https://github.com/mvanhorn/last30days-skill/pull/955) - GitHub searches for a topic could silently return zero results because the tool's own date filter clashed with search filters already baked into the query
- [#1083](https://github.com/mvanhorn/last30days-skill/pull/1083) - Reddit enrichment slots skipping high-comment threads
- Fixed [#1072](https://github.com/mvanhorn/last30days-skill/pull/1072): the X-search subprocess was handed a full copy of the environment, so every unrelated API key or secret on the machine could leak to it if that vendored client were ever compromised — now it only receives an explicit allowlist of the variables it actually needs

### [hermes-agent](https://github.com/NousResearch/hermes-agent) ![stars](https://img.shields.io/github/stars/NousResearch/hermes-agent?style=flat&label=stars&color=yellow)
- Diagnosed and fixed [#92242](https://github.com/NousResearch/hermes-agent/pull/92242): large streamed tool calls (big `write_file`/`apply_patch` payloads) got quadratically slower to assemble as more chunks arrived, credited by the maintainer in the merged salvage ([#101906](https://github.com/NousResearch/hermes-agent/pull/101906))

### [pascalorg/editor](https://github.com/pascalorg/editor) ![stars](https://img.shields.io/github/stars/pascalorg/editor?style=flat&label=stars&color=yellow)
- [#636](https://github.com/pascalorg/editor/pull/636) - `exportFloorplanPdf` wasn't exported from the package, blocking host apps from building their own floorplan-export UI outside the built-in Settings panel; also deduped a repeated export-scope check into one shared predicate with direct test coverage

### [CPython](https://github.com/python/cpython) ![stars](https://img.shields.io/github/stars/python/cpython?style=flat&label=stars&color=yellow)
- Fixed [#155862](https://github.com/python/cpython/pull/155862): `class MyFlag(Mixin, Flag)` silently threw away the mixin's own `|`/`&`/`^` operator overrides in favor of `Flag`'s defaults, because `enum.py` never checked what the mixin's operators actually resolved to before overwriting them

### [Node.js](https://github.com/nodejs/node) ![stars](https://img.shields.io/github/stars/nodejs/node?style=flat&label=stars&color=yellow)
- [#65243](https://github.com/nodejs/node/pull/65243) - Clarified the `process` signal docs: `SIGTERM`/`SIGINT` listeners run asynchronously, so an otherwise-idle process can exit before the listener actually runs — a gap that had confused users since 2019

### [Compound Engineering Plugin](https://github.com/EveryInc/compound-engineering-plugin) ![stars](https://img.shields.io/github/stars/EveryInc/compound-engineering-plugin?style=flat&label=stars&color=yellow)
- [#1292](https://github.com/EveryInc/compound-engineering-plugin/pull/1292) - On Windows, background AI workers could quietly launch on the wrong bash (WSL instead of Git Bash) and skip work without any error
- [#1291](https://github.com/EveryInc/compound-engineering-plugin/pull/1291) - Renamed a confusing internal flag (`mode:headless` → `mode:non-interactive`) across skills, keeping the old name working temporarily so nothing breaks

### [MemPalace](https://github.com/MemPalace/mempalace) ![stars](https://img.shields.io/github/stars/MemPalace/mempalace?style=flat&label=stars&color=yellow)
- [#2342](https://github.com/MemPalace/mempalace/pull/2342) - Pre-commit's Ruff hook could drift from the version pinned in `pyproject.toml` and CI, letting local checks silently pass or fail differently than CI; aligned all three sources and scoped version extraction to the Ruff hook block so unrelated hook bumps can't trip the check

### [Actual Budget](https://github.com/actualbudget/actual) ![stars](https://img.shields.io/github/stars/actualbudget/actual?style=flat&label=stars&color=yellow)
- Fixed [#8719](https://github.com/actualbudget/actual/pull/8719): merging two payees left "one of"/"not one of" rule conditions with the merged payee listed twice, so deleting the visible duplicate in the UI silently deleted both underlying entries and dropped the payee from the rule entirely

### [rtk](https://github.com/rtk-ai/rtk) ![stars](https://img.shields.io/github/stars/rtk-ai/rtk?style=flat&label=stars&color=yellow)
- Fixed [#3560](https://github.com/rtk-ai/rtk/pull/3560): three output-compaction filters (spring-boot, liquibase, ssh) had regexes so broad they silently mangled unrelated commands — e.g. any `java -jar` file got Spring-only filtering, `rm -rf /opt/liquibase` triggered liquibase compaction, and `ssh-keygen`/`ssh-add` got caught by a plain `ssh` filter

### [reticle](https://github.com/reticlehq/reticle) ![stars](https://img.shields.io/github/stars/reticlehq/reticle?style=flat&label=stars&color=yellow)
- Fixed [#746](https://github.com/reticlehq/reticle/pull/746): a missing OS shared library (e.g. `libnspr4.so`) was misreported as "Chromium is not installed," sending users to run a reinstall command that succeeded but fixed nothing

### [Needle](https://github.com/cactus-compute/needle) ![stars](https://img.shields.io/github/stars/cactus-compute/needle?style=flat&label=stars&color=yellow)
- [#98](https://github.com/cactus-compute/needle/pull/98) - Made the setup script auto-detect and prefer `uv` (10-100x faster than pip) when available, falling back to pip only when it isn't installed

### [quickjs-ng](https://github.com/quickjs-ng/quickjs) ![stars](https://img.shields.io/github/stars/quickjs-ng/quickjs?style=flat&label=stars&color=yellow)
- Fixed [#1657](https://github.com/quickjs-ng/quickjs/pull/1657): `quickjs.c` failed to compile on GCC 14+ for any ESP32 target, because six call sites passed `int*` where the platform's `int32_t*` was expected (or vice versa)

### [DeepAgents](https://github.com/langchain-ai/deepagents) ![stars](https://img.shields.io/github/stars/langchain-ai/deepagents?style=flat&label=stars&color=yellow)
- Fixed [#5747](https://github.com/langchain-ai/deepagents/pull/5747): `edit_file` with an empty search string silently corrupted files by inserting the replacement between every single character instead of erroring out

### [apify-mcp-server](https://github.com/apify/apify-mcp-server) ![stars](https://img.shields.io/github/stars/apify/apify-mcp-server?style=flat&label=stars&color=yellow)
- Fixed [#1315](https://github.com/apify/apify-mcp-server/pull/1315): running the conformance test suite locally leaked the raw `APIFY_TOKEN` to the terminal in plain text — CI masked it, but the local script had no equivalent redaction

### [caveman](https://github.com/JuliusBrussee/caveman) ![stars](https://img.shields.io/github/stars/JuliusBrussee/caveman?style=flat&label=stars&color=yellow)
- Fixed [#900](https://github.com/JuliusBrussee/caveman/pull/900): `/caveman-stats` and the statusline showed no cost-savings figure at all on any Claude 5 session, because the pricing table only recognized Claude 3/4 model names

### [gstack](https://github.com/garrytan/gstack) ![stars](https://img.shields.io/github/stars/garrytan/gstack?style=flat&label=stars&color=yellow)
- Fixed [#2409](https://github.com/garrytan/gstack/pull/2409): setup docs told agents to run two memory-sync scripts as bare commands, which fail with "No such file or directory" since they're plain `.ts` files with no bin alias — corrected to the proper `bun run` invocation
- Fixed [#2615](https://github.com/garrytan/gstack/pull/2615): a test meant to catch a missing gbrain install leaked the real system PATH, so it passed even when the bug was present on machines where gbrain is actually installed (e.g. Homebrew on Apple Silicon)

### [rueidis](https://github.com/redis/rueidis) ![stars](https://img.shields.io/github/stars/redis/rueidis?style=flat&label=stars&color=yellow) 
- Fixed [#1023](https://github.com/redis/rueidis/pull/1023): `rueidiscompatmock` panicked with "unexpected call to DoCache" whenever a test tried to mock a client-side-cached `Cache(ttl)` call, instead of routing it through the existing expectation queue.

### [tslearn](https://github.com/tslearn-team/tslearn) ![stars](https://img.shields.io/github/stars/tslearn-team/tslearn?style=flat&label=stars&color=yellow)
- Fixed [#703](https://github.com/tslearn-team/tslearn/pull/703) - Added `silhouette_samples()` for time-series clustering, giving per-series silhouette scores (for outlier detection and silhouette plots) with DTW/soft-DTW metrics — previously only the single aggregate score was available, forcing a manual workaround

### [OpenMAIC](https://github.com/THU-MAIC/OpenMAIC) ![stars](https://img.shields.io/github/stars/THU-MAIC/OpenMAIC?style=flat&label=stars&color=yellow)
- Fixed [#1144](https://github.com/THU-MAIC/OpenMAIC/pull/1144) - Added a "Download Script" feature letting teachers export a classroom's narration text as Markdown or a real Word `.docx` for lesson prep, localized across all 12 supported languages

### [plano](https://github.com/katanemo/plano) ![stars](https://img.shields.io/github/stars/katanemo/plano?style=flat&label=stars&color=yellow)
- Fixed [#1018](https://github.com/katanemo/plano/pull/1018): fast, short streaming responses could crash the LLM gateway worker with a divide-by-zero error while recording throughput metrics, taking down other requests sharing that worker

### [openstreetmap-website](https://github.com/openstreetmap/openstreetmap-website) ![stars](https://img.shields.io/github/stars/openstreetmap/openstreetmap-website?style=flat&label=stars&color=yellow)
- Fixed [#7297](https://github.com/openstreetmap/openstreetmap-website/pull/7297): future-tense block-expiry text ("in 3 days") bypassed the app's own translation file and fell back to an English-only default

### [pypdf](https://github.com/py-pdf/pypdf) ![stars](https://img.shields.io/github/stars/py-pdf/pypdf?style=flat&label=stars&color=yellow)
- Fixed [#3998](https://github.com/py-pdf/pypdf/pull/3998): PDF outline items created with `is_open=False` still showed expanded in PDF viewers, because the writer never actually marked them collapsed per the PDF spec

### [loopx](https://github.com/huangruiteng/loopx) ![stars](https://img.shields.io/github/stars/huangruiteng/loopx?style=flat&label=stars&color=yellow)
- Fixed [#2801](https://github.com/huangruiteng/loopx/pull/2801): repeated `/loopx` calls picked a random agent each time instead of remembering which one a conversation was already using

### [AgentMemory](https://github.com/rohitg00/agentmemory) ![stars](https://img.shields.io/github/stars/rohitg00/agentmemory?style=flat&label=stars&color=yellow)
- Fixed [#1132](https://github.com/rohitg00/agentmemory/pull/1132): deleting a memory could falsely say "deleted" when nothing was actually removed, and there was no way to delete a saved lesson at all — both now fixed

### [qm](https://github.com/yc-software/qm) ![stars](https://img.shields.io/github/stars/yc-software/qm?style=flat&label=stars&color=yellow)
- Fixed [#149](https://github.com/yc-software/qm/pull/149): a brief database hiccup while waiting for a job to finish could crash the whole process instead of just timing out safely

### [Buzz](https://github.com/block/buzz) ![stars](https://img.shields.io/github/stars/block/buzz?style=flat&label=stars&color=yellow)
- Fixed [#4500](https://github.com/block/buzz/pull/4500): docs told users to import agent packs via a "zip file + Install Pack button" that doesn't exist anymore in the app, now corrected to match the real import flow

### [tesseract-ocr](https://github.com/tesseract-ocr/tesseract) ![stars](https://img.shields.io/github/stars/tesseract-ocr/tesseract?style=flat&label=stars&color=yellow)
- [#4609](https://github.com/tesseract-ocr/tesseract/pull/4609) - `UNICHAR::UTF8ToUTF32` read one byte past a string ending in a truncated multibyte UTF-8 prefix — a real out-of-bounds read confirmed under AddressSanitizer; now clamps the step to the bytes actually remaining and returns empty on invalid input as documented

### [planning-with-files](https://github.com/OthmanAdi/planning-with-files) ![stars](https://img.shields.io/github/stars/OthmanAdi/planning-with-files?style=flat&label=stars&color=yellow)
- Audited [#216](https://github.com/OthmanAdi/planning-with-files/pull/216): found 5 duplicate language skills had silently drifted out of sync (missing bug fixes, missing features)

### [OpenMausBot](https://github.com/milind-soni/OpenMausBot) ![stars](https://img.shields.io/github/stars/milind-soni/OpenMausBot?style=flat&label=stars&color=yellow)
- Fixed [#230](https://github.com/milind-soni/OpenMausBot/pull/230): two permission requests arriving with the same ID could silently clobber each other, leaving one request permanently stuck with no way to answer it — now the second one is rejected outright instead of overwriting the first
- Fixed [#234](https://github.com/milind-soni/OpenMausBot/pull/234): a test suite from #230 broke on Windows because four test cases accidentally shared the same truncated identifier, causing one test's leftover named pipe to block the next — renamed the IDs and added a check.

### [impeccable](https://github.com/pbakaus/impeccable) ![stars](https://img.shields.io/github/stars/pbakaus/impeccable?style=flat&label=stars&color=yellow)
- Diagnosed [#551](https://github.com/pbakaus/impeccable/pull/551): `hooks reset` silently re-armed a disabled hook because it deleted the config but left provider manifests wired — fix credited by name in the merged follow-up ([#668](https://github.com/pbakaus/impeccable/pull/668))
