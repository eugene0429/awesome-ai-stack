# awesome-ai-stack

A curated catalog of AI tools — open-source and commercial (SaaS) — plus Claude Code skills, collected from the wild, researched, and organized.

> New finds go into [`raw.txt`](raw.txt) in any format. Running the [`/update-tools`](#-how-this-catalog-is-maintained) command researches each new entry, classifies it, and appends it to the right section below. See [How this catalog is maintained](#-how-this-catalog-is-maintained).

**Legend** · `OSS` open source · `SaaS` commercial/hosted · `Skill` Claude Code skill or plugin · `Free` free to use

## Contents

- [Research & Academic](#research--academic)
- [RAG & Knowledge Management](#rag--knowledge-management)
- [LLM Optimization & Local Inference](#llm-optimization--local-inference)
- [Agent Frameworks & Multi-Agent Systems](#agent-frameworks--multi-agent-systems)
- [Claude Code Skills & Plugins](#claude-code-skills--plugins)
- [Creative & Media Generation](#creative--media-generation)
- [CAD & Engineering](#cad--engineering)
- [Business, Marketing & Career](#business-marketing--career)
- [Web Scraping & Browser Automation](#web-scraping--browser-automation)
- [UI / Web Design](#ui--web-design)
- [Datasets](#datasets)
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

## RAG & Knowledge Management

Frameworks that turn documents, code, or media into queryable knowledge.

| Tool | What it does | Link | Tags |
|------|--------------|------|------|
| RAG-Anything | All-in-one multimodal RAG framework retrieving across text, images, tables, and equations via dual-graph construction and cross-modal hybrid retrieval. | [github.com/HKUDS/RAG-Anything](https://github.com/HKUDS/RAG-Anything) | `OSS` |
| Understand-Anything | Multi-agent plugin that turns any codebase into an interactive, queryable knowledge graph with plain-English summaries and AI walkthroughs. | [github.com/Lum1104/Understand-Anything](https://github.com/Lum1104/Understand-Anything) | `OSS` `Skill` |
| Graphify | Skill that turns any folder of code/docs/papers/media into a queryable knowledge graph (Tree-sitter + NetworkX + Leiden), with Obsidian-compatible output. | [github.com/safishamsi/graphify](https://github.com/safishamsi/graphify) | `OSS` `Skill` |

## LLM Optimization & Local Inference

Run bigger models on smaller hardware; compression and efficient inference.

| Tool | What it does | Link | Tags |
|------|--------------|------|------|
| bitnet.cpp | Microsoft's official inference framework for 1-bit (1.58-bit) LLMs, with optimized kernels that cut compute and energy dramatically. | [github.com/microsoft/BitNet](https://github.com/microsoft/BitNet) | `OSS` |
| ntransformer | Dependency-free C++/CUDA engine running Llama 3.1 70B on a single RTX 3090 via 3-tier adaptive caching (VRAM + RAM + NVMe). Trades speed for fit. | [github.com/xaskasdf/ntransformer](https://github.com/xaskasdf/ntransformer) | `OSS` |
| Turbovec | Rust vector index (Python bindings) implementing TurboQuant — training-free 2–4 bit vector compression with SIMD nearest-neighbor search for local RAG. | [github.com/RyanCodrai/turbovec](https://github.com/RyanCodrai/turbovec) | `OSS` |
| AirLLM | Layer-by-layer sharding so a 70B model runs on a single 4GB GPU (405B on 8GB) with no quantization/distillation. | [github.com/lyogavin/airllm](https://github.com/lyogavin/airllm) | `OSS` |

## Agent Frameworks & Multi-Agent Systems

Building, training, and orchestrating autonomous and swarm agents.

| Tool | What it does | Link | Tags |
|------|--------------|------|------|
| Agent Lightning | Microsoft framework adding RL, prompt optimization, and fine-tuning to any agent with near-zero code changes; works with LangChain, AutoGen, CrewAI, etc. | [github.com/microsoft/agent-lightning](https://github.com/microsoft/agent-lightning) | `OSS` |
| Hermes Agent | Open-source self-improving agent with a closed learning loop — writes reusable skill files, stores outcomes in memory, refines across sessions. | [github.com/NousResearch/hermes-agent](https://github.com/NousResearch/hermes-agent) | `OSS` |
| MetaGPT | Multi-agent framework simulating a software company — roles (PM, architect, engineer) follow SOPs to turn one line into PRDs, designs, and code. | [github.com/FoundationAgents/MetaGPT](https://github.com/FoundationAgents/MetaGPT) | `OSS` |
| MiroFish | Swarm-intelligence prediction engine spinning up thousands-to-millions of agents in parallel simulated social worlds to forecast outcomes (on CAMEL-AI OASIS). | [github.com/666ghj/MiroFish](https://github.com/666ghj/MiroFish) | `OSS` |
| ruflo | Multi-agent meta-harness for Claude Code/Codex — coordinating agent swarms with adaptive memory, self-learning, GOAP planning, RAG, and federated comms. | [github.com/ruvnet/ruflo](https://github.com/ruvnet/ruflo) | `OSS` `Skill` |

## Claude Code Skills & Plugins

Skills, plugins, and tooling that extend Claude Code (and other AI coding agents).

| Tool | What it does | Link | Tags |
|------|--------------|------|------|
| superpowers | Agentic skills framework and dev methodology — composable skills (brainstorming, TDD, debugging, verification) plus enforcement that the agent uses them. | [github.com/obra/superpowers](https://github.com/obra/superpowers) | `OSS` `Skill` |
| claude-mem | Persistent memory plugin — captures session activity, compresses it with AI, and injects relevant context into future sessions. | [github.com/thedotmack/claude-mem](https://github.com/thedotmack/claude-mem) | `OSS` `Skill` |
| Agent Skills | Anthropic's open format for extending agents: a folder with `SKILL.md` (metadata + instructions, optional scripts) that Claude loads automatically when relevant. | [github.com/anthropics/skills](https://github.com/anthropics/skills) | `OSS` |
| GSD (Get Shit Done) | Lightweight meta-prompting / spec-driven dev system (slash commands + sub-agents + hooks) that fights context rot by working in fresh, verified units. | [github.com/gsd-build/get-shit-done](https://github.com/gsd-build/get-shit-done) | `OSS` `Skill` |
| Ralph | The "Ralph Wiggum" technique by Geoffrey Huntley: re-feed an agent the same prompt in a fresh context until it signals done. Used for overnight refactors. | [ghuntley.com/ralph](https://ghuntley.com/ralph/) | `OSS` |
| pixel-agents | VS Code / JetBrains extension that visualizes AI coding agents as animated pixel-art characters by watching Claude Code's JSONL transcripts. | [github.com/pablodelucca/pixel-agents](https://github.com/pablodelucca/pixel-agents) | `OSS` `Skill` |
| autoresearch | Karpathy's project where agents autonomously run ~100 research experiments overnight on single-GPU nanochat training; you edit context files, not Python. | [github.com/karpathy/autoresearch](https://github.com/karpathy/autoresearch) | `OSS` |
| OpenSpec | Tool-agnostic spec-driven development framework — keeps proposals, specs, and tasks in-repo as the source of truth before code. Works with 20+ tools. | [github.com/Fission-AI/OpenSpec](https://github.com/Fission-AI/OpenSpec) | `OSS` `Skill` |
| claude-peers | MCP-based peer-discovery channel letting multiple running Claude Code instances find each other and message ad-hoc via a localhost broker. | [github.com/louislva/claude-peers-mcp](https://github.com/louislva/claude-peers-mcp) | `OSS` `Skill` |
| Codex Plugin | OpenAI's official plugin to use Codex from inside Claude Code — delegate tasks or get adversarial/standard code reviews. | [github.com/openai/codex-plugin-cc](https://github.com/openai/codex-plugin-cc) | `OSS` `Skill` |
| Claudian | Obsidian plugin embedding Claude Code/Codex as an AI collaborator inside your vault (read/write/search/bash with the vault as working dir). | [github.com/YishenTu/claudian](https://github.com/YishenTu/claudian) | `OSS` `Skill` |
| grill-me-codex | Plan-verification skill: "grills" you to lock a plan, then hands it to Codex which adversarially tears it apart over rounds until both sign off. | [github.com/chaseai-yt/grill-me-codex](https://github.com/chaseai-yt/grill-me-codex) | `OSS` `Skill` |
| humanizer | Skill that removes signs of AI-generated writing (em-dash overuse, rule of three, AI vocabulary, etc.) based on Wikipedia's "Signs of AI writing" guide. | [github.com/blader/humanizer](https://github.com/blader/humanizer) | `OSS` `Skill` |
| gstack | Open-source Claude Code skill pack (~23+ slash commands) turning Claude Code into an AI engineering team — CEO, designer, eng manager, QA, security; `/office-hours` gives YC-style planning. | [github.com/garrytan/gstack](https://github.com/garrytan/gstack) | `OSS` `Skill` |

## Creative & Media Generation

Image, video, 3D, animation, motion capture, and visual generation.

| Tool | What it does | Link | Tags |
|------|--------------|------|------|
| Weavy (Figma Weave) | Node-based browser creative platform chaining many AI models (Kling, Runway, Luma, OpenAI…) into reusable pipelines for image/video/3D. Acquired by Figma. | [weavy.ai](https://www.weavy.ai/) | `SaaS` |
| FreeMoCap | Free, open-source markerless motion capture using ordinary webcams/phones + CV pose estimation to produce research-grade 3D motion data, processed locally. | [github.com/freemocap/freemocap](https://github.com/freemocap/freemocap) | `OSS` `Free` |
| Napkin AI | Turns text into business visuals — auto-generates infographics, diagrams, flowcharts, and mind maps; exports to PPT/PNG/SVG/PDF. | [napkin.ai](https://www.napkin.ai/) | `SaaS` |
| Illustrae | AI scientific-illustration platform with an infinite canvas; generates/edits detailed scientific figures from text, sketches, or photos. | [illustrae.co](https://illustrae.co/) | `SaaS` |
| SAM 3D | Meta's generative model reconstructing full 3D objects (shape, texture, layout) from a single 2D image, including occluded objects. Companion to SAM 3. | [ai.meta.com/blog/segment-anything-model-3](https://ai.meta.com/blog/segment-anything-model-3/) | `OSS` |
| AI4Animation | Research framework for data-driven neural character animation (locomotion, scene interaction, sports). Unity-based; `ai4animationpy` is the Python port. | [github.com/sebastianstarke/AI4Animation](https://github.com/sebastianstarke/AI4Animation) | `OSS` |
| Manus | General-purpose autonomous AI agent; its slides module researches, structures, and designs a full PowerPoint deck from a prompt (.pptx/PDF/web). | [manus.im](https://manus.im/) | `SaaS` |
| Higgsfield + Seedance 2.0 | Higgsfield is an AI video/image platform aggregating many models; Seedance 2.0 is ByteDance's multimodal video model (multi-shot, synced audio, lip-sync). | [higgsfield.ai](https://higgsfield.ai/) | `SaaS` |
| LingBot-Map | Feed-forward 3D foundation model for real-time streaming scene reconstruction from a single RGB camera (~20 FPS, no LiDAR/depth). | [github.com/robbyant/lingbot-map](https://github.com/robbyant/lingbot-map) | `OSS` |

## CAD & Engineering

Text/image-to-CAD and engineering copilots.

| Tool | What it does | Link | Tags |
|------|--------------|------|------|
| CadXStudio | Free browser-based AI CAD + CAM platform; turns plain-language prompts into parametric 3D models, generates G-code, with Git-style versioning. | [cadxstudio.in](https://cadxstudio.in/) | `Free` |
| Adam (adam.new) | AI CAD copilot generating parametric 3D models from text/images in seconds; exports STEP/STL/OBJ. (YC W25; see CADAM for its OSS component.) | [adam.new](https://adam.new/) | `SaaS` |
| MecAgent | AI CAD copilot integrating with SolidWorks, CATIA, Inventor, Fusion 360, Creo — generates parts from text, runs standards checks, estimates cost. | [mecagent.com](https://mecagent.com/) | `SaaS` |
| CADAM | Open-source text-to-CAD web app behind Adam — natural language/images → parametric models via OpenSCAD, in-browser via WebAssembly; exports STL/SCAD/DXF. | [github.com/Adam-CAD/CADAM](https://github.com/Adam-CAD/CADAM) | `OSS` |

## Business, Marketing & Career

Pitching, marketing, product management, and job-search tooling.

| Tool | What it does | Link | Tags |
|------|--------------|------|------|
| Career-Ops | Job-search system on Claude Code — scans career portals, reasons about job fit vs your CV, and generates per-listing ATS-optimized resume PDFs. | [github.com/santifer/career-ops](https://github.com/santifer/career-ops) | `OSS` `Skill` |
| marketing-skills | Collection of marketing skills for Claude Code/AI agents — CRO, copywriting, SEO, analytics, growth engineering. | [github.com/coreyhaines31/marketingskills](https://github.com/coreyhaines31/marketingskills) | `OSS` `Skill` |
| pm-skills | 100+ Claude Code skills/commands for product managers across the full lifecycle — discovery, strategy, PRDs/OKRs/roadmaps, market research, analytics (SQL, cohorts, A/B), and go-to-market. | [github.com/phuryn/pm-skills](https://github.com/phuryn/pm-skills) | `OSS` `Skill` |
| PitchUs | AI tool that converts a founder's pitch deck into a US VC-ready format — restructuring and optimizing the deck to match American investor expectations. | [pitchusai.com](https://www.pitchusai.com/) | `SaaS` |

## Web Scraping & Browser Automation

Turning the web into data and driving browsers programmatically.

| Tool | What it does | Link | Tags |
|------|--------------|------|------|
| Firecrawl | API/toolkit for scraping, crawling, and searching the web — turns sites into LLM-ready clean markdown / structured data. | [github.com/firecrawl/firecrawl](https://github.com/firecrawl/firecrawl) | `OSS` |
| Playwright | Microsoft's cross-browser automation library for end-to-end testing and programmatic browser control. | [playwright.dev](https://playwright.dev) | `OSS` |
| Perplexity (ppl-ai) | AI answer engine / conversational search. `ppl-ai` is Perplexity's GitHub org; public OSS (pplx-garden, pplx-kernels) lives under `perplexityai`. | [perplexity.ai](https://www.perplexity.ai/) | `SaaS` |

## UI / Web Design

Design-intelligence skills and resources for building better interfaces.

| Tool | What it does | Link | Tags |
|------|--------------|------|------|
| Emil Kowalski (skill + components) | Design engineer (Linear, ex-Vercel); creator of animations.dev, Sonner & Vaul, and an "Emil Design Eng" Claude skill encoding his animation philosophy. | [emilkowal.ski](https://emilkowal.ski) | `OSS` `Skill` |
| impeccable | Design-language skill (1 skill, 23 commands — polish, audit, critique, animate…) that makes AI coding harnesses better at frontend design. | [github.com/pbakaus/impeccable](https://github.com/pbakaus/impeccable) | `OSS` `Skill` |
| taste-skill | Design skill giving the agent "good taste" — DESIGN.md files that ban AI-slop patterns and enforce real typography, asymmetric layouts, tuned motion. | [github.com/Leonxlnx/taste-skill](https://github.com/Leonxlnx/taste-skill) | `OSS` `Skill` |
| UI/UX Pro Max | Design-intelligence skill: searchable database of styles, palettes, font pairings, UX guidelines, and charts across stacks, with a CLI to generate design systems. | [github.com/nextlevelbuilder/ui-ux-pro-max-skill](https://github.com/nextlevelbuilder/ui-ux-pro-max-skill) | `OSS` `Skill` |
| huashu-design | HTML-native design skill (inspired by Claude Design) — turns a sentence into high-fidelity prototypes, decks, animations, infographics; MP4/PPTX export. | [github.com/alchaincyf/huashu-design](https://github.com/alchaincyf/huashu-design) | `OSS` `Skill` |

## Datasets

| Tool | What it does | Link | Tags |
|------|--------------|------|------|
| The Well | 15TB collection of 16 physics-simulation datasets (fluid dynamics, MHD, acoustics, supernovae…) with a unified PyTorch interface for ML surrogate models. | [github.com/PolymathicAI/the_well](https://github.com/PolymathicAI/the_well) | `OSS` |

## System & Dev Utilities

Local machine, infrastructure, and analytics tools.

| Tool | What it does | Link | Tags |
|------|--------------|------|------|
| Mole | Free, open-source all-in-one macOS optimization toolkit — clean, uninstall, analyze, optimize, and monitor the Mac from the terminal. | [github.com/tw93/Mole](https://github.com/tw93/Mole) | `OSS` `Free` |
| docker-android | Docker image running Android emulators with noVNC and video recording — for Android app dev and native/web/hybrid testing (Appium, Espresso). | [github.com/budtmo/docker-android](https://github.com/budtmo/docker-android) | `OSS` |
| Clicky | Open-source macOS menu-bar AI teaching assistant — sees your screen, takes push-to-talk voice, and points its cursor at on-screen UI elements to guide you through tasks. Built on Claude + AssemblyAI + ElevenLabs. | [github.com/farzaa/clicky](https://github.com/farzaa/clicky) | `OSS` `Free` |
| Google Workspace (gws) | Google's cloud productivity suite (Gmail, Docs, Sheets, Drive, Calendar). Listed here for its MCP/Claude integrations that let agents read and write Workspace docs. | [workspace.google.com](https://workspace.google.com) | `SaaS` |

## Curated Lists

Meta-resources — lists worth mining for more tools.

| Tool | What it does | Link | Tags |
|------|--------------|------|------|
| awesome-opensource-ai | Curated list of battle-tested, production-proven, truly open-source AI projects, models, libraries, and dev tools. | [github.com/alvinreal/awesome-opensource-ai](https://github.com/alvinreal/awesome-opensource-ai) | `OSS` |
| awesome-claude-code | Curated list of skills, hooks, slash-commands, agent orchestrators, and plugins for Claude Code. (Generic name — several competing repos.) | [github.com/hesreallyhim/awesome-claude-code](https://github.com/hesreallyhim/awesome-claude-code) | `OSS` |
| awesome-design-md | Curated collection of 73+ DESIGN.md files extracted from major brand sites (Claude, Vercel, Airbnb, Tesla…). Drop one into a project so coding agents generate a matching UI. | [github.com/voltagent/awesome-design-md](https://github.com/voltagent/awesome-design-md) | `OSS` |

---

## 🔄 How this catalog is maintained

This catalog auto-updates from `raw.txt` via a Claude Code slash command.

1. **Drop new finds into [`raw.txt`](raw.txt)** — any format, one per line, partial names are fine.
2. **Run `/update-tools`** in Claude Code from this directory.
3. The command reads `raw.txt` and this `README.md`, figures out which entries are **not yet catalogued** (so it's safe to re-run), **web-researches** each new tool, classifies it into the scheme above, and inserts it into the right table. It then prints a summary of what changed.

The command definition lives in [`.claude/commands/update-tools.md`](.claude/commands/update-tools.md).
