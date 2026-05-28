---
title: "AI and Process Design"
---

# AI and Process Design

**Summary**: AI is a building block within a process, not a replacement for a process. The right model of AI-human collaboration depends on the goal, context, accuracy requirements, and whether the cognitive work of doing the task has intrinsic value.
**Tags**: #AI #process-design #legal-tech #benchmarking #accuracy #legal-processes
**Created**: 2026-05-28
**Last Updated**: 2026-05-28

---

## The Core Principle

> *AI alone will not deliver any value — it only delivers value within the context of a process.*

AI is a building block within a process. Its value manifests in how a given outcome can be delivered more effectively in a process redesigned and enabled by AI. When people say "AI is better at redlining than humans" or "AI will replace the billable hour," they're treating AI as a process-level replacement rather than a component within a process. That's where most thinking goes wrong.

The implication: benchmarks (e.g. "AI performs at X% accuracy on task Y") are useful but incomplete. You have to step back and understand what you're trying to achieve from the overall process, then find the best way to weave AI into it.

---

## Tasks vs Processes

A critical distinction that gets routinely conflated:

**Processes** operate at a higher abstraction. They are comprised of multiple tasks. Contract drafting is a process; redlining is a task within it.

**Tasks** are where technology supports work. Technology helps reshape tasks, which in turn redesigns the process.

The mistake: legal tech vendors want the bucket of "manual things lawyers hate doing" to be as large as possible. They inadvertently include tasks in that bucket that are not actually manual or tedious at all. Contract drafting and legal research are processes that involve some terrible tasks and some genuinely valuable ones — treating the whole process as something to automate misses the point.

> *I struggle with AI companies who try to automate my brain but not my keyboard clicks.*

The right framing: be specific about which tasks within a high-value process are genuinely mechanical, and target those. Automate the court binder, not the litigation strategy. Automate the cross-reference checking, not the drafting of the termination clause.

---

## The Process Models (Chronology Example)

Using chronology generation as an example — a task that appears in complex litigation:

| Model | Who builds | Who checks | When appropriate |
|-------|-----------|-----------|-----------------|
| Model 1 | Human | Human | Traditional baseline |
| Model 2 | AI | Human (quick) | You already know the facts; just need them recorded |
| Model 3 | AI | Human (deep) | You don't know the facts; must read documents to verify |
| Model 4 | Human | AI | Fundamental goal is knowledge acquisition, not just artefact production |
| Model 4A | Human + AI assistance | AI | Complex matters; need knowledge in head; AI helps surface things and supervise |

The right model depends on the context:
- Complex litigation where you need all the facts in your head → Model 4 or 4A
- Simple litigation where everyone knows the facts and you just need a reference document → Model 2 or 3

The mistake is assuming everything is Model 2 (AI in the driving seat, human checks at end).

---

## Accuracy Thresholds Are Context-Dependent

Different processes require different levels of accuracy. This is not a single curve — it changes based on the use case.

**When accuracy threshold is low** (you already know the facts, just need them recorded):
- Value is proportionate to accuracy after a point
- Very low accuracy → still slower than doing it yourself
- Reasonable accuracy → meaningful value, even if not perfect
- Very high accuracy → diminishing returns

**When accuracy threshold is high** (output goes to court; you don't know the documents):
- Low-to-moderate accuracy → no value, possibly negative value (harder to spot errors in confident AI output)
- High accuracy needed to make the process viable
- The "humans should always check AI output" caveat is insufficient when errors are hard to spot

> *There may be a dip in the curve as work transitions from obviously inaccurate to deceptively inaccurate — because it becomes harder to spot errors.*

**When accuracy threshold is moderate** (AI as "better search" within documents to surface relevant sections):
- Being too accurate might stop people from considering issues they hadn't thought to search for
- Value may plateau or even decline after a certain accuracy level

The takeaway: accuracy is not a universal metric. Think about it in context of the process and how it's deployed.

---

## The Intrinsic Value Problem

Some manual tasks appear to be pure overhead but contain hidden value. The court bundling example:

Court bundling — gathering documents, indexing, relabelling, producing in a specified format — was hated. It caused late nights, caused stress when documents needed reordering. It looks like prime automation territory.

But: the person who spent hours making the court bundle knew the documents like the back of their hand. When the case went to court and someone had an urgent question about which documents were relevant, that person could answer immediately. The manual process had built knowledge as a by-product.

Automating this removes the knowledge-building by-product. The question becomes: if you automate court bundling, how do you replace the knowledge that process was building? Can technology enable the same level of familiarity without the tedium?

This is the general challenge: **some boring things might have intrinsic value, so be careful automating them.** Not a reason to preserve manual processes — but a reason to understand what you'd lose and find a way to replace it.

---

## Context Matters for "Is This Boring?"

Not all instances of the same process type are the same:

- Drafting a termination clause carefully to account for cross-defaults in associated contracts → high-value, worth a lawyer's full attention
- Drafting a third-party provisions clause in a standard contract → probably templatable, lower value
- Legal research on directors' duties (always the same) → could be templated
- Legal research on a novel point of law with strategic implications → high value, worth deep engagement

The context — who the client is, what the stakes are, how standardised the situation is — determines whether a task within a process is genuinely mechanical or genuinely valuable.

---

## The Multi-Factor Benchmarking Framework

When assessing whether and how to deploy AI in a process, the factors to weigh:

| Factor | Question |
|--------|---------|
| Speed | Is time of the essence? Better to have something than nothing? |
| Importance | How good does the work product actually need to be? |
| Cost | What can the client pay for it, given its importance? |
| Transparency | How important is it that every conclusion can be reverse-engineered by a human? |
| Consistency | How important is it that the same exercise is done identically each time? |
| Insights | Is a key purpose to store data for future reuse that a human would never capture? |
| Knowledge | Does doing the task build expertise the person needs for subsequent work? |

Weighing these factors differently produces different optimal process models. A high-complexity litigation context (speed less critical, knowledge critical, transparency critical) pushes toward Model 4A. A high-volume, time-sensitive, standardised context pushes toward Model 2.

---

## The Legal Research Case

Legal research illustrates the intrinsic value problem most clearly:

A legal opinion in a banking transaction → its value largely lies in the words on paper (risk resolution). Could in principle be automated with complete accuracy.

A complex legal advice memo during litigation → its value lies in both the words and in the knowledgeable lawyer who can facilitate discussion, answer follow-ups, think outside the box. Automating this with complete accuracy doesn't produce the same outcome — you lose the lawyer who knows the facts in depth.

> *Before assuming we need to involve AI in a specific workflow and that AI needs to be accurate, we should consider whether we are automating away a process that itself has intrinsic value.*

---

---

## Easy vs Hard Verification Exercises

"Humans should always check AI output" is often cited as the mitigation for hallucinations. Whether this actually mitigates risk depends on what humans are being asked to verify.

**Easy verification**: The AI extracts a data point (e.g. governing law clause). A well-designed product shows the extract alongside the source document, making cross-referencing trivial. The human can verify quickly and reliably. The benefit of AI is largely preserved.

**Hard verification**: The AI produces a legal research memo or detailed contractual analysis. The human must read, interpret, and compare multiple sources — often making judgment calls. Hard verification has three problems:
1. **Laziness** — humans are more inclined to trust AI output when verification is effortful. The cognitive load of checking makes shortcuts tempting.
2. **Anchoring** — the AI's output shapes how the human thinks about the problem. If the AI went down the wrong track, the human may not consider alternatives.
3. **Benefit offset** — checking complex AI output takes time. Some or all of the efficiency gain is eaten by verification effort.

The implication: "humans check everything" is a viable mitigation for easy exercises. For hard exercises, the reliance on human verification needs to be scrutinised carefully — and for some use cases, the only real solution is not to use AI at all, or to limit AI to the parts of the task that don't require hard verification.

**What makes verification hard vs easy** — it's not output length; it's the nature of the judgment calls required and the extent to which you can verify without being influenced by the AI's framing.

---

## Hallucinations: What They Are and Aren't

LLMs are designed to do one thing: predict the next token. Their only operational success metric is whether they correctly predict the most likely next word given the context. This is explicitly *not* a measure of factual accuracy.

"Hallucination" was coined to describe cases where LLM output is wrong, fabricated, or cites non-existent sources. The term exists because LLMs are often judged against a goal (factual accuracy) they were not designed to achieve.

Implications:
- Telling an LLM "don't hallucinate" affects the token prediction calculation, not any underlying verification mechanism — it changes what word the model thinks is likely, not whether the model is checking facts
- RAG (retrieval-augmented generation) reduces hallucinations by grounding output in a trusted dataset, but doesn't eliminate them — you can't always tell what came from the dataset vs the foundation model, the wrong dataset sections may be retrieved, or the dataset itself may be wrong
- Larger models and reasoning loops ("verify your own output") reduce hallucination frequency but don't eliminate it
- The practical strategy isn't to try to eliminate hallucinations — it's to choose use cases and verification processes where their effect can be mitigated

The corollary: when evaluating an AI tool and asking "how accurate is it?", you're asking about a secondary property, not a designed-in one. Tools can be optimised to improve accuracy, but it should be treated as something to mitigate around rather than something to assume away.

---

## Related Notes
- [[ai-in-contract-drafting]] — specific application to contract drafting stages; three drafting models
- [[agentic-search]] — when answer generation is and isn't the right goal
- [[ai-productivity-and-hidden-costs]] — the same argument about writing-as-thinking
- [[legal-tech-strategy]] — process before tech; levels of abstraction in use cases
- [[legal-tech-adoption]] — making the case for process change to lawyers
