# AI in Contract Drafting

**Summary**: Models have improved since 2023 and substantive holes in AI-generated drafts are fewer — but "fewer holes" still means holes, and the core issues around provenance, consistency, and knowledge capture remain unresolved.
**Tags**: #AI #contract-drafting #legal-tech #law-firms #knowledge-management
**Created**: 2026-05-27
**Last Updated**: 2026-05-27

---

## What's Improved

The quality of AI-generated drafting has improved noticeably since 2023. You're less likely to get the kind of howler that appeared then — e.g. ChatGPT producing a Lock-Up Agreement that allowed free transfers for gifts and unaffiliated parties, completely undermining the agreement's purpose.

Agentic AI and reasoning models have also improved: better document structure, more logical clause ordering, fewer internal contradictions. Real potential for review workflows where an agent cross-checks a draft against a term sheet or playbook in multiple passes.

## What Hasn't Changed

### The Provenance Problem
You're still reviewing a document of unknown origin with no idea where the risks might hide. And better drafting quality arguably makes this *worse*: the output looks polished, so you trust it. That's exactly when things slip through.

Battle-tested language that has survived real negotiations is still preferable to something that's never been used on a live deal, no matter how good it reads.

### Consistency
Generative AI produces different text each time. When two lawyers use a contract automation tool, they get the same document. When two lawyers prompt an LLM, they don't. This is a fundamental problem if you care about managing risk at scale.

### Knowledge Capture
An agent can reason about structure, but it has no lived experience of how a clause performed in a real negotiation. Better reasoning helps with mechanical and analytical tasks, but it doesn't solve the knowledge capture problem.

---

## Genuinely Interesting Developments

### AI Drafting Panels in Word
Panels embedded in Word that sit alongside your document, helping you refine language as you work. Meaningfully different from "generate me a first draft from a prompt."

The value: they *support* the lawyer's thinking rather than replacing it. You're still constructing each sentence, still reasoning through the document. The AI suggests alternatives, tightens language, flags ambiguities.

> *The process of writing is where lawyers actually learn the document. An LLM-produced first draft clouds thinking, whereas a tool that helps sharpen your own drafting keeps you in the driving seat.*

There are ways of using LLMs short of getting them to draft the entire contract. The industry is slowly waking up to this.

### Contract Automation + AI Interface
An important distinction that people still confuse:

| Contract Automation | Generative AI |
|---------------------|---------------|
| Templates with built-in logic | Produces novel text each time |
| Fill a form → right clauses appear | No guarantee of consistency |
| Deterministic output | Probabilistic output |

What's interesting: contract automation products are starting to expose themselves through protocols like MCP. An AI agent can trigger them via natural language — *probabilistic input, deterministic output*. 

This could go further: feed the agent a term sheet, client instructions, prior deal data. The agent interprets context and populates the automation form on your behalf. The template does the heavy lifting; AI makes it easier to get the right inputs in.

> *A more compelling use of AI in drafting than having it generate novel text from scratch.*

---

## Word as the Ceiling

A longer-term structural issue: at some point we will run out of road with Microsoft Word.

Right now, to get value from AI, documents must be processed, chunked up, and semantic layers built on the fly. That overhead limits the value extractable from these tools.

If lawyers worked in ways that naturally established relationships between clauses as they drafted, AI would have far more to work with. Several vendors have tried to fight this battle and pivoted. But the gap between how contracts are authored and how AI needs to consume them is real and growing.

---

## The Unchanged Conclusion

> *AI works best on a solid foundation of good templates, curated knowledge, and well-defined processes. Without these, you're asking AI to paper over cracks.*

There is still massive over-investment in tech implementation and under-investment in business process implementation across the legal world. The cake still needs putting in the oven. AI is the cherry on top.

---

## Three Models for AI-Assisted Drafting

Specifically for non-contract legal content — advice memos, research notes, situations where there is no template or clear precedent to start from. The blank page problem.

**Model 1: AI thinks, AI writes, human reviews**

Prompt the AI with a question or scenario; take the output as the starting point. The problem: the blank page forces the author to properly engage with the issues. Structuring ideas in your head establishes relationships between ideas and surfaces conflicts. If AI does this, the author may not be able to tell whether the direction "works" — because they haven't thought through it themselves.

> *The value of legal work product is often not in the words presented on a page, but the thought process and knowledge accumulated while making it.*

This model is uncomfortable for competent lawyers — and should be.

**Model 2: Human thinks, AI writes, human reviews**

Human develops the structure; AI pads it out with words. More defensible than Model 1. Benefits: removes time spent wordsmithing early drafts that a senior will rewrite anyway; may suit clients who value speed over stylistic perfection.

Practical problem: legal drafts rarely stay loyal to their opening structure. Writing surfaces weaknesses in the argument. If AI does the writing, those weaknesses surface later — if at all.

Also: AI-generated legal prose is typically full of clichés, jargon, and insufficient analysis.

**Model 3: Human thinks, human writes, AI reviews**

Jack's preferred approach: write the draft yourself, then use AI to sweep up errors, spot points you missed, or challenge weak reasoning. AI operates on the *review* end, not the *creation* end.

Benefits:
- Minimal behaviour change required — process stays the same, AI adds value at review stage
- Human learning is preserved — you think as you write
- Hallucination risk is lower — AI isn't generating substantive content

Practical applications in this model: consolidating multi-party comments; interpreting vague partner annotations ("expand on this", "?"); checking grammatical consistency; prompting consideration of issues not yet addressed.

> *AI in the driving seat of the thinking risks creating a document the author cannot defend or interrogate. AI at the review stage preserves thinking while adding value.*

Note: for templatable work (contracts, standard advice notes), the starting-point problem is different and the above doesn't directly apply — see the provenance and consistency sections above.

---

## Related Notes
- [[knowledge-management-in-law]] — The knowledge foundation AI needs to work on
- [[legal-tech-strategy]] — Process before tech; same principle applied more broadly
- [[ai-productivity-and-hidden-costs]] — The risks of using AI to write rather than to assist writing
- [[ai-process-design]] — Process models 1–4A for AI-human collaboration; accuracy thresholds
