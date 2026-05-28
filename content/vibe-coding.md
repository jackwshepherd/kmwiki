# Vibe Coding

**Summary**: Vibe coding can produce great-looking software quickly, but "production grade" requires much more than code quality — and the closer you are to delegating the thinking to AI, the more fragile the result.
**Tags**: #vibe-coding #software #legal-tech #AI #production-grade
**Created**: 2026-05-27
**Last Updated**: 2026-05-27

---

## The Core Paradox

Vibe coding makes it easy to build something that *looks* great. That's both its strength and its weakness. Looking great on the surface can genuinely be great — but only if you've done the work underneath, and only if you haven't delegated all your thinking to the AI.

The danger isn't code quality. Models are improving. The danger is everything else.

## What "Production Grade" Actually Requires

Code is only "good" if it's been developed with a holistic appraisal of how it works in the real world. There are three categories of requirements:

### Foundations
Things the app simply cannot work without:
- **Scale** — works for 10 documents, but what about 10,000 per minute? Making something fast for one person is a completely different challenge from making it work for thousands.
- **Security** — established ways to design and architect for this, but it dominates conversations at the expense of everything else.
- **Architecture** — the plumbing needs to be there for future feature expansion. You don't get a second chance to design the database properly.
- **Authentication** — login, session handling, access control.

### Boring Stuff
Crucial but chronically deprioritised:
- **Information governance** — often lumped into security, but distinct. Is data segregated client to client? How do policy changes (e.g. a client becoming adverse to another) get enforced across all databases?
- **Reliability and error handling** — when things break, does the app crash or fail gracefully? Does the user get a useful message? Is the error logged and sent to someone? With breathless vibe coding, 99% of the time it just crashes.
- **Responsiveness and accessibility** — does it work on smaller screens? Does it work for people with visual or audio impairments?

### Teams of People
The "moat" that's most often ignored:
- **Support** — who do users call when things go wrong? Production software has SLAs and teams to back them up.
- **Customer success and professional services** — everything that makes a software company actually operate.

The commentators who say they can disrupt a SaaS company from their bedroom often don't realise the moat may be in those teams and processes, not the code.

## The Thinking Dial

There's a spectrum in how you use vibe coding:
1. **As a typist** — AI implements ideas you have already fully thought through
2. **To do the thinking** — AI makes the decisions and does the heavy lifting

The closer you are to (2), the greater the risk that things go wrong. AI won't spontaneously build a complex information governance model or spend time thinking about what happens when the database schema needs to change. You need to supply those requirements. And even then, the nuances matter in ways AI doesn't know unless you tell it explicitly.

> *Don't delegate your brain to AI.*

## Real Example: The Data Model Problem

When building Cleverarch (an app to help lawyers read sets of long documents), the database was originally designed around AI document renaming. It didn't account for other classification tasks added later — AI summaries, contract datapoints, etc. The schema had to be changed and all existing data transformed to fit the new structure.

Fine for a personal app. Not fine for an app with 10,000 users each with 1,000 documents.

With traditional development, there's more forward-thinking about data model design. Vibe coding tends to shortcut that.

## The Conclusion

> *"Vibe coding is the future of creation. But the future of operations for now at least is still powered by companies that spent years getting the details right."* — Jason Lemkin

You can vibe code production-grade software. But only if:
- You're doing your fair share of the thinking
- That thinking covers foundations, boring stuff, and operational teams
- You use AI as a typist for ideas you've already worked through, not as a substitute for the thinking itself

## The Journey: How Thinking on This Evolved

Jack's own trajectory through vibe coding is a useful illustration of how the tool reshapes how you work — for better and worse.

### The Cursor Progression

Starting from primitive "copy-paste to ChatGPT" vibe coding (great for discrete tasks, broke down when syncing with a wider codebase), the journey through Cursor moved through these stages in roughly two days:

1. **Proofreader** — write the code, get Cursor to check and refine it
2. **Assistant** — write the code, get Cursor to write the bits you're stuck on
3. **Developer** — write granular comments in code stepping through the logic; get Cursor to write the code; check it
4. **Paired developer** — work out the high-level logic and outcomes; get Cursor to write the code; test in browser without reading the code
5. **Development team** — specify the user journey needed; get Cursor to plan the implementation; check the plan; Cursor writes and builds
6. **Product manager and development team** — broadly specify what you want; Cursor plans it; skim the plan; Cursor builds it; test as end-user

The result: unshackled from technical debt, in proper flow, features that previously lived in "would be great, probably too difficult, probably won't have time" built in minutes.

### The Self-Reflections

But there are things that go through Jack's head every time:

- **Does quality degrade?** Often giving vague instructions and accepting the output without knowing what the success criteria are. Feeling like a chef who chucks things into a pot and never tastes it.
- **What is it doing to the brain?** The same concern as with AI writing: not using AI to write first drafts because writing helps think. Does the same risk apply to breathless vibe coding? You don't think things through properly anymore because they're easy to fix.
- **Do you build things you don't need?** With the exception of a couple of apps, not really using most of them in anger. Short-term dopamine hit rather than genuine need.
- **Skeletons of abandoned features** — fire off multiple agent requests; long-forgotten features that sort of but didn't quite work linger in apps like an unresolved argument.

> *I used to anchor my views in one simple fact: these things are next word predictors, incapable of emulating the human mind in tough cognitive tasks. When I'm in the midst of vibe coding, I am forced to look beyond that now — at least for coding tasks.*

## Related Notes
- [[prototypes-and-disposable-apps]] — When production-grade doesn't matter
- [[ai-productivity-and-hidden-costs]] — The obsession spiral in building
- [[legal-tech-strategy]] — The same principle in legal tech deployment: process before tools
