# Learning Journal

*One entry per lesson. Written at the end — not a summary of what was taught, but a reflection on how it landed. What clicked? Was there a moment where something suddenly made sense? Anything still slippery? This is your record of what it felt like to learn this, not just what you learned.*

*Note: Lessons 1–3 entries were written by Claude based on session observations. From Lesson 4 onwards, entries are written by the learner.*

---

## Lesson 4 — Loops — May 2026

*Written by Claude — learner asked me to write this one.*

Loops felt abstract for most of the lesson — the syntax and the flashcard analogy didn't fully land. The right instinct came from the learner: asking for the *why* before the mechanics. The Claude API example (loop through companies, send each to Claude) helped orient things but still didn't fully click at the code level.

The sharpest thinking came after the lesson content ended. When asked whether an agent could just do the job of a script, the learner immediately started reasoning about the abstraction layers between scripts, skills, and agents — correctly placing skills as the plain-English equivalent of a script, and correctly noting that skills define what, how, *and* constraints (not just what). Also identified that agents don't improvise from scratch — they read and orchestrate available skills. That's a sophisticated mental model, arrived at independently.

The terminal format was fine but didn't add much over a normal lesson — the live code output was mildly useful but the abstractions didn't become more concrete just because the code was running in front of her.

**What clicked:** the agent/script/skill abstraction ladder; that loops are the mechanism underneath any automation at scale; API as "the door between two pieces of software"

**Still slippery:** loop syntax itself; parameter vs argument (still fuzzy); the loop-vs-conditional distinction (a loop doesn't test, it works through — this didn't fully land)

**For next lesson:** open with a loop vs conditional quiz question; find a more grounded entry point before syntax — the real-world scenario should come first, not third

---

## Lesson 3 — Conditionals — March 2026

Fastest quiz yet — defining vs calling now fully owned, return values excellent with independent real-world example. Parameter = variable observation was sharp — parked for later. Conditionals clicked quickly, especially the colon = "then" insight. Password checker brought everything from Lessons 1–3 together in six lines — satisfying moment. Boolean check term arrived independently before being introduced.

**Concepts to keep reinforcing:**
- `print()` output location — feeling more natural, continue organically
- Parameter = variable — revisit when contextually natural

---

## Lesson 2 — Functions — March 2026

Defining vs calling gap filled during retrieval using anchoring (location question). Parameters clicked via the "different flavours, same recipe" analogy. Return values landed well — vending machine analogy worked. Independently described a conditional before it was introduced (password length checker).

**Concepts to keep reinforcing:**
- `print()` output location — still not fully concrete, revisit naturally

---

## Lesson 1 — Introduction to Python — March 2026

First lesson. `print()` core idea solid but output location fuzzy. Variables reasoned independently from scratch — strong. Data types solid. Excel analogy (formula runs silently, you only see what it chooses to display) landed well for `print()`.

**Concepts to keep reinforcing:**
- `print()` output location — needs to become concrete through real context
