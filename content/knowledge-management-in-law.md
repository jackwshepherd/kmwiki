# Knowledge Management in Law

**Summary**: KM in law firms sits at the intersection of process design, technology, and culture — and the biggest barrier is often simply that lawyers don't think to share knowledge, because sharing isn't built into how work is done.
**Tags**: #knowledge-management #KM #law-firms #process #information #taxonomy
**Created**: 2026-05-27
**Last Updated**: 2026-05-27

---

## The European vs US Divide

Two fundamentally different views on what KM is:

| Approach | View | Implication |
|----------|------|-------------|
| US | Technology project — aggregate all data, make it searchable | "We will never get our lawyers to do anything to the content itself" |
| European | Content project — separate usable from unusable content | Technology is a skin over well-curated content |

The most sensible approach treats it as both. You won't get decent KM value without doing something to the content. At the same time, you can't curate everything, so you need a technology layer for the rest. All firms appear to be converging towards this middle ground.

---

## The Curation / Categorisation / Contextualisation Triad

These three are often conflated — they are distinct:

**Curation** = separating useful data from unhelpful data (e.g. "final", "reusable", "PSL-approved"). A qualitative assessment. Not generally apparent from the four corners of a document — requires information about the circumstances in which the document was made.

**Categorisation** = adding profiles or labels to data (e.g. "share purchase agreement", "New York law", "white-list assignment provisions"). Increasingly automatable with LLMs. But LLMs are probabilistic, so for core characteristics, pre-classification is still needed for consistency.

**Contextualisation** = annotating documents with notes about context (e.g. "we were forced to accept Clause 4.1, but avoid doing so on future matters"). Hardest of the three — requires headspace and time, and the important context is usually not in the document but known only by the lawyer who drafted it.

Having all three is the holy grail. It's very hard.

### Why Curation Is Hard

The classic techniques — lawyers marking documents as final or placing them in specific locations — consistently fail. Not because of time (you can reduce the effort to seconds, and people still don't do it). They fail because:
1. Lawyers don't think to do it — it's not built into how they work
2. It's not enforced
3. Lawyers enjoy a significant degree of latitude in how they work and resist defined processes

### Degrees of Curation

Curation is not binary:
- Level 1: final documents (the hallmark of having been signed off)
- Level 2: good or useful final documents specifically marked as appropriate to reuse
- Level 3: compiled playbooks from useful final documents — one source of truth, not scattered individual documents

The balance is always between what's practically doable given culture and resources, and what value you want to drive.

### Why People Say Curation Is No Longer Needed

Vendors promising automation of curation, categorisation, and contextualisation have always been well-received because law firms want to believe the manual effort is unnecessary. It's an easy sell, and very difficult to deliver — mostly because curation is a qualitative assessment that depends on information outside the document. AI can tell you a document is a share purchase agreement. It can't tell you whether it represents the firm's best practice, or whether a key clause was accepted for exceptional client-specific reasons that shouldn't be replicated.

See [[agentic-search]] for the specific question of whether agentic search changes this. Short answer: curation matters *more* with agentic search, not less.

### Curating as You Go

The most promising direction: weaving curation into the fabric of tools lawyers use every day.

Examples:
- Transaction management tools using deal closing processes as automatic curation triggers
- Structured document versioning (auction draft → execution version → executed copy) instead of anonymous numbered versions (1, 2, 3)
- One-click "flag for reuse" at point of save

The model needs to shift from curation as a separate after-the-fact process to curation as a by-product of something useful.

---

## The KM Workflow Breakdown

A useful frame for where AI can and can't help in European-style (curated) KM. Five stages of the knowledge process:

| Stage | What it involves | AI potential |
|-------|-----------------|--------------|
| **Building** | Creating guides, playbooks, templates — the "crown jewels" built by knowledge lawyers or on a side-of-desk basis | Can generate content that looks human-written, but depends on quality of input data. Hallucination risk is real. "Garbage in, garbage out" applies at a knowledge-asset level |
| **Sharing** | The rate-limiting step — lawyers deciding what to surface, how, and when | Some tools propose proactive recommendations for what to share. Will remain a human volition problem. The AI has to understand what "good" looks like, which requires curated input |
| **Categorising** | Adding metadata labels so content is findable (practice group, document type, jurisdiction, etc.) | Strong AI potential — predictable fields can be pre-populated. Limits: human nuance (e.g. contextual drafting notes) cannot be filled in by AI. Pick the specific fields AI can handle, not the whole form |
| **Reviewing** | Quality gate — catching client-confidential content, poor quality submissions, near-duplicates | Auto-triage potential: flag for redaction, flag near-duplicates for rejection. Lower complexity than building or sharing |
| **Maintaining** | Updating knowledge for law changes, marking stale content | Limited AI potential currently — temporal training data limitations mean AI struggles to know what's current |

The pattern: AI helps most at the categorising and reviewing stages. Building and sharing require human judgement. Maintaining is a gap.

The chicken-and-egg problem with AI-driven building: to generate high-quality knowledge, you need high-quality training data — which means curated content. So you still need curation to drive AI output quality. There is no shortcut around the content problem.

---

## The Core Problem

> *Perhaps the biggest blocker to knowledge sharing in law is people not thinking to do it...it doesn't come up naturally in processes.*

There is no "Submit to Knowledge" button on the water cooler. Knowledge is created constantly in law firms — in deals, in client advice, in negotiations — but capturing it requires deliberate process design. Left to organic behaviour, it doesn't happen.

This is why structuring processes (e.g. transaction management workflows) is so interesting for KM. If the capture moment is built into the process, it doesn't require people to remember to do an extra step.

---

## Knowledge vs. Text

An important distinction that gets blurred:

> *Text is one thing... language is another... and knowledge/ideas reduced into text and language is another altogether.*

We should be careful about conflating principles, experience, ideas, and knowledge with text. AI can process text. Whether it processes *knowledge* — the tacit understanding of how a clause performed in a real negotiation, why a particular structure was chosen, what the client's underlying concern really was — is a different question.

This matters enormously for AI in legal work. See [[ai-in-contract-drafting]].

---

## Taxonomy and Metadata

> *I've never met a law firm that has not been intimidated by the prospect of designing some sort of taxonomy or metadata schema for their information.*

In reality, it shouldn't be that scary. The rules:
1. Don't design by committee
2. Don't make it too complex

The problem isn't taxonomy design itself — it's the organisational dynamics around it. Committee design produces bloated, unusable schemas. Over-engineered taxonomies get abandoned.

Moving from folders to metadata is a fundamental conceptual shift that many lawyers haven't made. Folders are intuitive; metadata is more powerful but requires understanding the principle first.

---

## The Information Governance Challenge

Information governance is distinct from security (though often lumped together):
- Is data segregated from one client to the next?
- How do changes to policies (e.g. a client becomes adverse to another) get enforced across the tools and databases where the data lives?

This is one of the "boring stuff" categories from the [[vibe-coding]] framework — crucial, but chronically deprioritised because it's not exciting.

---

## What Law Firms Get Wrong

### Keeping Success Stories Quiet

Law firms keep their actual innovation success stories too quiet. Their clients would love to hear about these — those clients face the very same challenges of tidying data, contracts, and fixing broken processes. Great opportunity to showcase what's being done.

### Tech Without Process

> *There is still massive over-investment in tech implementation and under-investment in business process implementation across the legal world.*

The cake still needs putting in the oven. AI is the cherry on top. See [[ai-in-contract-drafting]] for the full argument, and [[legal-tech-strategy]] for the strategic view.

### The Echo Chamber

Consensus exists in the KM/legal tech world. The people who need to change often aren't part of the conversation — or are ignoring it. The problem is translating frameworks into specific tasks people can actually do.

---

## AI and KM: Where It Helps

The most compelling use of AI in KM isn't generating content — it's making structured processes easier to trigger. Examples:
- An AI agent that interprets a term sheet and populates a contract automation form (see [[ai-in-contract-drafting]])
- AI that surfaces relevant precedent when a lawyer starts a new matter, without requiring the lawyer to search
- AI-assisted tagging and classification of documents at the point of creation (reducing the "think to do it" problem)

The pattern that works: **AI as the interface layer on top of deterministic, well-curated underlying knowledge**. Probabilistic input; deterministic output.

---

## What AI Can and Cannot Tell About a Document

A useful frame for understanding the limits of AI in KM:

**What AI can tell:**
- Document type (share purchase agreement, advice memo, etc.)
- Applicable jurisdiction and governing law
- Whether specific provisions exist or are absent
- Named parties, dates, defined terms

**What only a human can tell:**
- Whether the document represents the firm's best practice
- Whether a clause was accepted for exceptional client-specific reasons that shouldn't be replicated
- Whether advice given was correct (vs received from another firm being sued for negligence)
- The negotiating context and what it means for reuse

The implication: AI is very useful for categorisation (labelling documents with profiles). It is not sufficient for curation (making the qualitative judgment that a document is reliable and reusable). Curation depends on information outside the four corners of a document.

Firms with well-structured, well-labelled knowledge bases will get far more value from AI tools than firms that throw their entire DMS at an LLM and hope for the best. Building "AI-ready" knowledge means doing the curation and categorisation work now — not waiting for AI to do it.

## The Customer Success Analogy

Law firms could experiment with drawing from customer success principles — treating each practice group's adoption of a tech or knowledge solution in the same way a CSM treats individual clients, with success plays tailored to their specific context and needs. This is worth exploring particularly for international firms where adoption patterns vary significantly across offices.

---

## Related Notes
- [[ai-in-contract-drafting]] — AI and contract knowledge: what's still unsolved
- [[agentic-search]] — whether agentic search removes the need for curation (it doesn't)
- [[km-getting-started]] — practical framework for starting a KM programme
- [[transaction-management]] — structured deal processes as a natural KM capture mechanism
- [[legal-tech-strategy]] — Process before tech; the user research approach; taxonomy in practice
- [[ai-productivity-and-hidden-costs]] — The risk of AI replacing thinking rather than supporting it
