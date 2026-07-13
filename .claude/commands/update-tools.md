---
description: Research tools given in the prompt and add them to README.md
argument-hint: <tool names / URLs / hints, in any format>
allowed-tools: Read, Edit, Write, WebSearch, WebFetch, Bash, Agent
---

You maintain the `awesome-ai-stack` catalog. Your job: take the tool candidates the user provided **directly in the prompt** (below as ARGUMENTS), research the ones **not yet** in `README.md`, classify them, and add them to the catalog. Be accurate over comprehensive — flag what you can't verify rather than guessing.

## Steps

### 1. Read the catalog and parse the input
- Read `README.md` (the catalog) in this directory.
- Parse ARGUMENTS into individual tool candidates. The input is freeform — names may be one per line or comma-separated, misspelled, partial, in Korean/English mixed, with optional hints in parentheses (e.g. "Cognee (기억 향상)") or URLs. One tool per line/clause; a line can also contain multiple distinct tools (e.g. "A + B" may be two tools — use the hints and research to decide). Ignore empty lines and non-tool commentary.
- If ARGUMENTS is empty, ask the user to provide the tools to research and stop.

### 2. Diff — find new entries
- For each candidate, check whether it's **already represented** in `README.md`. Match by canonical name OR raw alias — fuzzily. A tool already in the catalog under any spelling is NOT new. When unsure whether something matches, treat it as already-present (don't create duplicates).
- The result is the list of **new candidates**. If the list is empty, report "Nothing new to add" and stop.

### 3. Research each new candidate
- Use `WebSearch`/`WebFetch` to identify each tool. For many candidates at once, fan out parallel `Agent` (general-purpose) calls — one agent per batch of ~8 tools — to keep it fast. Pass along the user's hints. Give each agent this output contract per tool: **canonical name, one-to-two-sentence factual description, official link (GitHub repo preferred, else homepage), confidence (FOUND / UNCERTAIN / NOT_FOUND), open-source? (yes/no/unknown)**.
- Prefer official/primary sources. Note when a raw name is a misspelling of a known project (e.g. "haushu" → "huashu").

### 4. Classify and write
For each researched tool, decide placement:

- **NOT_FOUND** (no real tool matches the name) → do NOT add it to `README.md`. Report it back to the user with what was searched and ask for the correct name or a link.
- **FOUND / UNCERTAIN** → add a row to the single best-fitting category table below. If UNCERTAIN, still place it in the best category but note the uncertainty in the description and add the `` `⚠️` `` tag.

**Categories** (use the existing section that fits best; only create a new `##` section if a tool genuinely fits none):
`Research & Academic` · `RAG & Knowledge Management` · `LLM Optimization & Local Inference` · `Agent Frameworks & Multi-Agent Systems` · `Claude Code Skills & Plugins` · `Creative & Media Generation` · `CAD & Engineering` · `Business, Marketing & Career` · `Web Scraping & Browser Automation` · `UI / Web Design` · `Datasets` · `Open Models` · `System & Dev Utilities` · `Curated Lists`

Placement rules of thumb:
- Classify by **primary domain/function**. A Claude Code skill with a strong domain (e.g. a marketing skill) goes in its domain section with a `` `Skill` `` tag; only tools whose primary identity *is* "a Claude Code skill/plugin" (memory, orchestration, spec frameworks, IDE plugins) go in **Claude Code Skills & Plugins**.
- Open-weight models (LLMs, vision models…) whose identity is "a model you download and run" go in **Open Models**; a domain-specific model with one clear use case (e.g. SAM 3D) goes in its domain section instead.

**Row format** (match the existing tables exactly):
```
| Tool name | One-to-two-sentence factual description. | [short-link-text](https://full-url) | `Tags` |
```
- Link text: strip `https://` and trailing slashes (e.g. `github.com/owner/repo` or `tool.com`).
- **Tags** from this set: `OSS` (open source) · `SaaS` (commercial/hosted) · `Skill` (Claude Code skill/plugin) · `Free` (free to use) · `⚠️` (identity not fully verified). Combine as appropriate.
- Insert rows in a sensible spot in the table (keep related tools near each other; otherwise append).
- If you added a brand-new `##` section, also add it to the **Contents** list near the top.

Use `Edit` to insert rows into the correct tables. Do not reorder or rewrite existing rows.

### 5. Report
Print a concise summary:
- ✅ Added: `<tool>` → `<category>` (one line each)
- ❓ Not found (needs correct name/link from user): `<tool>` (one line each)
- ⏭️ Skipped (already catalogued): count only

Do not commit to git unless the user asks.

## Principles
- **Idempotent:** re-running with the same input must change nothing.
- **Accuracy over coverage:** an honest ⚠️ flag or a "not found" report beats a confident wrong entry.
- **Preserve the file:** only add rows (and Contents entries / new sections when needed); never delete or restructure existing content.

ARGUMENTS: $ARGUMENTS
