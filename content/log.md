# Ingest Log

Append-only record of all ingests, queries filed back to wiki, and lint passes.
Format: `## [YYYY-MM-DD] operation | description`

---

## [2026-05-27] ingest | Session 1 — initial vault build

**Sources processed:** 4 articles (my_articles, Mar 2026), Twitter archive (my_social)

**Pages created:**
- wiki/vibe-coding
- wiki/prototypes-and-disposable-apps
- wiki/ai-in-contract-drafting
- wiki/ai-productivity-and-hidden-costs
- wiki/legal-tech-strategy (from Twitter archive)
- wiki/knowledge-management-in-law (from Twitter archive)
- wiki/index

---

## [2026-05-28] ingest | Session 2 — article archive + Karpathy pattern adoption

**Sources processed:**
- `2026-03-02_Why-I-was-wrong-about-vibe-coding.md` → updated wiki/vibe-coding (Cursor journey, self-reflections)
- `ai-copilots-everywhere-now-what.md` → created wiki/ai-copilots
- `draft_Agentic-search-and-legal-knowledge-management.md` + `draft_agentic-search-article.md` + `podcast_agentic-search-without-the-hype.md` → created wiki/agentic-search
- `I-want-to-do-knowledge-management-what-do-I-do-first.md` → created wiki/km-getting-started
- `A Realist's Guide to Legal Tech.txt` (Book Ch. 1) → updated wiki/legal-tech-strategy (unspoken mundane, vapourware/shelfware/SISP, dinosaurs vs dreamers)
- HTML: `2025-10-23_KM-curation.html` + `2024-11-22_AI-agents.html` + `2025-02-10_gold-nuggets.html` → updated wiki/knowledge-management-in-law (curation/categorisation/contextualisation triad), wiki/agentic-search
- DOCX: Knowledge Base templates (business case, eval framework, pilot guide, landscape) → wiki/km-getting-started (business case section)
- `ai-and-contract-drafting-substack.md` → duplicate of existing processed article, no new content

**Schema change:** Adopted Karpathy LLM Wiki pattern — updated CLAUDE.md to codify ingest/query/lint operations; added log.md; updated index.md to catalog format

**Pages created:** wiki/agentic-search, wiki/ai-copilots, wiki/km-getting-started, wiki/log
**Pages updated:** wiki/vibe-coding, wiki/knowledge-management-in-law, wiki/legal-tech-strategy, wiki/index

**Backlog noted:** ~40 HTML articles from 2019–2025 remain unprocessed (listed in wiki/index)

---

## [2026-05-28] ingest | Session 3 — HTML backlog batch 1

**Sources processed:**
- `2023-09-23_What-are-the-specific-use-cases-for-generative-AI-in-contract-drafting.html` → integrated into wiki/ai-in-contract-drafting (partial — distinct use-case framing noted but substantial overlap with existing content)
- `2023-07-03_Knowledge-management-and-AI--a-match-made-in-heaven.html` → updated wiki/knowledge-management-in-law (European/US divide fleshed out, knowledge vs text section)
- `2025-02-19_Legal-Tech--AI--and-Automating-Our-Brains--Striking-the-Right-Balance.html` → created wiki/ai-process-design (intrinsic value of manual work; AI as building block not process; tasks vs processes)
- `2025-03-03_AI--process-design-and-benchmarking.html` → merged into wiki/ai-process-design (process models 1–4A; accuracy thresholds; multi-factor benchmarking framework)
- `2022-09-12_Transaction-management---knowledge-management--the-missing-link.html` → created wiki/transaction-management (structured vs unstructured; deal bible as KM; pandemic catalyst)
- `2021-09-27_Adoption-of-legal-tech.html` → created wiki/legal-tech-adoption (shelfware; zone of apathy; pull/push factors; fee pressure; user-centric communication)

**Pages created:** wiki/ai-process-design, wiki/legal-tech-adoption, wiki/transaction-management
**Pages updated:** wiki/knowledge-management-in-law (added "What AI Can and Cannot Tell About a Document"), wiki/index

**Backlog remaining:** ~34 HTML articles from 2019–2025
