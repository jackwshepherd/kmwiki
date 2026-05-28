---
title: "Prototypes and Disposable Apps"
---

# Prototypes and Disposable Apps

**Summary**: Production-grade standards only matter if the software gets into the real world with dependent users. Prototypes and disposable apps are the two cases where vibe coding genuinely shines — with caveats.
**Tags**: #vibe-coding #prototypes #disposable-apps #legal-tech #law-firms
**Created**: 2026-05-27
**Last Updated**: 2026-05-27

---

## When Production Grade Doesn't Matter

The case against vibe coding as a path to production software is real (see [[vibe-coding]]). But this is only a problem if the software gets out into the real world with users who depend on it. Two situations where it doesn't matter: **prototypes** and **disposable apps**.

---

## Prototypes

A prototype is a *learning vehicle*. You build one when you've exhausted your ability to learn without something tangible. It purposefully falls short of production grade — because you don't want to spend too much time and effort creating something that might not be worthwhile in the first place.

**Example:** Dictator — a hybrid dictation and editing app harnessing LLMs and voice detection to structure thoughts into written work-product. Vibe coded quickly, discovered within hours (not weeks) that the fundamental approach was flawed. Even a failed prototype generates useful learning. In this case: formatting of text was a problem, and a simple markdown interface was probably better than rich text.

Prototypes are excellent for:
- Validating ideas
- Drawing out niche requirements you wouldn't have thought of abstractly
- Discovering what questions to ask

### Beware the Vanity Project

Prototypes can go sour when they stop being prototypes. The obsessive-building pattern: start with a core idea → add a feature → then another → then another → then another. Each individually feels like progress. Collectively, the purpose has shifted.

Dictator became a vanity project: post-it notes, AI grouping, AI renaming, AI content writing, a new ideas-structuring tab. The thrill was in the building, not in the having-built. No plans to sell it or release it. Used briefly, then reverted to old habits.

> *How many vibe-coded solutions on social media are legitimate learning vehicles? How many will be used by more than one person? How many are really just delivering a short-term dopamine hit?*

Tinkering is great. You have to tinker to learn. Just don't kid yourself that you're going to change the world.

### Beware the Marketing Tool

A well-designed vibe-coded app is almost indistinguishable from production software. Until it isn't.

This has always been a problem with Figma mockups — realistic, clickable, non-functional screenshots dressed up to look like working software. The same risk applies to vibe-coded prototypes used as sales or marketing tools.

Rules for showing prototypes:
1. Be explicit that it is a prototype
2. Be explicit that it doesn't exist as working software

If you're not explicit on both, people will assume it's production-ready. When they discover it isn't, they won't trust you again.

---

## Disposable Apps

A disposable app is: made for me, by me, used once, then never again.

**Example:** A taxonomy remapping tool. Painful in Excel, no off-the-shelf solution, not worth building properly given the time horizon. Perfect candidate for vibe coding because:

- **Local** — runs locally, no database, everything in the browser, nothing leaves the computer
- **Discrete task** — used once for a specific purpose, then never again. Limited time window for things to go wrong
- **Small user base** — used by one or a handful of people; if there are errors, vibe code your way out without impacting anyone
- **Backup plan** — at all times, can export to Excel and continue the old way

The stakes are low enough that perfection doesn't matter.

### The Strategic Opportunity for Law Firms

Lawyers are going to realise how easy it is to make disposable apps for mundane tasks: document renaming, information extraction, taxonomy mapping, bespoke data formatting. They'll want custom workflow layers that get data exactly in the shape they need it.

The question for law firms is how to *manage* this surge. Left unmanaged: a bunch of half-baked and overpromised solutions. Managed properly: allow lawyers to experiment, ideate, and improve how they work.

> *Firms that don't have a strategy around this will unconsciously drift into years of cleanup work around apps they don't even know exist.*

---

## The Two-Track Model

| Who | Use case |
|-----|----------|
| Software engineers | Use vibe coding to assist in making production-grade software |
| Everyone else | Use vibe coding to prototype ideas and make disposable solutions |

Both are legitimate. The problem is when the second group forgets which track they're on.

## Related Notes
- [[vibe-coding]] — What makes software actually production grade
- [[ai-productivity-and-hidden-costs]] — The obsession spiral: how prototypes become vanity projects
- [[legal-tech-strategy]] — Law firm strategies for managing the surge in new tools
