# Hey, I'm Som Samantray

[![LinkedIn](https://img.shields.io/badge/LinkedIn-som--samantray-blue?style=flat&logo=linkedin)](https://linkedin.com/in/som-samantray)

Tinkering with AI and building skills

## Building:

- [mac-storage-doctor](https://github.com/SomSamantray/mac-storage-doctor) ![stars](https://badgen.net/github/stars/SomSamantray/mac-storage-doctor?color=yellow&label=stars) - A Claude skill that audits a Mac's disk usage — orphaned app data, dev-tool caches, git repo bloat, rarely-used apps — and reports exactly what's safe to delete, with nothing ever removed without explicit per-item confirmation
- [dwnld-any](https://github.com/SomSamantray/dwnld-any) ![stars](https://badgen.net/github/stars/SomSamantray/dwnld-any?color=yellow&label=stars) - Agent skill + local CLI for downloading videos from 8 platforms (YouTube, Instagram, X, Reddit, and more) via yt-dlp, no cloud deploy.
- [tidbits](https://github.com/SomSamantray/tidbits) ![stars](https://badgen.net/github/stars/SomSamantray/tidbits?color=yellow&label=stars) - Bite-sized trivia website built with Next.js 16 and Turso/libSQL.
- [airesearch](https://github.com/SomSamantray/airesearch) ![stars](https://badgen.net/github/stars/SomSamantray/airesearch?color=yellow&label=stars) - Claude Code/Codex research skill that runs a deterministic engine (not the LLM) to pull evidence-led findings across X, Reddit, arXiv, GitHub, HN, and YouTube.
- [Claude-Dashboard](https://github.com/SomSamantray/Claude-Dashboard) ![stars](https://badgen.net/github/stars/SomSamantray/Claude-Dashboard?color=yellow&label=stars) - Local analytics dashboard for Claude Code usage — tokens, costs, sessions, heatmaps.
- [Claude-Code-Token-Limit](https://github.com/SomSamantray/Claude-Code-Token-Limit) ![stars](https://badgen.net/github/stars/SomSamantray/Claude-Code-Token-Limit?color=yellow&label=stars) - Claude Code plugin that shows context window %, turns remaining, and daily/weekly token budgets after every response.


## Opensource Contributions:

### [hermes-agent](https://github.com/NousResearch/hermes-agent) ![stars](https://badgen.net/github/stars/NousResearch/hermes-agent?color=yellow&label=stars)
- Diagnosed and fixed [#92242](https://github.com/NousResearch/hermes-agent/pull/92242): large streamed tool calls (big `write_file`/`apply_patch` payloads) got quadratically slower to assemble as more chunks arrived, credited by the maintainer in the merged salvage ([#101906](https://github.com/NousResearch/hermes-agent/pull/101906))

### [gstack](https://github.com/garrytan/gstack) ![stars](https://badgen.net/github/stars/garrytan/gstack?color=yellow&label=stars)
- Fixed [#2966](https://github.com/garrytan/gstack/pull/2966): Codex templates now report `mktemp` failures clearly instead of continuing with empty temp-file paths; carried into merged release [#3057](https://github.com/garrytan/gstack/pull/3057).
- Fixed [#2961](https://github.com/garrytan/gstack/pull/2961): Ubuntu 26.04 setup now selects the Playwright browser build for the host architecture; carried into merged release [#2959](https://github.com/garrytan/gstack/pull/2959).
- Fixed [#2409](https://github.com/garrytan/gstack/pull/2409): setup docs told agents to run two memory-sync scripts as bare commands, which fail with "No such file or directory" since they're plain `.ts` files with no bin alias — corrected to the proper `bun run` invocation
- Fixed [#2615](https://github.com/garrytan/gstack/pull/2615): a test meant to catch a missing gbrain install leaked the real system PATH, so it passed even when the bug was present on machines where gbrain is actually installed (e.g. Homebrew on Apple Silicon)
- Fixed [#2976](https://github.com/garrytan/gstack/pull/2976): design-detect only looked for the Impeccable skill in its legacy install path, so anyone who installed it as a Claude Code plugin (the current normal way) always got reported as not having it — commits retained and merged via maintainer's hardening pass ([#2978](https://github.com/garrytan/gstack/pull/2978))
- Fixed [#2965](https://github.com/garrytan/gstack/pull/2965): the Aside readiness probe reported `NEEDS_ASIDE` when the CLI was installed at `~/.local/bin` but that directory wasn't on `PATH` — it now finds and uses the CLI there; fix ported and credited in merged release PR [#3025](https://github.com/garrytan/gstack/pull/3025)

### [Node.js](https://github.com/nodejs/node) ![stars](https://badgen.net/github/stars/nodejs/node?color=yellow&label=stars)
- [#65243](https://github.com/nodejs/node/pull/65243) - Clarified the `process` signal docs: `SIGTERM`/`SIGINT` listeners run asynchronously, so an otherwise-idle process can exit before the listener actually runs — a gap that had confused users since 2019

### [caveman](https://github.com/JuliusBrussee/caveman) ![stars](https://badgen.net/github/stars/JuliusBrussee/caveman?color=yellow&label=stars)
- Fixed [#900](https://github.com/JuliusBrussee/caveman/pull/900): `/caveman-stats` and the statusline showed no cost-savings figure at all on any Claude 5 session, because the pricing table only recognized Claude 3/4 model names
- Fixed [#1084](https://github.com/JuliusBrussee/caveman/pull/1084): added native Grok Build support to the unified installer, including owned skill copies under `GROK_HOME/skills` and discovery in `--list`.

### [rtk](https://github.com/rtk-ai/rtk) ![stars](https://badgen.net/github/stars/rtk-ai/rtk?color=yellow&label=stars)
- Fixed [#3560](https://github.com/rtk-ai/rtk/pull/3560): three output-compaction filters (spring-boot, liquibase, ssh) had regexes so broad they silently mangled unrelated commands — e.g. any `java -jar` file got Spring-only filtering, `rm -rf /opt/liquibase` triggered liquibase compaction, and `ssh-keygen`/`ssh-add` got caught by a plain `ssh` filter

### [impeccable](https://github.com/pbakaus/impeccable) ![stars](https://badgen.net/github/stars/pbakaus/impeccable?color=yellow&label=stars)
- Diagnosed [#551](https://github.com/pbakaus/impeccable/pull/551): `hooks reset` silently re-armed a disabled hook because it deleted the config but left provider manifests wired — fix credited by name in the merged follow-up ([#668](https://github.com/pbakaus/impeccable/pull/668))

### [CPython](https://github.com/python/cpython) ![stars](https://badgen.net/github/stars/python/cpython?color=yellow&label=stars)
- Fixed [#155862](https://github.com/python/cpython/pull/155862): `class MyFlag(Mixin, Flag)` silently threw away the mixin's own `|`/`&`/`^` operator overrides in favor of `Flag`'s defaults, because `enum.py` never checked what the mixin's operators actually resolved to before overwriting them

### [tesseract-ocr](https://github.com/tesseract-ocr/tesseract) ![stars](https://badgen.net/github/stars/tesseract-ocr/tesseract?color=yellow&label=stars)
- [#4609](https://github.com/tesseract-ocr/tesseract/pull/4609) - `UNICHAR::UTF8ToUTF32` read one byte past a string ending in a truncated multibyte UTF-8 prefix — a real out-of-bounds read confirmed under AddressSanitizer; now clamps the step to the bytes actually remaining and returns empty on invalid input as documented

### [VoiceStudio](https://github.com/debpalash/VoiceStudio) ![stars](https://badgen.net/github/stars/debpalash/VoiceStudio?color=yellow&label=stars)
- [Setup wizard](https://github.com/debpalash/VoiceStudio/pull/1930) - Stopped the consent and dictation steps repeating the same title 2-3 times on one screen: real description subtitles across all 21 locales, redundant card heading removed

### [Last30Days Skill](https://github.com/mvanhorn/last30days-skill) ![stars](https://badgen.net/github/stars/mvanhorn/last30days-skill?color=yellow&label=stars)
- Fixed [#1009](https://github.com/mvanhorn/last30days-skill/pull/1009): YouTube search now uses a ScrapeCreators backstop below the thin-results floor, preserves yt-dlp results, and marks degraded lanes partial; carried into merged [#1248](https://github.com/mvanhorn/last30days-skill/pull/1248).
- [#911](https://github.com/mvanhorn/last30days-skill/pull/911) - Windows setup silently failed to auto-install `npx` because the resolved path wasn't passed to the install command
- [#912](https://github.com/mvanhorn/last30days-skill/pull/912) - Four bugs: `--web-backend=keyless` flag was rejected by the CLI, arXiv searches returned nothing for normal phrases, source links showed as plain text instead of clickable links, and Truth Social requests were blocked by Cloudflare
- [#955](https://github.com/mvanhorn/last30days-skill/pull/955) - GitHub searches for a topic could silently return zero results because the tool's own date filter clashed with search filters already baked into the query
- [#1083](https://github.com/mvanhorn/last30days-skill/pull/1083) - Reddit enrichment slots skipping high-comment threads
- Fixed [#1072](https://github.com/mvanhorn/last30days-skill/pull/1072): the X-search subprocess was handed a full copy of the environment, so every unrelated API key or secret on the machine could leak to it if that vendored client were ever compromised — now it only receives an explicit allowlist of the variables it actually needs
- [#1098](https://github.com/mvanhorn/last30days-skill/pull/1098) - Added a live CI status badge (Validate workflow, which runs the full pytest suite on every push/PR) to the README across all seven language translations, closing a long-open visibility request instead of duplicating the suite with a redundant second workflow
- [#970](https://github.com/mvanhorn/last30days-skill/pull/970) - GitHub search qualifiers wrapped in parentheses, quotes, or brackets (e.g. `(created:>2025-03-20)`) still slipped past the earlier strip, colliding with the tool's own date filter and silently returning zero results
- [#1027](https://github.com/mvanhorn/last30days-skill/pull/1027) - X search kept reporting "not authenticated" even with valid credentials, because it only recognized xurl's old flat credential file, not its current directory-based layout
- [#1126](https://github.com/mvanhorn/last30days-skill/pull/1126) - When Claude Desktop leaves an API key field blank, it writes a literal placeholder string instead of nothing — this was being read as a valid credential, so the tool reported healthy setup right up until the request hit the real API and failed

### [MemPalace](https://github.com/MemPalace/mempalace) ![stars](https://badgen.net/github/stars/MemPalace/mempalace?color=yellow&label=stars)
- [#2342](https://github.com/MemPalace/mempalace/pull/2342) - Pre-commit's Ruff hook could drift from the version pinned in `pyproject.toml` and CI, letting local checks silently pass or fail differently than CI; aligned all three sources and scoped version extraction to the Ruff hook block so unrelated hook bumps can't trip the check

### [chrome-devtools-mcp](https://github.com/ChromeDevTools/chrome-devtools-mcp) ![stars](https://badgen.net/github/stars/ChromeDevTools/chrome-devtools-mcp?color=yellow&label=stars)
- Fixed [#3085](https://github.com/ChromeDevTools/chrome-devtools-mcp/pull/3085): slim-mode `evaluate` failures looked like successful text responses instead of errors; they now return `Error: …` with `isError: true`, while successful response text stays unchanged.

### [LocalAI](https://github.com/mudler/LocalAI) ![stars](https://badgen.net/github/stars/mudler/LocalAI?color=yellow&label=stars)
- Fixed [#11652](https://github.com/mudler/LocalAI/pull/11652): the whisper backend ignored the port LocalAI actually launched it on and always bound to a hardcoded default, causing a misleading "connection unavailable" error instead of working

### [OpenMAIC](https://github.com/THU-MAIC/OpenMAIC) ![stars](https://badgen.net/github/stars/THU-MAIC/OpenMAIC?color=yellow&label=stars)
- Fixed [#1144](https://github.com/THU-MAIC/OpenMAIC/pull/1144) - Added a "Download Script" feature letting teachers export a classroom's narration text as Markdown or a real Word `.docx` for lesson prep, localized across all 12 supported languages
- Fixed [#1621](https://github.com/THU-MAIC/OpenMAIC/pull/1621): extracted a shared narration walk for script and speaker-notes exports, keeping speech-text handling consistent across both.

### [open-notebook](https://github.com/lfnovo/open-notebook) ![stars](https://badgen.net/github/stars/lfnovo/open-notebook?color=yellow&label=stars)
- Fixed [#1360](https://github.com/lfnovo/open-notebook/pull/1360): stored provider API keys now use versioned PBKDF2-HMAC-SHA256 derivation, while legacy values remain readable and can be migrated in place.

### [Buzz](https://github.com/block/buzz) ![stars](https://badgen.net/github/stars/block/buzz?color=yellow&label=stars)
- Fixed [#4500](https://github.com/block/buzz/pull/4500): docs told users to import agent packs via a "zip file + Install Pack button" that doesn't exist anymore in the app, now corrected to match the real import flow

### [github-chinese](https://github.com/maboloshi/github-chinese) ![stars](https://badgen.net/github/stars/maboloshi/github-chinese?color=yellow&label=stars)
- Fixed [#806](https://github.com/maboloshi/github-chinese/pull/806): added Simplified and Traditional Chinese feature-request templates.
- Fixed [#805](https://github.com/maboloshi/github-chinese/pull/805): fixed a leftover “on” after translating a time element.

### [Recordly](https://github.com/webadderallorg/Recordly) ![stars](https://badgen.net/github/stars/webadderallorg/Recordly?color=yellow&label=stars)
- Fixed [#1127](https://github.com/webadderallorg/Recordly/pull/1127): microphone and system audio companion files such as `recording-mic.wav` or `system.mp4` could be treated as mixed audio and routed to the wrong track; the fix recognizes supported filename patterns and routes each file to its matching track.
- Fixed [#1003](https://github.com/webadderallorg/Recordly/pull/1003): cancelling a screen recording left the microphone stream open in the background, so the next recording opened a second concurrent mic stream and produced silent/dead audio until the device was manually reselected

### [laya](https://github.com/NandhaKishorM/laya) ![stars](https://badgen.net/github/stars/NandhaKishorM/laya?color=yellow&label=stars)
- [#656](https://github.com/NandhaKishorM/laya/pull/656) - Added `LAYA_ROOT_PATH` support so the FastAPI server can be deployed behind a reverse proxy under a URL prefix (e.g. `/laya`), with OpenAPI/Swagger UI generating correct prefixed URLs

### [DeepAgents](https://github.com/langchain-ai/deepagents) ![stars](https://badgen.net/github/stars/langchain-ai/deepagents?color=yellow&label=stars)
- Fixed [#5747](https://github.com/langchain-ai/deepagents/pull/5747): `edit_file` with an empty search string silently corrupted files by inserting the replacement between every single character instead of erroring out

### [opendataloader-pdf](https://github.com/opendataloader-project/opendataloader-pdf) ![stars](https://badgen.net/github/stars/opendataloader-project/opendataloader-pdf?color=yellow&label=stars)
- [#710](https://github.com/opendataloader-project/opendataloader-pdf/pull/710) - Made the hybrid backend's page batch size configurable (`--hybrid-chunk-size`) instead of a fixed 50, letting users on constrained backends shrink batches to avoid a known request-hang issue
- Fixed [#771](https://github.com/opendataloader-project/opendataloader-pdf/pull/771): JSON output could retain a NUL from an unmapped `<0000>` ToUnicode mapping, disrupting extracted text; it now omits the NUL while preserving the surrounding paragraph.

### [AgentMemory](https://github.com/rohitg00/agentmemory) ![stars](https://badgen.net/github/stars/rohitg00/agentmemory?color=yellow&label=stars)
- Fixed [#1132](https://github.com/rohitg00/agentmemory/pull/1132): deleting a memory could falsely say "deleted" when nothing was actually removed, and there was no way to delete a saved lesson at all — both now fixed

### [Actual Budget](https://github.com/actualbudget/actual) ![stars](https://badgen.net/github/stars/actualbudget/actual?color=yellow&label=stars)
- Fixed [#8719](https://github.com/actualbudget/actual/pull/8719): merging two payees left "one of"/"not one of" rule conditions with the merged payee listed twice, so deleting the visible duplicate in the UI silently deleted both underlying entries and dropped the payee from the rule entirely

### [mastra-ai/mastra](https://github.com/mastra-ai/mastra) ![stars](https://badgen.net/github/stars/mastra-ai/mastra?color=yellow&label=stars)
- [#24239](https://github.com/mastra-ai/mastra/pull/24239) - Multi-step agentic loops with Observational Memory enabled could crash with `Turn already ended` when a sealed turn got reused on the same message list; the processor now discards an ended turn before reuse so the next step starts fresh

### [planning-with-files](https://github.com/OthmanAdi/planning-with-files) ![stars](https://badgen.net/github/stars/OthmanAdi/planning-with-files?color=yellow&label=stars)
- Audited [#216](https://github.com/OthmanAdi/planning-with-files/pull/216): found 5 duplicate language skills had silently drifted out of sync (missing bug fixes, missing features)
- Fixed [#291](https://github.com/OthmanAdi/planning-with-files/pull/291): Cursor's hooks used an old event and response schema the current Cursor runtime no longer recognizes, so plan context silently stopped reaching Cursor conversations

### [floci](https://github.com/floci-io/floci) ![stars](https://badgen.net/github/stars/floci-io/floci?color=yellow&label=stars)
- Fixed [#5448](https://github.com/floci-io/floci/pull/5448): Cognito user-pool responses now include configured prefix and custom domain names, omitting either field when it is unset.
- Fixed [#5450](https://github.com/floci-io/floci/pull/5450): imported API Gateway methods with API-key security could be called without a key, so imports now enforce `x-api-key` when every security alternative requires it while preserving access through optional alternatives.

### [Compound Engineering Plugin](https://github.com/EveryInc/compound-engineering-plugin) ![stars](https://badgen.net/github/stars/EveryInc/compound-engineering-plugin?color=yellow&label=stars)
- Fixed [#1848](https://github.com/EveryInc/compound-engineering-plugin/pull/1848): clarified which project assets Stage 4 of code review should read.
- Fixed [#1849](https://github.com/EveryInc/compound-engineering-plugin/pull/1849): made the commit workflow follow the project’s own commit conventions.
- [#1292](https://github.com/EveryInc/compound-engineering-plugin/pull/1292) - On Windows, background AI workers could quietly launch on the wrong bash (WSL instead of Git Bash) and skip work without any error
- [#1291](https://github.com/EveryInc/compound-engineering-plugin/pull/1291) - Renamed a confusing internal flag (`mode:headless` → `mode:non-interactive`) across skills, keeping the old name working temporarily so nothing breaks
- Fixed [#1733](https://github.com/EveryInc/compound-engineering-plugin/pull/1733): a fully completed code review could report its adversarial-review coverage using the exact same phrase as a skipped one, making a finished review indistinguishable from a skipped one at a glance

### [pascalorg/editor](https://github.com/pascalorg/editor) ![stars](https://badgen.net/github/stars/pascalorg/editor?color=yellow&label=stars)
- [#636](https://github.com/pascalorg/editor/pull/636) - `exportFloorplanPdf` wasn't exported from the package, blocking host apps from building their own floorplan-export UI outside the built-in Settings panel; also deduped a repeated export-scope check into one shared predicate with direct test coverage

### [CodexBar](https://github.com/steipete/CodexBar) ![stars](https://badgen.net/github/stars/steipete/CodexBar?color=yellow&label=stars)
- Fixed [#3438](https://github.com/steipete/CodexBar/pull/3438): China-region Moonshot account balances and deficits were mislabeled in USD instead of CNY, both in the menu bar display and CLI output

### [qm](https://github.com/yc-software/qm) ![stars](https://badgen.net/github/stars/yc-software/qm?color=yellow&label=stars)
- Fixed [#149](https://github.com/yc-software/qm/pull/149): a brief database hiccup while waiting for a job to finish could crash the whole process instead of just timing out safely

### [semantica](https://github.com/semantica-agi/semantica) ![stars](https://badgen.net/github/stars/semantica-agi/semantica?color=yellow&label=stars)
- [#1595](https://github.com/semantica-agi/semantica/pull/1595) - Added a Looker connector (Looks, Dashboards, LookML models, Folders, Projects) as an optional dependency, plus SSRF hardening on the SDK's session (URL/DNS-rebind validation, forced TLS, zero redirects, secret-field stripping) since the official SDK builds its own HTTP transport outside the repo's existing request guard

### [Needle](https://github.com/cactus-compute/needle) ![stars](https://badgen.net/github/stars/cactus-compute/needle?color=yellow&label=stars)
- [#98](https://github.com/cactus-compute/needle/pull/98) - Made the setup script auto-detect and prefer `uv` (10-100x faster than pip) when available, falling back to pip only when it isn't installed
- [#123](https://github.com/cactus-compute/needle/pull/123): a correctly-extracted number was rejected as "fabricated" whenever the source text wrote it with a thousands separator (e.g. `$1,200.00`), since the grounding check compared values as plain text instead of as numbers — this broke even the README's own example
- [#124](https://github.com/cactus-compute/needle/pull/124): the acceptance suites' pass/fail scoring rule (90% threshold, critical-failure override, confidence gate) was documented but never actually tested, so a silent change to it could ship without anyone noticing — pinned with regression tests and documented what a red suite means

### [ebiten](https://github.com/hajimehoshi/ebiten) ![stars](https://badgen.net/github/stars/hajimehoshi/ebiten?color=yellow&label=stars)
- Fixed [#3921](https://github.com/hajimehoshi/ebiten/pull/3921): corrected `RestoreWindow` behavior when the window has finite size limits.

### [trino](https://github.com/trinodb/trino) ![stars](https://badgen.net/github/stars/trinodb/trino?color=yellow&label=stars)
- Fixed [#31540](https://github.com/trinodb/trino/pull/31540): wide Iceberg ORC tables could miss metrics for sorted columns beyond the inferred-column limit, and `OPTIMIZE` could miss NULLs in required columns when metrics were disabled; metrics now honor the output schema and sort order, and required columns retain null counts.

### [kiss-translator](https://github.com/fishjar/kiss-translator) ![stars](https://badgen.net/github/stars/fishjar/kiss-translator?color=yellow&label=stars)
- Fixed [#1167](https://github.com/fishjar/kiss-translator/pull/1167): translating nearby text no longer gives unloaded inline images zero dimensions, preventing blank image previews.

### [apify-mcp-server](https://github.com/apify/apify-mcp-server) ![stars](https://badgen.net/github/stars/apify/apify-mcp-server?color=yellow&label=stars)
- Fixed [#1315](https://github.com/apify/apify-mcp-server/pull/1315): running the conformance test suite locally leaked the raw `APIFY_TOKEN` to the terminal in plain text — CI masked it, but the local script had no equivalent redaction

### [Unciv](https://github.com/yairm210/Unciv) ![stars](https://badgen.net/github/stars/yairm210/Unciv?color=yellow&label=stars)
- Fixed [#15756](https://github.com/yairm210/Unciv/pull/15756): restored ruleset order for promotion battle modifiers so they appear in the same order as the promotions in the battle preview.

### [pypdf](https://github.com/py-pdf/pypdf) ![stars](https://badgen.net/github/stars/py-pdf/pypdf?color=yellow&label=stars)
- Fixed [#3998](https://github.com/py-pdf/pypdf/pull/3998): PDF outline items created with `is_open=False` still showed expanded in PDF viewers, because the writer never actually marked them collapsed per the PDF spec

### [filebrowser](https://github.com/gtsteffaniak/filebrowser) ![stars](https://badgen.net/github/stars/gtsteffaniak/filebrowser?color=yellow&label=stars)
- Fixed [#3125](https://github.com/gtsteffaniak/filebrowser/pull/3125): admins using `createUserDir` could be narrowed to a personal folder; new admins now keep the source root and skip personal-directory creation, while non-admins still get their own directory.

### [plano](https://github.com/katanemo/plano) ![stars](https://badgen.net/github/stars/katanemo/plano?color=yellow&label=stars)
- Fixed [#1018](https://github.com/katanemo/plano/pull/1018): fast, short streaming responses could crash the LLM gateway worker with a divide-by-zero error while recording throughput metrics, taking down other requests sharing that worker

### [loopx](https://github.com/loopx-project/loopx) ![stars](https://badgen.net/github/stars/loopx-project/loopx?color=yellow&label=stars)
- Fixed [#2801](https://github.com/huangruiteng/loopx/pull/2801): repeated `/loopx` calls picked a random agent each time instead of remembering which one a conversation was already using

### [Cloudflare Docs](https://github.com/cloudflare/cloudflare-docs) ![stars](https://badgen.net/github/stars/cloudflare/cloudflare-docs?color=yellow&label=stars)
- Fixed [#33406](https://github.com/cloudflare/cloudflare-docs/pull/33406): the Workers AI JSON Mode docs listed three models as supporting it even though none of their schemas actually declare that capability, misleading anyone trying to use it
- Fixed [#33408](https://github.com/cloudflare/cloudflare-docs/pull/33408): R2 Sippy command examples rendered with a broken syntax-highlight color, because the shell syntax highlighter misread the unquoted `<BUCKET_NAME>` placeholder as a redirect operator

### [OpenMausBot](https://github.com/milind-soni/OpenMausBot) ![stars](https://badgen.net/github/stars/milind-soni/OpenMausBot?color=yellow&label=stars)
- Fixed [#2633](https://github.com/milind-soni/OpenMausBot/pull/2633): reduced glass pop-up flicker on Windows.
- Fixed [#230](https://github.com/milind-soni/OpenMausBot/pull/230): two permission requests arriving with the same ID could silently clobber each other, leaving one request permanently stuck with no way to answer it — now the second one is rejected outright instead of overwriting the first
- Fixed [#234](https://github.com/milind-soni/OpenMausBot/pull/234): a test suite from #230 broke on Windows because four test cases accidentally shared the same truncated identifier, causing one test's leftover named pipe to block the next — renamed the IDs and added a check.

### [chat-on-steroids](https://github.com/totec448-spec/chat-on-steroids) ![stars](https://badgen.net/github/stars/totec448-spec/chat-on-steroids?color=yellow&label=stars)
- Fixed [#1555](https://github.com/totec448-spec/chat-on-steroids/pull/1555): users could only select Skills from leading slash completion and had no inline project-file references; added inline `/` Skill and `@` file pickers that insert references as text without running app commands.

### [cherry-markdown](https://github.com/Tencent/cherry-markdown) ![stars](https://badgen.net/github/stars/Tencent/cherry-markdown?color=yellow&label=stars)
- Fixed [#1901](https://github.com/Tencent/cherry-markdown/pull/1901): applying a heading level to a multiline selection containing ordinary text and an existing heading did not update both lines consistently; it now applies the selected level to each line while preserving spacing after an existing marker.

### [CLI Printing Press](https://github.com/mvanhorn/cli-printing-press) ![stars](https://badgen.net/github/stars/mvanhorn/cli-printing-press?color=yellow&label=stars)
- Fixed [#4990](https://github.com/mvanhorn/cli-printing-press/pull/4990): when dogfood still failed after two fix loops, the receipt system rejected the handoff to archive manuscripts; it now records the hold and archives without promoting the failed CLI.
- [#4049](https://github.com/mvanhorn/cli-printing-press/pull/4049) - A passing local check still let an unrewritten module path slip into a packaged CLI; added a module-path check and surfaced the review-gate rules agents were missing
- [#3855](https://github.com/mvanhorn/cli-printing-press/pull/3855) - Windows credential tests failed because sandbox test folders had overly loose permissions, now locked to owner-only
- [#3856](https://github.com/mvanhorn/cli-printing-press/pull/3856) - A Windows test failure showed the wrong folder path, making the real problem hard to track down
- [#3857](https://github.com/mvanhorn/cli-printing-press/pull/3857) - Generated export/sync tools could report "success" even when saving the file actually failed
- [#1890](https://github.com/mvanhorn/printing-press-library/pull/1890) - Google Search Console CLI's `sitemaps-submit`/`get`/`delete` 404'd whenever a feedpath was an absolute URL, since the raw `https://` slashes split the REST path; now percent-encoded as a single path segment so it routes correctly
- [#1893](https://github.com/mvanhorn/printing-press-library/pull/1893) - Movie Goat CLI's local/offline search silently returned zero results (exit 0) because the untyped search branch never assigned results, and separately crashed on FTS5-syntax queries like `Space: 1999`; both fixed with real FTS hits and per-token query sanitization
- Fixed [#4829](https://github.com/mvanhorn/cli-printing-press/pull/4829): dogfood testing flagged a false WARN for CLIs with no sync command at all, mistaking "no sync command exists" for "sync command uses generic Upsert calls"

### [FluxDown](https://github.com/zerx-lab/FluxDown) ![stars](https://badgen.net/github/stars/zerx-lab/FluxDown?color=yellow&label=stars)
- Fixed [#849](https://github.com/zerx-lab/FluxDown/pull/849): users were pointed to a nonexistent in-app feedback button; issue templates and READMEs now direct them to the website feedback page, and the English/Chinese interface guides no longer describe the button.

### [wanderer](https://github.com/open-wanderer/wanderer) ![stars](https://badgen.net/github/stars/open-wanderer/wanderer?color=yellow&label=stars)
- Fixed [#1384](https://github.com/open-wanderer/wanderer/pull/1384): notifications disappeared from October through February because PocketBase compared numeric `@month` against ISO timestamps; removing the month cutoff lets users see notifications year-round.

### [quickjs-ng](https://github.com/quickjs-ng/quickjs) ![stars](https://badgen.net/github/stars/quickjs-ng/quickjs?color=yellow&label=stars)
- Fixed [#1657](https://github.com/quickjs-ng/quickjs/pull/1657): `quickjs.c` failed to compile on GCC 14+ for any ESP32 target, because six call sites passed `int*` where the platform's `int32_t*` was expected (or vice versa)

### [WordPress-iOS](https://github.com/wordpress-mobile/WordPress-iOS) ![stars](https://badgen.net/github/stars/wordpress-mobile/WordPress-iOS?color=yellow&label=stars)
- Fixed [#26137](https://github.com/wordpress-mobile/WordPress-iOS/pull/26137): clearing the Store Sandbox secret could leave a stale cookie in WebKit and send checkout to the wrong store; the fix synchronizes cookie updates and deletion across shared storage and WebKit.

### [tuicr](https://github.com/agavra/tuicr) ![stars](https://badgen.net/github/stars/agavra/tuicr?color=yellow&label=stars)
- Fixed [#768](https://github.com/agavra/tuicr/pull/768): local themes reached through a symlink could not find a relative `.tmTheme` beside the target, and missing or invalid syntax files could make the theme unusable; tuicr now checks the target and falls back to bundled highlighting while preserving the local theme and surfacing a warning.

### [tslearn](https://github.com/tslearn-team/tslearn) ![stars](https://badgen.net/github/stars/tslearn-team/tslearn?color=yellow&label=stars)
- Fixed [#703](https://github.com/tslearn-team/tslearn/pull/703) - Added `silhouette_samples()` for time-series clustering, giving per-series silhouette scores (for outlier detection and silhouette plots) with DTW/soft-DTW metrics — previously only the single aggregate score was available, forcing a manual workaround

### [spliit](https://github.com/spliit-app/spliit) ![stars](https://badgen.net/github/stars/spliit-app/spliit?color=yellow&label=stars)
- Fixed [#635](https://github.com/spliit-app/spliit/pull/635): an expense dated the 1st of the month could be grouped under "Last month" while its own row still showed the 1st, because the timezone conversion for grouping (unlike display) shifted UTC-midnight dates backward for anyone west of UTC

### [rueidis](https://github.com/redis/rueidis) ![stars](https://badgen.net/github/stars/redis/rueidis?color=yellow&label=stars) 
- Fixed [#1023](https://github.com/redis/rueidis/pull/1023): `rueidiscompatmock` panicked with "unexpected call to DoCache" whenever a test tried to mock a client-side-cached `Cache(ttl)` call, instead of routing it through the existing expectation queue.

### [openstreetmap-website](https://github.com/openstreetmap/openstreetmap-website) ![stars](https://badgen.net/github/stars/openstreetmap/openstreetmap-website?color=yellow&label=stars)
- Fixed [#7297](https://github.com/openstreetmap/openstreetmap-website/pull/7297): future-tense block-expiry text ("in 3 days") bypassed the app's own translation file and fell back to an English-only default

### [trzsz-ssh](https://github.com/trzsz/trzsz-ssh) ![stars](https://badgen.net/github/stars/trzsz/trzsz-ssh?color=yellow&label=stars)
- Fixed [#288](https://github.com/trzsz/trzsz-ssh/pull/288): added support for `@` in SSH usernames.

### [Xed-Editor](https://github.com/Xed-Editor/Xed-Editor) ![stars](https://badgen.net/github/stars/Xed-Editor/Xed-Editor?color=yellow&label=stars)
- Fixed [#1708](https://github.com/Xed-Editor/Xed-Editor/pull/1708): the universal runner split script paths containing spaces before Bash could run them; the fix forwards each argument separately so paths like `My stuff/script.py` reach the runner intact.

### [Universal-G-Code-Sender](https://github.com/winder/Universal-G-Code-Sender) ![stars](https://badgen.net/github/stars/winder/Universal-G-Code-Sender?color=yellow&label=stars)
- Fixed [#3219](https://github.com/winder/Universal-G-Code-Sender/pull/3219): inch-reported GRBL positions could show incorrect calibration values, skew step estimates, and misapply jog soft limits; the wizard now converts positions to millimeters for display, estimates, and limit checks.

### [Printing Press Library](https://github.com/mvanhorn/printing-press-library) ![stars](https://badgen.net/github/stars/mvanhorn/printing-press-library?color=yellow&label=stars)
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
- [MyAnimeList](https://github.com/mvanhorn/printing-press-library/pull/1976) - Every public MyAnimeList surface in one binary, plus offline analytics the site can't answer: score-split/divisive detection, drift tracking, drop-risk scoring, per-episode consistency trends, manga-adaptation coverage, and franchise-gap detection
- [Swiggy](https://github.com/mvanhorn/printing-press-library/pull/1994) - CLI for Swiggy's MCP API (Food, Instamart, Dineout) — 51 tools plus cross-domain spend history, a safe-retry guard for failed order placement, and a UPI payment-wait command
- [Philonet](https://github.com/mvanhorn/printing-press-library/pull/2112) - CLI for Philonet (no public API; reverse-engineered from the logged-in web app): reading streaks, friends' thoughts, and unanswered-thread tracking, plus local history the web app doesn't keep — weekly/monthly reading rhythm, a read-later queue fitted to your free minutes, and which of your thoughts earned reactions
- [InvestorPaisa](https://github.com/mvanhorn/printing-press-library/pull/2333) - Nifty 200 terminal CLI for screening stocks, tracking movers and market breadth, and building local snapshot and adjusted price history

### [sleek](https://github.com/ransome1/sleek) ![stars](https://badgen.net/github/stars/ransome1/sleek?color=yellow&label=stars)
- Fixed [#924](https://github.com/ransome1/sleek/pull/924): Markdown-linked project and context values appeared as raw `[label](url)` text in the drawer and todo group headers; they now show the link label while keeping the original value for filtering.

### [split-pro](https://github.com/oss-apps/split-pro) ![stars](https://badgen.net/github/stars/oss-apps/split-pro?color=yellow&label=stars)
- Fixed [#752](https://github.com/oss-apps/split-pro/pull/752): invite-email failures now show a clear error in expense and group flows instead of appearing successful, while retaining the added friend.

### [PriceBuddy](https://github.com/jez500/pricebuddy) ![stars](https://badgen.net/github/stars/jez500/pricebuddy?color=yellow&label=stars)
- Fixed [#215](https://github.com/jez500/pricebuddy/pull/215): formatted the dashboard's Potential savings stat with the configured currency and locale, matching other dashboard values.

### [backpass](https://github.com/kunchenguid/backpass) ![stars](https://badgen.net/github/stars/kunchenguid/backpass?color=yellow&label=stars)
- Fixed [#216](https://github.com/kunchenguid/backpass/pull/216): the Quick Start omitted the default review UI's `lavish-axi` requirement and terminal fallback, so it now documents the install command and `--no-ui` option.
- Fixed [#217](https://github.com/kunchenguid/backpass/pull/217): a `CLAUDE.md` symlink to `AGENTS.md` triggered a false separate-memory warning; symlinks resolving to the same file are now treated as pointers, with regression coverage.

### [reticle](https://github.com/reticlehq/reticle) ![stars](https://badgen.net/github/stars/reticlehq/reticle?color=yellow&label=stars)
- Fixed [#1330](https://github.com/reticlehq/reticle/pull/1330): corrected `reticle_lease` documentation to use the accepted `seedStorage` keys and a valid `local` example.
- Fixed [#1332](https://github.com/reticlehq/reticle/pull/1332): added `reticle_lease` guidance to the recovery message when opening a URL fails to launch the browser.
- Fixed [#746](https://github.com/reticlehq/reticle/pull/746): a missing OS shared library (e.g. `libnspr4.so`) was misreported as "Chromium is not installed," sending users to run a reinstall command that succeeded but fixed nothing
- Fixed [#743](https://github.com/reticlehq/reticle/pull/743): `reticle init` kept reporting its install step as failed on every re-run even after the dependencies were correctly installed by hand, and gave the wrong error hint for a pnpm virtual-store conflict
- Fixed [#744](https://github.com/reticlehq/reticle/pull/744): flow files silently dropped typo'd or unsupported `expect` assertion keys instead of erroring, so a broken test could "pass" while asserting nothing at all

### [maki](https://github.com/tontinton/maki) ![stars](https://badgen.net/github/stars/tontinton/maki?color=yellow&label=stars)
- Fixed [#1265](https://github.com/tontinton/maki/pull/1265): `maki auth login` sent users setting up the Vibe / Coding profile to the outdated Codestral CLI page; it now opens Mistral’s Vibe Code extensions page, where they can create or choose an API key.

### [sdns](https://github.com/semihalev/sdns) ![stars](https://badgen.net/github/stars/semihalev/sdns?color=yellow&label=stars)
- Fixed [#711](https://github.com/semihalev/sdns/pull/711): oversized cache settings could exceed the available memory budget without warning; sdns now warns at startup and with `-t` when estimated full-occupancy memory is too high.

### [cve-lite-cli](https://github.com/OWASP/cve-lite-cli) ![stars](https://badgen.net/github/stars/OWASP/cve-lite-cli?color=yellow&label=stars)
- Fixed [#1084](https://github.com/OWASP/cve-lite-cli/pull/1084): the version comparator ranked a pre-release version (e.g. `1.2.3-beta.1`) as *greater than* its stable release, causing the vulnerability scanner to falsely report a vulnerable pre-release install as safe

### [xdsl](https://github.com/xdslproject/xdsl) ![stars](https://badgen.net/github/stars/xdslproject/xdsl?color=yellow&label=stars)
- Fixed [#6560](https://github.com/xdslproject/xdsl/pull/6560): IRDL verification now rejects negative, malformed, or inconsistent variadic segment sizes for operands and results, with clear diagnostics and regression coverage.

### [phonopy](https://github.com/phonopy/phonopy) ![stars](https://badgen.net/github/stars/phonopy/phonopy?color=yellow&label=stars)
- Fixed [#1055](https://github.com/phonopy/phonopy/pull/1055): documented the limitation on irreducible representations for magnetic space groups.

### [fud-ai](https://github.com/apoorvdarshan/fud-ai) ![stars](https://badgen.net/github/stars/apoorvdarshan/fud-ai?color=yellow&label=stars)
- Fixed [#531](https://github.com/apoorvdarshan/fud-ai/pull/531): progressive-meal thumbnails could show an earlier capture and open a different photo when tapped; they now prefer the final capture and open its matching viewer image while keeping galleries chronological.

### [mcpproxy-go](https://github.com/smart-mcp-proxy/mcpproxy-go) ![stars](https://badgen.net/github/stars/smart-mcp-proxy/mcpproxy-go?color=yellow&label=stars)
- Fixed [#1627](https://github.com/smart-mcp-proxy/mcpproxy-go/pull/1627): removing a server with more than 1,000 tools could leave the excess tools indexed; it now deletes matching tools in bounded pages and batches until none remain, while preserving other servers' tools.
