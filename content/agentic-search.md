---
title: "Agentic Search"
---

# Agentic Search

**Summary**: Agentic search is a genuine and exciting addition to the legal knowledge toolkit — but the hype has overshot the reality. Curation still matters. Categorisation still matters. Learning from reading still matters. It is one route, not the only route.
**Tags**: #agentic-search #knowledge-management #AI #legal-tech #search #KM
**Created**: 2026-05-28
**Last Updated**: 2026-05-28

---

## What It Is

Agentic search takes a user's question and does the following in sequence:

1. **Connect** — works out which systems are relevant to the query (via MCP, the protocol that lets AI talk to a DMS, knowhow library, email, billing system, etc.)
2. **Search** — breaks the question into multiple search queries with keywords and filters; runs them in parallel across connected systems; ranks and filters the results
3. **Output** — returns a synthesised answer with citations drawn from everything retrieved
4. **Explore** (emerging) — spins up a bespoke interface for the specific query — a sortable table, a filterable dashboard — so the answer becomes a workspace rather than a static destination

The promise: you can skip the painful exercise of running keyword searches, handling boolean logic (SPA OR "Share Purchase Agreement"), working out which systems to search, and manually reading documents to piece together an answer.

---

## Why Everyone Is Excited

The pitch is obvious. All that repetitive retrieval work becomes unnecessary. The AI handles permutations of search terms, knows which systems to look in, filters out irrelevant hits, and synthesises the answer.

And the demo looks amazing — particularly from non-legal vendors whose primary customers have lots of straightforward questions ("what is our expense policy?", "where are the brand guidelines?") where agentic search is a massive improvement over digging through SharePoint folders.

---

## What the Hype Gets Wrong

The framing of some vendors — that agentic search is *the* future and everything else is legacy — misses something important. There are four questions worth working through:

---

## 1. Curation: Still Needed

**Curation** = separating useful documents from unhelpful ones (finals, reusables, PSL-approved). Distinct from **categorisation** (labelling documents with profiles like "share purchase agreement" or "New York law").

The vendor pitch: curation is dead because AI will figure out what's good on the fly.

The problem: curation depends on information outside the four corners of a document. A document cannot tell you whether it was drafted by your firm or received from the firm you're now suing for professional negligence. A document cannot tell you whether a senior partner accepted a clause for exceptional client-specific reasons that shouldn't be replicated. These qualitative assessments require context that AI cannot access at scale — not yet.

If anything, curation matters *more* with agentic search than before. With traditional search, the user reviews documents and applies their own judgment. With agentic search, that step is automated away. In practice, users almost never check citations. They trust the answer. So if the underlying data is messy, the synthesised answer is built on shaky foundations.

**The litter-picker analogy:** Two camps exist in AI. One says tidy up data at source so the AI has clean material to work with. The other accepts the litter as fact and bets on robot litter-pickers to sift through the mess. The "don't litter" camp is right. Admitting defeat on tidy data is lazy — most of these are process problems wearing technology costumes.

> *Verdict: we still need to curate data.*

---

## 2. Categorisation: Pre-Classify Core, Let AI Sweep Up the Rest

**Categorisation** = labelling documents with profiles (contract type, governing law, deal size, features).

The vendor claim: AI can classify everything at the moment of need, so no pre-classification is needed.

Three problems with on-the-fly classification only:

1. **Consistency** — LLMs are probabilistic. Person A asks about loan agreement assignment provisions and gets "white list / black list." Person B asks the same tomorrow and gets "permitted / not permitted." You can't compare notes. Research can't be replicated.
2. **Speed and cost** — classifying long documents takes time and money. If you do it every time someone asks a question instead of storing it once, you pay for the same work repeatedly.
3. **Scale** — on-the-fly classification only works on small document sets. To get to that smaller set in the first place (show me loan agreements → show me loan agreements with assignment clauses → show me white-list assignment clauses), you need pre-classification.

The nuanced view: AI can sweep up the long tail — quirky or bespoke characteristics nobody predicted in advance. But core characteristics still need pre-classification up front.

> *Verdict: pre-classify the core; let AI handle the rest.*

---

## 3. Search, Filter and Browse: Not Dead

Four kinds of searches lawyers actually do:

| Type | Example | Best tool |
|------|---------|-----------|
| Known item, known details | "Find document #1,442,111" / "Final SPA from Project Mercury" | Traditional search/filter |
| Known item, unknown details | "The email I sent to the client about measure of damages last year" | Mixed |
| Unknown item, known details | Research with some parameters | Agentic search helps |
| Unknown item, unknown details | Discovery, market practice research | Agentic search shines |

A lot of legal work sits in the first quadrant. Agentic search is overkill there — a probabilistic chat interface is more likely to misinterpret a known-item query than help with it. The tooling for this quadrant has been embarrassingly poor for years. Agentic search doesn't fix that gap.

> *Verdict: agentic search helps discovery and avoids repetitive querying. Targeted retrieval still needs targeted tools.*

---

## 4. Answer Generation: Situational

For some queries, synthesised answers work well:
- Market practice questions ("how many of our loan agreements have white-list assignment provisions?")
- Legal research questions ("in what circumstances does common interest privilege apply?")

For **drafting**, much more caution is warranted. You want a clause that has been used before, that is authoritative. A synthesis of fragments from various clauses, never appeared together as standalone language in the wild, is a different beast.

### Two assumptions worth challenging

**Assumption 1: hallucinations go away if AI is grounded in your own documents.**
False, in two ways:
- The wrong documents may be retrieved, making the synthesis built on the wrong foundation
- Even with the right documents retrieved, the LLM can hallucinate while synthesising them. The output looks plausible, reads well, and is wrong.

**Assumption 2: needing to read documents is a problem to fix.**
Situational. For basic questions ("what's our sick leave policy?"), a direct answer is fine. For complex questions, the engagement with underlying materials is where the real learning happens.

A lawyer who asks "in what circumstances does common interest privilege apply" and accepts a four-bullet answer will look like a fool the first time a client asks a follow-up. Reading the underlying cases and articles gives you an understanding of the doctrine, the policy reasons, the contested edge cases — the things that let you have a real conversation.

> *This is my biggest worry about AI in general. The value of much professional work lives in flexing your brain muscles on the way to the answer. If you skip yourself straight to the answer every single time, you end up with professionals who can produce outputs without being able to think.*

> *Verdict: answer generation works for market practice and research questions; use with caution for drafting and complex legal matters.*

---

## Where Agentic Search Fits in the Legal KM Toolkit

| Use case | Role of agentic search |
|----------|----------------------|
| Internal corporate knowledge (policies, HR, firm guidance) | Can be primary route — accuracy bar moderate, learning value low |
| Legal research, complex advisory | Useful as starting point and for initial orientation; output should prompt further investigation, not replace it |
| Precedent retrieval (drafting starting point) | Some help in discovery phase; qualitative fit-for-purpose judgment remains manual |
| Market practice analysis | Promising; accuracy requirements still high; data quality determines reliability |

---

## The Data Foundation Point

The underlying data matters enormously. Your DMS is the riverbed; useful documents are the gold nuggets. Before reliable agentic search, you need a strategy for separating gold from silt — through rules-based extraction, indicators, or human curation woven into existing workflows. The firms that will get the most from agentic search are those that have invested in organising their knowledge properly.

AI can amplify good knowledge management practices. It cannot substitute for them.

---

## Agentic AI: The Broader Concern

Agentic AI (AI that breaks a task into steps, feeds its output back into itself, and takes a series of reasoned actions) is genuinely exciting. But some caveats:

- **Control matters** — risk-averse professionals (lawyers especially) will want to understand the steps being taken and be able to course-correct. Product design needs to allow for this.
- **Stochastic vs deterministic** — LLMs are stochastic; the same prompt can produce different actions each time. For processes where consistency matters, this is a problem. Some processes are better served by deterministic expert logic applications, or a combination of both.
- **Human reasoning** — the argument that these systems "mimic human reasoning" is likely an oversimplification. The more important question is whether we're using the right tool for the job, and whether we lose something cognitively if AI repeatedly performs tasks that humans should be doing.

---

## Three Takeaways

1. Don't be the firm that throws away its DMS metadata because a vendor told you the AI would handle it.
2. Don't be the lawyer who stops reading cases because the synthesis is good enough.
3. Don't be the knowledge manager who admits defeat on data quality and hopes the robot litter-pickers will save you.

---

## Related Notes
- [[knowledge-management-in-law]] — curation, categorisation, contextualisation in depth
- [[km-getting-started]] — how to build the data foundation agentic search needs
- [[ai-in-contract-drafting]] — answer generation and provenance issues in a specific legal context
- [[legal-tech-strategy]] — process before tech; same principle applied to KM infrastructure
