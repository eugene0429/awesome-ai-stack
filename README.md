# awesome-ai-stack

A curated catalog of AI tools — open-source and commercial (SaaS) — plus Claude Code skills, collected from the wild, researched, and organized.

> Paste new finds directly into the [`/update-tools`](#-how-this-catalog-is-maintained) command — any format, partial names fine. It researches each new entry, classifies it, and appends it to the right section below. See [How this catalog is maintained](#-how-this-catalog-is-maintained).

**Legend** · `OSS` open source · `SaaS` commercial/hosted · `Skill` Claude Code skill or plugin · `Free` free to use · `⚠️` identity not fully verified

> Skills are filed by **what they do**, not by the fact that they're skills — a marketing skill lives under marketing, a video skill under video. The `Skill` tag marks them wherever they land.

## Contents

- [Research & Academic](#research--academic)
- [RAG & Knowledge Management](#rag--knowledge-management)
- [Document Parsing & OCR](#document-parsing--ocr)
- [LLM Optimization & Local Inference](#llm-optimization--local-inference)
- [Agent Frameworks & Multi-Agent Systems](#agent-frameworks--multi-agent-systems)
- [Coding Agents & Dev Workflow](#coding-agents--dev-workflow)
- [Skill & MCP Tooling](#skill--mcp-tooling)
- [Security & Offensive Testing](#security--offensive-testing)
- [Video & Audio](#video--audio)
- [Creative & Media Generation](#creative--media-generation)
- [CAD & Engineering](#cad--engineering)
- [Business, Marketing & Career](#business-marketing--career)
- [Finance & Trading](#finance--trading)
- [Web Scraping & Browser Automation](#web-scraping--browser-automation)
- [UI / Web Design](#ui--web-design)
- [Writing, Learning & Communication](#writing-learning--communication)
- [Datasets](#datasets)
- [Open Models](#open-models)
- [System & Dev Utilities](#system--dev-utilities)
- [Curated Lists](#curated-lists)

---

## Research & Academic

Tools for literature search, paper reading, academic writing, citations, and peer review.

| Tool | What it does | Link | Tags |
|------|--------------|------|------|
| Prism | OpenAI's free AI-native LaTeX editor/workspace for scientists, with GPT integrated for paper writing, citations, and collaboration. | [openai.com/prism](https://openai.com/prism/) | `SaaS` `Free` |
| Ponder | AI research workspace for literature review and paper reading — finds relevant passages, compares sources, organizes notes in a knowledge graph. | [ponder.ing](https://ponder.ing/) | `SaaS` |
| ThesisAI | AI academic writing assistant that drafts long-form documents with inline, verified citations; supports LaTeX/Overleaf, Zotero/Mendeley. | [thesisai.io](https://www.thesisai.io/) | `SaaS` |
| Sci-bot | AI research assistant integrating Sci-Hub's paper corpus; answers questions with real academic citations (APA/MLA/IEEE…), 10+ languages, token-based pricing. | [sci-bot.ru](https://sci-bot.ru/) | `SaaS` |
| Liner | AI search assistant with Liner Scholar — a literature-review agent over 200M+ academic sources, citation recommender, hypothesis generator. | [liner.com](https://liner.com/) | `SaaS` `Free` |
| AnswerThis | YC-backed research assistant; semantic search over 300M+ papers, citation-backed literature reviews with line-by-line sources and citation maps. | [answerthis.io](https://answerthis.io/) | `SaaS` |
| PaperVizAgent | Google Research multi-agent framework that turns raw scientific content into publication-quality figures (Retriever/Planner/Stylist/Visualizer/Critic). | [github.com/google-research/papervizagent](https://github.com/google-research/papervizagent) | `OSS` |
| ScholarPeer | Google Research multi-agent framework for automated peer review — produces structured reviews grounded in live literature search. | [arxiv 2601.22638](https://arxiv.org/pdf/2601.22638) | — |
| NotebookLM | Google's AI research/notetaking tool grounded in your uploaded sources; generates summaries, FAQs, and Audio Overviews. Community Python wrappers exist. | [notebooklm.google.com](https://notebooklm.google.com) | `SaaS` `Free` |
| Keywert Insight | AI patent-research platform (Wert Intelligence) — natural-language patent search, prior-art reports, and R&D-differentiation analysis; auto-generates invention disclosures and specs. | [ai.keywert.com](https://ai.keywert.com/) | `SaaS` |
| Last30Days | Research agent/skill that searches Reddit, X, YouTube, HN, Polymarket, and the web over the past 30 days and synthesizes a sourced, weighted summary. | [github.com/mvanhorn/last30days-skill](https://github.com/mvanhorn/last30days-skill) | `OSS` `Skill` |
| autoresearch | Karpathy's project where agents autonomously run ~100 research experiments overnight on single-GPU nanochat training; you edit context files, not Python. | [github.com/karpathy/autoresearch](https://github.com/karpathy/autoresearch) | `OSS` |
| Feynman | Open-source AI research agent — a terminal CLI plus workbench app that searches and synthesizes papers with citations, runs multi-agent literature reviews (Researcher/Reviewer/Writer/Verifier), ranks papers by evidence-based relevance, audits paper claims against a codebase, and plans replication studies. Built on the Pi framework with alphaXiv search; a skills-only install exposes its research library to Codex and Claude. | [github.com/companion-inc/feynman](https://github.com/companion-inc/feynman) | `OSS` `Skill` |
| Apodex | Verification-first deep-research agent system orchestrating up to 150 sub-agents with fact-checker/conflict-reviewer roles and auditable evidence chains; ships Apache-2.0 open-weight models (Apodex-1.0, fine-tuned from Qwen3.5) and the AgentHarness eval harness. | [github.com/ApodexAI](https://github.com/ApodexAI) | `OSS` |
| WebPlotDigitizer | Free, open-source web tool that extracts numerical data from images of plots and graphs (line, bar, scatter) via axis calibration plus manual or automatic point detection; exports to CSV/JSON. | [github.com/ankitrohatgi/WebPlotDigitizer](https://github.com/ankitrohatgi/WebPlotDigitizer) | `OSS` `Free` |

## RAG & Knowledge Management

Frameworks that turn documents, code, or media into queryable knowledge.

| Tool | What it does | Link | Tags |
|------|--------------|------|------|
| RAG-Anything | All-in-one multimodal RAG framework retrieving across text, images, tables, and equations via dual-graph construction and cross-modal hybrid retrieval. | [github.com/HKUDS/RAG-Anything](https://github.com/HKUDS/RAG-Anything) | `OSS` |
| Understand-Anything | Multi-agent plugin that turns any codebase into an interactive, queryable knowledge graph with plain-English summaries and AI walkthroughs. | [github.com/Lum1104/Understand-Anything](https://github.com/Lum1104/Understand-Anything) | `OSS` `Skill` |
| Graphify | Skill that turns any folder of code/docs/papers/media into a queryable knowledge graph (Tree-sitter + NetworkX + Leiden), with Obsidian-compatible output. | [github.com/safishamsi/graphify](https://github.com/safishamsi/graphify) | `OSS` `Skill` |
| HelixDB | Open-source graph-vector database built in Rust (LMDB-backed) with a typed query language (HelixQL), combining graph traversal and vector search for RAG and agent memory. | [github.com/HelixDB/helix-db](https://github.com/HelixDB/helix-db) | `OSS` |
| cognee | Open-source AI memory engine giving agents persistent long-term memory — builds a self-hosted knowledge graph combining vector embeddings, graph reasoning, and ontology generation (remember/recall/forget operations). | [github.com/topoteretes/cognee](https://github.com/topoteretes/cognee) | `OSS` |
| SurfSense | Open-source alternative to NotebookLM/Perplexity/Glean — a personal knowledge base plus research agent connected to Slack, Linear, Jira, Notion, GitHub, YouTube, Gmail and search engines, with hybrid semantic/full-text search, cited answers, 100+ LLMs including local Ollama, and an MCP server. | [github.com/MODSetter/SurfSense](https://github.com/MODSetter/SurfSense) | `OSS` |
| Repowise | Open-source (AGPL-3.0) codebase-intelligence tool that indexes a repo's AST, dependency graph, and git history to produce code-health scores, auto-generated architecture docs/wiki, dead-code detection, and nine MCP tools for AI coding agents. Positioned as an open-source CodeScene alternative. | [github.com/repowise-dev/repowise](https://github.com/repowise-dev/repowise) | `OSS` |
| obsidian-skills | Official Agent Skills for Obsidian by its CEO Steph Ango (kepano) — teaches agents the Obsidian CLI and open formats (Markdown/wikilinks, Bases, JSON Canvas) plus Defuddle web clipping; installable as a Claude Code plugin. | [github.com/kepano/obsidian-skills](https://github.com/kepano/obsidian-skills) | `OSS` `Skill` |
| Claudian | Obsidian plugin embedding Claude Code/Codex as an AI collaborator inside your vault (read/write/search/bash with the vault as working dir). | [github.com/YishenTu/claudian](https://github.com/YishenTu/claudian) | `OSS` `Skill` |

## Document Parsing & OCR

Turning PDFs, scans, and office files into structured, LLM-ready text.

| Tool | What it does | Link | Tags |
|------|--------------|------|------|
| MinerU | Open-source document-parsing engine from OpenDataLab (Shanghai AI Lab) converting PDFs, images, and Office files into LLM-ready Markdown/JSON with layout, formula, and table recognition; companion MinerU-Document-Explorer exposes it as an MCP knowledge engine. | [github.com/opendatalab/MinerU](https://github.com/opendatalab/MinerU) | `OSS` |
| pdf-inspector | Firecrawl's fast Rust library and CLI that classifies a PDF as text-based, scanned, image, or mixed in ~10–50ms with a confidence score, extracts position-aware text, and converts to Markdown without OCR (selective OCR routing optional). Python, Node, and WASM bindings; MIT. | [github.com/firecrawl/pdf-inspector](https://github.com/firecrawl/pdf-inspector) | `OSS` `Free` |
| Unlimited-OCR | Baidu's MIT-licensed OCR vision-language model for one-shot long-horizon parsing — builds on DeepSeek-OCR but swaps decoder attention for Reference Sliding Window Attention, giving a constant KV cache so it transcribes dozens of PDF pages in a single forward pass within 32K context. | [github.com/baidu/Unlimited-OCR](https://github.com/baidu/Unlimited-OCR) | `OSS` |

## LLM Optimization & Local Inference

Run bigger models on smaller hardware; compression and efficient inference.

| Tool | What it does | Link | Tags |
|------|--------------|------|------|
| bitnet.cpp | Microsoft's official inference framework for 1-bit (1.58-bit) LLMs, with optimized kernels that cut compute and energy dramatically. | [github.com/microsoft/BitNet](https://github.com/microsoft/BitNet) | `OSS` |
| ntransformer | Dependency-free C++/CUDA engine running Llama 3.1 70B on a single RTX 3090 via 3-tier adaptive caching (VRAM + RAM + NVMe). Trades speed for fit. | [github.com/xaskasdf/ntransformer](https://github.com/xaskasdf/ntransformer) | `OSS` |
| Turbovec | Rust vector index (Python bindings) implementing TurboQuant — training-free 2–4 bit vector compression with SIMD nearest-neighbor search for local RAG. | [github.com/RyanCodrai/turbovec](https://github.com/RyanCodrai/turbovec) | `OSS` |
| AirLLM | Layer-by-layer sharding so a 70B model runs on a single 4GB GPU (405B on 8GB) with no quantization/distillation. | [github.com/lyogavin/airllm](https://github.com/lyogavin/airllm) | `OSS` |
| Colibri | Minimal, dependency-free pure-C inference engine that runs a 744B-parameter GLM MoE model on consumer machines with as little as 25GB RAM by streaming experts from disk; exposes an OpenAI-compatible HTTP API. | [github.com/JustVugg/colibri](https://github.com/JustVugg/colibri) | `OSS` |
| pxpipe | Local proxy (TypeScript, MIT) that intercepts LLM API calls and renders bulky text blocks (code, JSON, tool output) as compact PNG images before forwarding, cutting token costs ~59–70%. Lossy — unreliable for exact strings/hashes/secrets. | [github.com/teamchong/pxpipe](https://github.com/teamchong/pxpipe) | `OSS` `Free` |

## Agent Frameworks & Multi-Agent Systems

Building, training, and orchestrating autonomous and swarm agents.

| Tool | What it does | Link | Tags |
|------|--------------|------|------|
| Agent Lightning | Microsoft framework adding RL, prompt optimization, and fine-tuning to any agent with near-zero code changes; works with LangChain, AutoGen, CrewAI, etc. | [github.com/microsoft/agent-lightning](https://github.com/microsoft/agent-lightning) | `OSS` |
| Hermes Agent | Open-source self-improving agent with a closed learning loop — writes reusable skill files, stores outcomes in memory, refines across sessions. | [github.com/NousResearch/hermes-agent](https://github.com/NousResearch/hermes-agent) | `OSS` |
| MetaGPT | Multi-agent framework simulating a software company — roles (PM, architect, engineer) follow SOPs to turn one line into PRDs, designs, and code. | [github.com/FoundationAgents/MetaGPT](https://github.com/FoundationAgents/MetaGPT) | `OSS` |
| MiroFish | Swarm-intelligence prediction engine spinning up thousands-to-millions of agents in parallel simulated social worlds to forecast outcomes (on CAMEL-AI OASIS). | [github.com/666ghj/MiroFish](https://github.com/666ghj/MiroFish) | `OSS` |
| ruflo | Multi-agent meta-harness for Claude Code/Codex — coordinating agent swarms with adaptive memory, self-learning, GOAP planning, RAG, and federated comms. | [github.com/ruvnet/ruflo](https://github.com/ruvnet/ruflo) | `OSS` `Skill` |
| LLM Council | Andrej Karpathy's web app where several LLMs answer a query, anonymously peer-review each other's responses, and a "chairman" model synthesizes the final answer. | [github.com/karpathy/llm-council](https://github.com/karpathy/llm-council) | `OSS` `Free` |
| claude-peers | MCP-based peer-discovery channel letting multiple running Claude Code instances find each other and message ad-hoc via a localhost broker. | [github.com/louislva/claude-peers-mcp](https://github.com/louislva/claude-peers-mcp) | `OSS` `Skill` |
| Agency Agents | Catalog of 230+ specialized subagent personas — a whole "AI agency" across 15+ divisions including engineering, design, marketing, product, security, finance, and game dev, each a Markdown persona with its own voice, process, and deliverables. Ships native installers for Claude Code, Copilot, Cursor, OpenCode, Aider, and Windsurf, plus a desktop app. MIT. | [github.com/msitarzewski/agency-agents](https://github.com/msitarzewski/agency-agents) | `OSS` `Skill` |

## Coding Agents & Dev Workflow

Agent harnesses, meta-frameworks, memory, and the methodology layer around AI coding.

| Tool | What it does | Link | Tags |
|------|--------------|------|------|
| OpenCode | Popular open-source, provider-agnostic AI coding agent for the terminal — works with Claude, OpenAI, Google, or local models. Formerly `sst/opencode`; pairs well with open models like Nemotron 3 for fully local agent stacks. | [github.com/anomalyco/opencode](https://github.com/anomalyco/opencode) | `OSS` `Free` |
| jcode | Terminal AI coding-agent harness (Rust) with fast boot (~14ms), low RAM, semantic/vector memory, native multi-agent "swarm" subagent delegation, and 30+ LLM providers. | [github.com/1jehuang/jcode](https://github.com/1jehuang/jcode) | `OSS` |
| superpowers | Agentic skills framework and dev methodology — composable skills (brainstorming, TDD, debugging, verification) plus enforcement that the agent uses them. | [github.com/obra/superpowers](https://github.com/obra/superpowers) | `OSS` `Skill` |
| ECC (Everything Claude Code) | Agent-harness optimization system by Affaan Mustafa bundling 68 agents, 286 skills, 94 commands, hooks, rules, security scanning, and persistent memory to enforce a plan → test → implement → review → verify → remember loop. Works across Claude Code, Codex, Cursor, OpenCode, Gemini, and Kimi Code. | [github.com/affaan-m/ECC](https://github.com/affaan-m/ECC) | `OSS` `Skill` |
| gstack | Open-source Claude Code skill pack (~23+ slash commands) turning Claude Code into an AI engineering team — CEO, designer, eng manager, QA, security; `/office-hours` gives YC-style planning. | [github.com/garrytan/gstack](https://github.com/garrytan/gstack) | `OSS` `Skill` |
| GSD (Get Shit Done) | Lightweight meta-prompting / spec-driven dev system (slash commands + sub-agents + hooks) that fights context rot by working in fresh, verified units. | [github.com/gsd-build/get-shit-done](https://github.com/gsd-build/get-shit-done) | `OSS` `Skill` |
| OpenSpec | Tool-agnostic spec-driven development framework — keeps proposals, specs, and tasks in-repo as the source of truth before code. Works with 20+ tools. | [github.com/Fission-AI/OpenSpec](https://github.com/Fission-AI/OpenSpec) | `OSS` `Skill` |
| Ralph | The "Ralph Wiggum" technique by Geoffrey Huntley: re-feed an agent the same prompt in a fresh context until it signals done. Used for overnight refactors. | [ghuntley.com/ralph](https://ghuntley.com/ralph/) | `OSS` |
| claude-mem | Persistent memory plugin — captures session activity, compresses it with AI, and injects relevant context into future sessions. | [github.com/thedotmack/claude-mem](https://github.com/thedotmack/claude-mem) | `OSS` `Skill` |
| context-engineering-kit | Skill kit for managing an agent's context window — structuring prompts, curating what enters context, and improving result quality across long sessions. | [github.com/NeoLabHQ/context-engineering-kit](https://github.com/NeoLabHQ/context-engineering-kit) | `OSS` `Skill` |
| Caveman | Skill that compresses AI agent output ~65–75% by stripping filler, articles, and pleasantries while preserving code, paths, URLs, and technical terms (`/caveman`, lite/full/ultra modes). | [github.com/JuliusBrussee/caveman](https://github.com/JuliusBrussee/caveman) | `OSS` `Skill` `Free` |
| Ponytail | Skill/plugin that makes coding agents "think like the laziest senior dev" — a decision ladder (skip → reuse → stdlib → native → one-liner → minimal code) that cuts generated code volume (~54% fewer LOC per its benchmarks) while keeping safety guardrails. | [github.com/DietrichGebert/ponytail](https://github.com/DietrichGebert/ponytail) | `OSS` `Skill` |
| Codex Plugin | OpenAI's official plugin to use Codex from inside Claude Code — delegate tasks or get adversarial/standard code reviews. | [github.com/openai/codex-plugin-cc](https://github.com/openai/codex-plugin-cc) | `OSS` `Skill` |
| grill-me-codex | Plan-verification skill: "grills" you to lock a plan, then hands it to Codex which adversarially tears it apart over rounds until both sign off. | [github.com/chaseai-yt/grill-me-codex](https://github.com/chaseai-yt/grill-me-codex) | `OSS` `Skill` |
| Herdr | Terminal-native "agent multiplexer" (Rust, single ~10MB binary) — think tmux rebuilt for AI coding agents; gives each agent (Claude Code, Codex, Copilot CLI, Cursor Agent, 15+ others) a real terminal pane with automatic idle/working/blocked/done state detection. | [github.com/ogulcancelik/herdr](https://github.com/ogulcancelik/herdr) | `OSS` |
| pixel-agents | VS Code / JetBrains extension that visualizes AI coding agents as animated pixel-art characters by watching Claude Code's JSONL transcripts. | [github.com/pablodelucca/pixel-agents](https://github.com/pablodelucca/pixel-agents) | `OSS` `Skill` |

## Skill & MCP Tooling

Creating, optimizing, discovering, and packaging agent skills and MCP servers.

| Tool | What it does | Link | Tags |
|------|--------------|------|------|
| Agent Skills | Anthropic's open format for extending agents: a folder with `SKILL.md` (metadata + instructions, optional scripts) that Claude loads automatically when relevant. | [github.com/anthropics/skills](https://github.com/anthropics/skills) | `OSS` |
| skill-creator | Anthropic's official skill that guides you through building new Claude skills — use-case definition, frontmatter generation, packaging, and validation. | [github.com/anthropics/skills](https://github.com/anthropics/skills/tree/main/skill-creator) | `OSS` `Skill` |
| mcp-builder | Anthropic's official skill for building MCP servers that expose external APIs to LLMs — a four-phase workflow covering tool design, implementation in Python/FastMCP or the TypeScript SDK, testing with MCP Inspector, and writing evaluations. | [github.com/anthropics/skills](https://github.com/anthropics/skills/tree/main/skills/mcp-builder) | `OSS` `Skill` |
| SkillOpt | Microsoft's text-space optimizer that "trains" a natural-language `SKILL.md` for a frozen LLM agent — rollouts, scoring, reflection, bounded add/delete/replace edits, and a validation gate produce a deployable best skill. Reports roughly +23 to +25 accuracy points over no skill; backends include the Claude Code CLI. | [github.com/microsoft/SkillOpt](https://github.com/microsoft/SkillOpt) | `OSS` |
| find-skill | Skill/CLI that discovers and installs skills from many community and official sources into Claude Code, Codex, OpenCode, or Cursor, with automatic format conversion. | [github.com/fockus/claude-skill-find-skill](https://github.com/fockus/claude-skill-find-skill) | `OSS` `Skill` |

## Security & Offensive Testing

Autonomous pentesting, bug hunting, and reverse engineering.

| Tool | What it does | Link | Tags |
|------|--------------|------|------|
| Strix | Open-source autonomous AI penetration-testing agents that run your app, find vulnerabilities (XSS, auth bypass…), validate them with proof-of-concept exploits, and can auto-generate fix PRs; integrates with CI/CD, GitHub/GitLab, Slack/Jira. | [github.com/usestrix/strix](https://github.com/usestrix/strix) | `OSS` |
| Claude-BugHunter | Claude Code skill bundle turning the agent into an offensive-security researcher — 82 skills organized by attack surface, 15 slash commands, and 681 vulnerability patterns mined from disclosed HackerOne reports across 24 vulnerability classes, plus enterprise attack matrices for M365/Entra, Okta, and vCenter. Integrates Burp Suite MCP and ProjectDiscovery tooling; scoped to external attack surface. | [github.com/elementalsouls/Claude-BugHunter](https://github.com/elementalsouls/Claude-BugHunter) | `OSS` `Skill` |

## Video & Audio

Video production, editing, understanding, downloading, and voice.

| Tool | What it does | Link | Tags |
|------|--------------|------|------|
| OpenMontage | Open-source agentic video production system that runs inside a coding agent — 12 pipelines (explainers, talking heads, screen demos, trailers, animation, podcasts, localization, documentary montages), 100+ tools, and 700+ production-knowledge files taking a described video through research, script, assets, editing, and render. AGPL-3.0. | [github.com/calesthio/OpenMontage](https://github.com/calesthio/OpenMontage) | `OSS` `Skill` |
| MoneyPrinterTurbo | Generates HD short-form videos (9:16 or 16:9) from a single topic by chaining an LLM script writer, Pexels/Pixabay stock footage, TTS voiceover, subtitles, and background music via MoviePy/FFmpeg; offers a Streamlit web UI, REST API, CLI, and an agent mode. | [github.com/harry0703/MoneyPrinterTurbo](https://github.com/harry0703/MoneyPrinterTurbo) | `OSS` `Free` |
| /brag | Skill that turns a project you just built into a short shareable launch video with one command — generates a composition brief, motion graphics, music, share copy, and a rendered MP4, with a controllable tone flag and optional Kokoro voiceover. Needs Node 22+, FFmpeg, and the Hyperframes CLI. | [github.com/latent-spaces/brag](https://github.com/latent-spaces/brag) | `OSS` `Skill` |
| video-shotcraft | AI video skill for Claude Code and Codex that builds cinematic product and promo videos with Remotion — 150+ shot recipe cards with timing and pitfalls, 200+ motion previews, and a pipeline covering visual direction, storyboarding, sound design, beat sync, and QA. | [github.com/Vincentwei1021/video-shotcraft](https://github.com/Vincentwei1021/video-shotcraft) | `OSS` `Skill` |
| Remotion Skill | Agent skill teaching AI coding agents to write correct Remotion code — Remotion being the open-source React framework for making videos programmatically (React components → MP4/WebM/GIF). | [remotion.dev/docs/ai/skills](https://www.remotion.dev/docs/ai/skills) | `OSS` `Skill` |
| claude-video | Gives Claude the ability to watch any video — `/watch <URL or file>` downloads with yt-dlp, extracts frames with ffmpeg, pulls captions (falling back to Whisper), and hands frames plus transcript to the model. Installs as a Claude Code plugin. | [github.com/bradautomates/claude-video](https://github.com/bradautomates/claude-video) | `OSS` `Skill` |
| manim_skill | Agent skill packaging best practices and patterns for Manim (both Community Edition and ManimGL) so agents produce 3Blue1Brown-style mathematical animations. | [github.com/adithya-s-k/manim_skill](https://github.com/adithya-s-k/manim_skill) | `OSS` `Skill` |
| Higgsfield + Seedance 2.0 | Higgsfield is an AI video/image platform aggregating many models; Seedance 2.0 is ByteDance's multimodal video model (multi-shot, synced audio, lip-sync). | [higgsfield.ai](https://higgsfield.ai/) | `SaaS` |
| yt-dlp | Feature-rich command-line audio/video downloader and youtube-dl successor, supporting 1,000+ sites with format selection, subtitles, and post-processing. The backbone of most agent video pipelines. | [github.com/yt-dlp/yt-dlp](https://github.com/yt-dlp/yt-dlp) | `OSS` `Free` |
| Youwee | Cross-platform desktop GUI for yt-dlp (Tauri + React) covering YouTube, TikTok, Instagram and 1800+ sites, with AI video summaries (Gemini/OpenAI/Ollama), natural-language editing (cut, convert, resize), batch playlists, and subtitles. | [github.com/vanloctech/youwee](https://github.com/vanloctech/youwee) | `OSS` `Free` |
| OpenVoice | MIT/MyShell instant voice-cloning model — clones tone color from a short reference clip with zero-shot cross-lingual transfer and control over emotion, accent, and rhythm; V2 covers English, Spanish, French, Chinese, Japanese, and Korean. | [github.com/myshell-ai/OpenVoice](https://github.com/myshell-ai/OpenVoice) | `OSS` `Free` |
| Deep-Live-Cam | Real-time webcam face swap and one-click video deepfake from a single reference image, built on insightface/inswapper with mouth-mask and multi-face support. One of GitHub's most-starred AI repos; AGPL-3.0. Consent and likeness laws apply. | [github.com/hacksider/Deep-Live-Cam](https://github.com/hacksider/Deep-Live-Cam) | `OSS` |

## Creative & Media Generation

Image, 3D, animation, motion capture, and visual generation.

| Tool | What it does | Link | Tags |
|------|--------------|------|------|
| Weavy (Figma Weave) | Node-based browser creative platform chaining many AI models (Kling, Runway, Luma, OpenAI…) into reusable pipelines for image/video/3D. Acquired by Figma. | [weavy.ai](https://www.weavy.ai/) | `SaaS` |
| Open-Generative-AI | Self-hosted, MIT-licensed AI generation studio for image, video, lip-sync, and audio, wrapping 400+ models (Flux, SDXL, Kling, Sora, Veo…) behind a Next.js app with Electron desktop builds and Docker. Circulated earlier as "Open-Higgsfield-AI"; a Muapi.ai gateway key is still required. | [github.com/Anil-matcha/Open-Generative-AI](https://github.com/Anil-matcha/Open-Generative-AI) | `OSS` |
| FreeMoCap | Free, open-source markerless motion capture using ordinary webcams/phones + CV pose estimation to produce research-grade 3D motion data, processed locally. | [github.com/freemocap/freemocap](https://github.com/freemocap/freemocap) | `OSS` `Free` |
| Napkin AI | Turns text into business visuals — auto-generates infographics, diagrams, flowcharts, and mind maps; exports to PPT/PNG/SVG/PDF. | [napkin.ai](https://www.napkin.ai/) | `SaaS` |
| Illustrae | AI scientific-illustration platform with an infinite canvas; generates/edits detailed scientific figures from text, sketches, or photos. | [illustrae.co](https://illustrae.co/) | `SaaS` |
| SAM 3D | Meta's generative model reconstructing full 3D objects (shape, texture, layout) from a single 2D image, including occluded objects. Companion to SAM 3. | [ai.meta.com/blog/segment-anything-model-3](https://ai.meta.com/blog/segment-anything-model-3/) | `OSS` |
| Hunyuan3D-2.1 | Tencent's open-source image-to-3D system generating high-fidelity meshes with production-ready PBR textures; ships model weights, VAE encoder, PBR texture model, and full training/inference code with a diffusers-style API. | [github.com/Tencent-Hunyuan/Hunyuan3D-2.1](https://github.com/Tencent-Hunyuan/Hunyuan3D-2.1) | `OSS` |
| img2threejs | Agent skill that rebuilds the object in a single reference image as a code-only, procedural, animation-ready Three.js model (TypeScript factory plus JSON spec, no mesh files) through a staged, quality-gated pipeline with deterministic Python validation. | [github.com/img2threejs/img2threejs](https://github.com/img2threejs/img2threejs) | `OSS` `Skill` |
| SLAM3R | CVPR 2025 Highlight system for real-time dense 3D scene reconstruction from monocular RGB video — feed-forward networks regress per-clip pointmaps and register them globally at 20+ FPS with no explicit camera-parameter estimation. | [github.com/PKU-VCL-3DV/SLAM3R](https://github.com/PKU-VCL-3DV/SLAM3R) | `OSS` |
| AI4Animation | Research framework for data-driven neural character animation (locomotion, scene interaction, sports). Unity-based; `ai4animationpy` is the Python port. | [github.com/sebastianstarke/AI4Animation](https://github.com/sebastianstarke/AI4Animation) | `OSS` |
| Manus | General-purpose autonomous AI agent; its slides module researches, structures, and designs a full PowerPoint deck from a prompt (.pptx/PDF/web). | [manus.im](https://manus.im/) | `SaaS` |
| LingBot-Map | Feed-forward 3D foundation model for real-time streaming scene reconstruction from a single RGB camera (~20 FPS, no LiDAR/depth). | [github.com/robbyant/lingbot-map](https://github.com/robbyant/lingbot-map) | `OSS` |

## CAD & Engineering

Text/image-to-CAD and engineering copilots.

| Tool | What it does | Link | Tags |
|------|--------------|------|------|
| CadXStudio | Free browser-based AI CAD + CAM platform; turns plain-language prompts into parametric 3D models, generates G-code, with Git-style versioning. | [cadxstudio.in](https://cadxstudio.in/) | `Free` |
| Adam (adam.new) | AI CAD copilot generating parametric 3D models from text/images in seconds; exports STEP/STL/OBJ. (YC W25; see CADAM for its OSS component.) | [adam.new](https://adam.new/) | `SaaS` |
| MecAgent | AI CAD copilot integrating with SolidWorks, CATIA, Inventor, Fusion 360, Creo — generates parts from text, runs standards checks, estimates cost. | [mecagent.com](https://mecagent.com/) | `SaaS` |
| CADAM | Open-source text-to-CAD web app behind Adam — natural language/images → parametric models via OpenSCAD, in-browser via WebAssembly; exports STL/SCAD/DXF. | [github.com/Adam-CAD/CADAM](https://github.com/Adam-CAD/CADAM) | `OSS` |
| McMaster-Carr | Large US industrial-hardware supplier (595,000+ products) with a renowned website; relevant to CAD because it offers downloadable feature-rich 3D/2D CAD models (STEP, SLDPRT, Parasolid…) for 700,000+ parts, plus a SolidWorks add-in. | [mcmaster.com](https://www.mcmaster.com/) | `SaaS` `Free` |
| SimScale | Cloud-native computer-aided engineering (CAE) platform for running CFD, FEA, thermal, and electromagnetics simulations entirely in the browser — no local hardware or install; now positioned as an AI-native/agentic simulation platform. | [simscale.com](https://www.simscale.com/) | `SaaS` |
| OpenRocket | Free, open-source model-rocketry design tool with full six-degrees-of-freedom aerodynamics and trajectory simulation; design and fly rockets virtually before building. Java, GPL. | [github.com/openrocket/openrocket](https://github.com/openrocket/openrocket) | `OSS` `Free` |
| ParaView | Open-source, multi-platform scientific data-analysis and visualization application built on VTK (developed by Kitware with Sandia/Los Alamos); handles large-scale datasets. BSD 3-clause. | [paraview.org](https://www.paraview.org/) | `OSS` `Free` |
| OpenFOAM | Free, open-source C++ toolbox for computational fluid dynamics (CFD) — solvers and pre-/post-processing for fluid flow, turbulence, heat transfer, reactions, acoustics, and more. GPLv3 (ESI and Foundation distributions). | [openfoam.com](https://www.openfoam.com/) | `OSS` `Free` |
| NASA GMAT | NASA's open-source, multi-mission software for spacecraft mission design, trajectory optimization, and navigation — from low Earth orbit to lunar, libration-point, and deep-space missions. NASA Open Source Agreement. | [github.com/nasa/GMAT](https://github.com/nasa/GMAT) | `OSS` `Free` |
| NASA CEA | NASA Glenn program that computes chemical-equilibrium compositions and thermodynamic/transport properties via free-energy minimization — used for theoretical rocket performance (c*, Isp), detonations, and shock analysis, over a 2000+ species database. | [github.com/nasa/cea](https://github.com/nasa/cea) | `OSS` `Free` |
| F´ (F Prime) | NASA JPL's open-source, component-driven flight-software and embedded-systems framework (C++) for spaceflight — flies on the Mars Ingenuity helicopter, CADRE lunar rovers, and Europa Clipper. | [github.com/nasa/fprime](https://github.com/nasa/fprime) | `OSS` `Free` |

## Business, Marketing & Career

Pitching, marketing, SEO, product management, and job-search tooling.

| Tool | What it does | Link | Tags |
|------|--------------|------|------|
| Career-Ops | Job-search system on Claude Code — scans career portals, reasons about job fit vs your CV, and generates per-listing ATS-optimized resume PDFs. | [github.com/santifer/career-ops](https://github.com/santifer/career-ops) | `OSS` `Skill` |
| marketing-skills | Collection of marketing skills for Claude Code/AI agents — CRO, copywriting, SEO, analytics, growth engineering. | [github.com/coreyhaines31/marketingskills](https://github.com/coreyhaines31/marketingskills) | `OSS` `Skill` |
| claude-seo | Universal SEO skill pack for Claude Code — 25 sub-skills and 18 sub-agents running in parallel across technical SEO, E-E-A-T content quality, Schema.org, generative-engine optimization, backlinks, local SEO, semantic clustering, and international SEO, with PDF/Excel reporting. | [github.com/AgriciDaniel/claude-seo](https://github.com/AgriciDaniel/claude-seo) | `OSS` `Skill` |
| OpenSEO | MIT-licensed open-source alternative to Semrush and Ahrefs — keyword research, rank tracking, backlinks, site audits, and AI-visibility tracking behind a web UI, plus an MCP server and agent skills shipped as Claude Code and Codex plugins. Data comes from DataForSEO with your own key when self-hosted. | [github.com/every-app/open-seo](https://github.com/every-app/open-seo) | `OSS` `Skill` |
| pm-skills | 100+ Claude Code skills/commands for product managers across the full lifecycle — discovery, strategy, PRDs/OKRs/roadmaps, market research, analytics (SQL, cohorts, A/B), and go-to-market. | [github.com/phuryn/pm-skills](https://github.com/phuryn/pm-skills) | `OSS` `Skill` |
| PitchUs | AI tool that converts a founder's pitch deck into a US VC-ready format — restructuring and optimizing the deck to match American investor expectations. | [pitchusai.com](https://www.pitchusai.com/) | `SaaS` |
| competitive-ads-extractor | Skill that extracts and analyzes competitors' ads from ad libraries (Meta Ad Library, Google Ads Transparency, LinkedIn) — screenshots, messaging/value-prop analysis, theme categorization, and pattern detection. | [github.com/ComposioHQ/awesome-claude-skills](https://github.com/ComposioHQ/awesome-claude-skills/tree/master/competitive-ads-extractor) | `OSS` `Skill` |
| ads-meta | Claude skill (part of the claude-ads pack) running a ~50-point audit of Facebook/Instagram ad accounts — Pixel/CAPI setup, creative fatigue, account structure, audience targeting — with a weighted scored report. | [github.com/AgriciDaniel/claude-ads](https://github.com/AgriciDaniel/claude-ads) | `OSS` `Skill` |
| OpenReply | Self-hosted open-source ManyChat alternative for Instagram — keyword triggers on comments fire automatic DMs and public replies, with story-reply triggers, tracked redirect links with click analytics, follow-gate verification, multi-account workspaces, a DM inbox, and per-account rate limiting. Next.js and Prisma/Postgres with BullMQ workers on the official Meta API. | [github.com/diwenne/openreply](https://github.com/diwenne/openreply) | `OSS` |
| Sandcastles.ai | AI YouTube research/ideation tool — surfaces outlier and viral videos, analyzes trends, and generates data-backed scripts and hooks for creators. | [sandcastles.ai](https://www.sandcastles.ai/) | `SaaS` |
| Meetily | Privacy-first, self-hosted AI meeting note-taker (macOS/Windows) — live Whisper/Parakeet transcription, speaker diarization, and local LLM summarization via Ollama; 100% local, no cloud. | [github.com/Zackriya-Solutions/meetily](https://github.com/Zackriya-Solutions/meetily) | `OSS` `Free` |

## Finance & Trading

Quant research, portfolio construction, backtesting, and trading agents.

| Tool | What it does | Link | Tags |
|------|--------------|------|------|
| Vibe-Trading | HKUDS's "personal trading agent" — an agent skill for Claude Code/Codex/ChatGPT for AI quantitative trading across crypto, stocks, and forex: market research, strategy generation, backtesting with validation artifacts, live trading, and multi-agent research swarms. | [github.com/HKUDS/Vibe-Trading](https://github.com/HKUDS/Vibe-Trading) | `OSS` `Skill` |
| OpenAlice | Local trading workspace for coding agents (Claude Code, Codex, opencode) covering equities, crypto, commodities, forex, and macro from research through entry, management, and exit — Markdown issue boards, a tracked entity graph of tickers and theses, and a "trading as git" staged, approval-gated broker workflow. Research mode needs no broker; execution is beta. | [github.com/TraderAlice/OpenAlice](https://github.com/TraderAlice/OpenAlice) | `OSS` |
| ai-berkshire | Value-investing research framework of ~19 Claude Code/Codex skills systematizing the methodologies of Buffett, Munger, Duan Yongping, and Li Lu; `/investment-team` spawns 4 parallel analyst agents plus a synthesizing team lead. | [github.com/xbtlin/ai-berkshire](https://github.com/xbtlin/ai-berkshire) | `OSS` `Skill` |
| NautilusTrader | High-performance, production-grade algorithmic trading platform and event-driven backtester — Rust core exposed to Python, nanosecond-resolution backtesting across multiple venues, and identical strategy code from backtest to live deployment. | [github.com/nautechsystems/nautilus_trader](https://github.com/nautechsystems/nautilus_trader) | `OSS` |
| GS Quant | Goldman Sachs' open-source Python toolkit for quantitative finance — derivatives pricing and risk through the GS Marquee developer APIs, plus standalone packages for timeseries analytics, backtesting, and portfolio risk. Apache-2.0; GS pricing endpoints need an account. | [github.com/goldmansachs/gs-quant](https://github.com/goldmansachs/gs-quant) | `OSS` |
| skfolio | Python portfolio-optimization and risk-management library built on scikit-learn's fit/predict/transform API — mean-variance through clustering-based allocation (HRP and friends), financial estimators, and time-series-aware cross-validation for backtesting and stress testing. BSD-3. | [github.com/skfolio/skfolio](https://github.com/skfolio/skfolio) | `OSS` `Free` |
| Kronos | First open-source decoder-only foundation model for financial K-line (OHLCV candlestick) time series, pre-trained across 45+ global exchanges — a tokenizer quantizes candlestick data into hierarchical discrete tokens that an autoregressive model then forecasts. AAAI 2026; weights and fine-tuning scripts released. | [github.com/shiyu-coder/Kronos](https://github.com/shiyu-coder/Kronos) | `OSS` |
| ir-search | Korean government grant and support-program survey skill — crawls K-Startup, 기업마당, NIPA, KOCCA, and SMTECH, then sorts programs into immediately eligible, conditional, and reframe-to-qualify buckets against a startup profile. Ships manifests for Claude Code, Codex, Cursor, and Gemini CLI. | [github.com/djfksjd/ir-search](https://github.com/djfksjd/ir-search) | `OSS` `Skill` |

## Web Scraping & Browser Automation

Turning the web into data and driving browsers programmatically.

| Tool | What it does | Link | Tags |
|------|--------------|------|------|
| Firecrawl | API/toolkit for scraping, crawling, and searching the web — turns sites into LLM-ready clean markdown / structured data. | [github.com/firecrawl/firecrawl](https://github.com/firecrawl/firecrawl) | `OSS` |
| Playwright | Microsoft's cross-browser automation library for end-to-end testing and programmatic browser control. | [playwright.dev](https://playwright.dev) | `OSS` |
| Perplexity (ppl-ai) | AI answer engine / conversational search. `ppl-ai` is Perplexity's GitHub org; public OSS (pplx-garden, pplx-kernels) lives under `perplexityai`. | [perplexity.ai](https://www.perplexity.ai/) | `SaaS` |
| Scrapling | High-performance, adaptive Python web-scraping library with built-in stealth/anti-bot bypassing (e.g. Cloudflare Turnstile), adaptive element tracking that survives site-structure changes, three fetching strategies, and a spider framework. | [github.com/D4Vinci/Scrapling](https://github.com/D4Vinci/Scrapling) | `OSS` |
| Agent-Reach | Gives agents "eyes on the internet" — a single install doc wires up unified search, read, and interact across 13–16 platforms (X, Reddit, YouTube transcripts, GitHub, LinkedIn, Instagram, Bilibili, XiaoHongShu, Weibo, V2EX, RSS, arbitrary URLs) using no-API-key scrapers. Works as an agent skill in Claude Code, Cursor, and Windsurf. | [github.com/Panniantong/agent-reach](https://github.com/Panniantong/agent-reach) | `OSS` `Skill` |
| PageAgent | Alibaba's in-page GUI agent: a JavaScript library you embed with `npm install page-agent` that lets users drive a web app's own UI in natural language, using DOM analysis rather than screenshots, vision models, extensions, or a headless browser. MIT. | [github.com/alibaba/page-agent](https://github.com/alibaba/page-agent) | `OSS` |

## UI / Web Design

Design-intelligence skills and resources for building better interfaces.

| Tool | What it does | Link | Tags |
|------|--------------|------|------|
| Emil Kowalski (skills) | Design engineer (Linear, ex-Vercel); creator of animations.dev, Sonner, and Vaul. His MIT skills collection holds 12 agent skills for designers and engineers, including "Emil Design Eng" for his animation philosophy and `apple-design`, which distills Apple's WWDC fluid-interface talks into web technique — response latency, direct manipulation, interruptibility, and velocity inheritance. | [github.com/emilkowalski/skills](https://github.com/emilkowalski/skills) | `OSS` `Skill` |
| impeccable | Design-language skill (1 skill, 23 commands — polish, audit, critique, animate…) that makes AI coding harnesses better at frontend design. | [github.com/pbakaus/impeccable](https://github.com/pbakaus/impeccable) | `OSS` `Skill` |
| taste-skill | Design skill giving the agent "good taste" — DESIGN.md files that ban AI-slop patterns and enforce real typography, asymmetric layouts, tuned motion. | [github.com/Leonxlnx/taste-skill](https://github.com/Leonxlnx/taste-skill) | `OSS` `Skill` |
| UI/UX Pro Max | Design-intelligence skill: searchable database of styles, palettes, font pairings, UX guidelines, and charts across stacks, with a CLI to generate design systems. | [github.com/nextlevelbuilder/ui-ux-pro-max-skill](https://github.com/nextlevelbuilder/ui-ux-pro-max-skill) | `OSS` `Skill` |
| huashu-design | HTML-native design skill (inspired by Claude Design) — turns a sentence into high-fidelity prototypes, decks, animations, infographics; MP4/PPTX export. | [github.com/alchaincyf/huashu-design](https://github.com/alchaincyf/huashu-design) | `OSS` `Skill` |
| SkillUI | CLI (`npx skillui`) that crawls any website, git repo, or local codebase and extracts its full design system — colors, typography, spacing, animations, components, screenshots — packaging it as a SKILL.md folder and `.skill` archive so Claude Code builds UI in that design language. | [github.com/amaancoderx/npxskillui](https://github.com/amaancoderx/npxskillui) | `OSS` `Skill` |
| frontend-slides | Claude Code skill that builds animation-rich single-file HTML presentations with inline CSS/JS and zero dependencies, either from scratch or by converting PPTX, using visual previews and curated style presets to avoid generic AI aesthetics. | [github.com/zarazhangrui/frontend-slides](https://github.com/zarazhangrui/frontend-slides) | `OSS` `Skill` |
| framer-motion-skill | Claude Code skill for Motion (the React/JS animation library formerly called Framer Motion) — declarative motion components, spring physics, gestures, layout animations, and scroll effects. The underlying library lives at motion.dev. | [github.com/Schoepplake/framer-motion-skill](https://github.com/Schoepplake/framer-motion-skill) | `OSS` `Skill` |
| screenshot-to-code | Converts screenshots, mockups, Figma designs, and screen recordings into HTML/Tailwind, React, or Vue code using vision models from OpenAI, Anthropic, and Google. React/Vite frontend with a FastAPI backend; hosted version available. | [github.com/abi/screenshot-to-code](https://github.com/abi/screenshot-to-code) | `OSS` |
| ai-website-cloner-template | GitHub template that clones any website with one `/clone-website` command — screenshots the target via a browser extension, extracts design tokens/components, dispatches parallel builder agents, and reconstructs it in Next.js/React/Tailwind with diff-fixing against the original. | [github.com/JCodesMore/ai-website-cloner-template](https://github.com/JCodesMore/ai-website-cloner-template) | `OSS` `Skill` |
| Scroll World | Agent skill (SKILL.md for Claude Code/Codex) that turns a brand into a scrollable Apple-style 3D-world landing page — one continuous camera flight through generated isometric diorama scenes (Higgsfield + Seedance/Kling image-to-video) scrubbed by scroll position. | [github.com/oso95/scroll-world](https://github.com/oso95/scroll-world) | `OSS` `Skill` |
| React Three Fiber | Poimandres' React renderer for Three.js — JSX elements map to Three.js objects (`<mesh />` becomes `new THREE.Mesh()`), so WebGL scenes are built declaratively from reusable, state-reactive components. Rendering happens outside React's DOM tree, so there is no per-frame React overhead and new Three.js features work without library updates. MIT; the de-facto standard for 3D in React, with a drei/postprocessing/rapier ecosystem. | [github.com/pmndrs/react-three-fiber](https://github.com/pmndrs/react-three-fiber) | `OSS` `Free` |
| ShaderGradient | Customizable animated 3D gradient renderer — a WebGL mesh whose shaders are driven by editable color, shape, motion, lighting, and grain parameters to produce looping gradient backgrounds. Ships `@shadergradient/react` as a lean renderer atop React Three Fiber, plus a hosted editor, a Figma plugin, and a Framer component that export stills, GIF, or video. MIT. | [github.com/ruucm/shadergradient](https://github.com/ruucm/shadergradient) | `OSS` `Free` |
| liquid-glass-js | Vanilla-JS WebGL 2.0 shader library rendering Apple-style Liquid Glass surfaces — rounded-rect, circle, and pill elements with real-time refraction, blur, masking, and nested glass where children sample the parent's output; samples the page behind via html2canvas. MIT, script-tag install, no npm package. The name is crowded: `rdev/liquid-glass-react` is a far more widely used React component doing the same effect through SVG displacement maps. ⚠️ | [github.com/dashersw/liquid-glass-js](https://github.com/dashersw/liquid-glass-js) | `OSS` `Free` `⚠️` |
| liquid-logo | Paper Design web app that turns an uploaded logo (high-contrast or transparent PNG) into animated liquid metal, using the image as a mask and displacement input to a WebGL fragment shader with adjustable refraction, edge, pattern, and speed. Source-available under PolyForm Shield 1.0.0, not an OSI license; the underlying `@paper-design/shaders-react` library is separate and Apache-2.0. | [github.com/paper-design/liquid-logo](https://github.com/paper-design/liquid-logo) | `Free` |

## Writing, Learning & Communication

Making AI prose sound human, and making hard things explainable.

| Tool | What it does | Link | Tags |
|------|--------------|------|------|
| humanizer | Skill that removes signs of AI-generated writing (em-dash overuse, rule of three, AI vocabulary, etc.) based on Wikipedia's "Signs of AI writing" guide. | [github.com/blader/humanizer](https://github.com/blader/humanizer) | `OSS` `Skill` |
| im-not-ai | Korean-language counterpart to humanizer — a Claude Code plugin (3 skills, 9 sub-agents) that detects translationese, mechanical parallelism, and 71 other "AI tells" and rewrites Korean text to read as human prose. Also supports Copilot, Codex, and Gemini CLI. | [github.com/epoko77-ai/im-not-ai](https://github.com/epoko77-ai/im-not-ai) | `OSS` `Skill` |
| ELI5 | Claude Code skill that adapts an explanation to its audience — detects the target from the prompt (ages 5 through 40+, job roles, family relationships) and calibrates vocabulary, analogies, tone, and depth, from toys for a five-year-old to business outcomes for a manager. Ships a Python evaluation framework. | [github.com/DreambigOu/ELI5](https://github.com/DreambigOu/ELI5) | `OSS` `Skill` |
| PenEcho | Open-source infinite spatial canvas for thinking with AI — handwrite equations, diagrams, or notes anywhere and the model reads the marks and their spatial relationships, answering beside them. Includes an agent mode over local files and web research; works offline with OpenAI-compatible, Anthropic, or Codex CLI backends. | [github.com/penecho/penecho](https://github.com/penecho/penecho) | `OSS` |

## Datasets

| Tool | What it does | Link | Tags |
|------|--------------|------|------|
| The Well | 15TB collection of 16 physics-simulation datasets (fluid dynamics, MHD, acoustics, supernovae…) with a unified PyTorch interface for ML surrogate models. | [github.com/PolymathicAI/the_well](https://github.com/PolymathicAI/the_well) | `OSS` |

## Open Models

Open-weight models you can download, fine-tune, and run yourself — LLMs, vision models, and beyond. (Domain-specific models with one clear use case, like SAM 3D or Kronos, stay in their domain section.)

| Tool | What it does | Link | Tags |
|------|--------------|------|------|
| NVIDIA Nemotron 3 | NVIDIA's open-weight MoE model family for agentic reasoning — Nano (30B/3B active), Super (~120B/12.7B active, 1M-token context), Ultra (550B/55B active); weights on Hugging Face under the NVIDIA Open Model License (commercial use OK). Paired with OpenCode, forms a local coding-agent stack that rivals paid coding agents. | [developer.nvidia.com/nemotron](https://developer.nvidia.com/nemotron) | `OSS` |
| RF-DETR | Roboflow's real-time detection transformer (ICLR 2026) for object detection, instance segmentation, and keypoint detection on a DINOv2 backbone — SOTA on COCO/RF100-VL, designed for fine-tuning. Nano–Large weights and all code Apache-2.0; XL/2XL variants under Roboflow's PML license. | [github.com/roboflow/rf-detr](https://github.com/roboflow/rf-detr) | `OSS` |
| Code-as-World | Research system and model family (VL-4B and VL-9B, Apache-2.0) that turns video observations into executable code representations of physical state and dynamics through iterative simulation and verification with MuJoCo and SAM 3; ships local inference, vLLM serving, and the QuantiPhy benchmark. | [github.com/MirroS-Lab/Code-as-World](https://github.com/MirroS-Lab/Code-as-World) | `OSS` |

## System & Dev Utilities

Local machine, infrastructure, workflow automation, and analytics tools.

| Tool | What it does | Link | Tags |
|------|--------------|------|------|
| Mole | Free, open-source all-in-one macOS optimization toolkit — clean, uninstall, analyze, optimize, and monitor the Mac from the terminal. | [github.com/tw93/Mole](https://github.com/tw93/Mole) | `OSS` `Free` |
| docker-android | Docker image running Android emulators with noVNC and video recording — for Android app dev and native/web/hybrid testing (Appium, Espresso). | [github.com/budtmo/docker-android](https://github.com/budtmo/docker-android) | `OSS` |
| Clicky | Open-source macOS menu-bar AI teaching assistant — sees your screen, takes push-to-talk voice, and points its cursor at on-screen UI elements to guide you through tasks. Built on Claude + AssemblyAI + ElevenLabs. | [github.com/farzaa/clicky](https://github.com/farzaa/clicky) | `OSS` `Free` |
| n8n-skills | Fourteen complementary Claude Code skills for building n8n workflows — expression syntax, node config, validation, workflow patterns, Code node JS/Python, error handling, binary data, subworkflows, and self-hosting — plus a router skill and hooks enforcement layer, working through the author's n8n-mcp server. | [github.com/czlonkowski/n8n-skills](https://github.com/czlonkowski/n8n-skills) | `OSS` `Skill` |
| k-skill | Collection of 150+ agent skills for Korean everyday tasks — KTX/SRT and bus lookups, real-estate, auction and building-registry search, stock and corporate filings, Coupang/Kurly shopping, government permits, weather, and Korean spell-checking. Installs via npx; works with Claude Code, Codex, and OpenCode. | [github.com/NomaDamas/k-skill](https://github.com/NomaDamas/k-skill) | `OSS` `Skill` |
| Google Workspace (gws) | Google's cloud productivity suite (Gmail, Docs, Sheets, Drive, Calendar). Listed here for its MCP/Claude integrations that let agents read and write Workspace docs. | [workspace.google.com](https://workspace.google.com) | `SaaS` |
| Supervision | Roboflow's model-agnostic Python library of reusable computer-vision utilities — a unified Detections API with connectors for Ultralytics/Transformers/SAM, plus annotators, object tracking, zone counting, and dataset tools. | [github.com/roboflow/supervision](https://github.com/roboflow/supervision) | `OSS` |
| OmniRoute | Free, open-source (MIT, TypeScript) AI gateway/router exposing one OpenAI-compatible endpoint over 200+ LLM providers, with multi-tier auto-fallback, multiple routing strategies, token compression, and MCP support; connects Claude Code, Cursor, Cline. | [github.com/diegosouzapw/OmniRoute](https://github.com/diegosouzapw/OmniRoute) | `OSS` `Free` |

## Curated Lists

Meta-resources — lists worth mining for more tools.

| Tool | What it does | Link | Tags |
|------|--------------|------|------|
| awesome-opensource-ai | Curated list of battle-tested, production-proven, truly open-source AI projects, models, libraries, and dev tools. | [github.com/alvinreal/awesome-opensource-ai](https://github.com/alvinreal/awesome-opensource-ai) | `OSS` |
| awesome-claude-code | Curated list of skills, hooks, slash-commands, agent orchestrators, and plugins for Claude Code. (Generic name — several competing repos.) | [github.com/hesreallyhim/awesome-claude-code](https://github.com/hesreallyhim/awesome-claude-code) | `OSS` |
| awesome-systematic-trading | Curated list of 112 quant libraries (backtesting, live trading, analytics, data sources), 40+ strategies, and 55+ books for systematic trading; notable for citing replication research across 4,843 backtested strategies. An older list of the same name by wangzhe3224 emphasizes code quality. | [github.com/paperswithbacktest/awesome-systematic-trading](https://github.com/paperswithbacktest/awesome-systematic-trading) | `OSS` |
| awesome-design-md | Curated collection of 73+ DESIGN.md files extracted from major brand sites (Claude, Vercel, Airbnb, Tesla…). Drop one into a project so coding agents generate a matching UI. | [github.com/voltagent/awesome-design-md](https://github.com/voltagent/awesome-design-md) | `OSS` |
| claude-fable-5.md (system-prompt collections) | Community-extracted system prompts for Anthropic's Claude Fable 5, mirrored in system-prompt-collection repos (asgeirtj/system_prompts_leaks, elder-plinius/CL4R1T4S). A reference document, not a tool; unofficial. | [github.com/asgeirtj/system_prompts_leaks](https://github.com/asgeirtj/system_prompts_leaks) | `Free` |

---

## 🔄 How this catalog is maintained

This catalog updates via a Claude Code slash command — new finds are passed directly in the prompt.

1. **Run `/update-tools <new finds>`** in Claude Code from this directory — any format, partial names, Korean/English hints, and URLs are all fine (e.g. `/update-tools Cognee (기억 향상), RF-DETR, https://github.com/owner/repo`).
2. The command parses your input, checks this `README.md` for what's **not yet catalogued** (so it's safe to re-run), **web-researches** each new tool, classifies it into the scheme above, and inserts it into the right table. It then prints a summary of what changed.

The command definition lives in [`.claude/commands/update-tools.md`](.claude/commands/update-tools.md).
