# Teaching Framework

---

> 💡 **What is this?** A self-directed Python and tech literacy course for a non-technical professional — built lesson by lesson with Claude — to develop enough fluency to communicate confidently with developers and understand the AI landscape. Not about becoming a programmer. About becoming fluent.

---

## Core Philosophy

### Learning Approach

- **Intuition-first where possible:** Before explaining a concept, prompt the learner to reason through the "why" themselves. Only explain after they've had a chance to guess.
- **Analogies over jargon:** Always reach for a plain-English analogy before technical terminology. Linguistics background is an asset — language-based framings work well.
- **Purpose before mechanics:** Learner responds well to understanding *why* something exists before learning *how* it works. Lead with purpose, but sometimes flip it and ask the learner to figure out the why themselves.
- **Short lessons, clear stopping points:** Each lesson covers 2–3 concepts maximum. End before the brain gets full.

### Making the Abstract Tangible

Some concepts don't stick until they have something tangible to attach to. When a concept feels abstract or slippery, try one of these techniques:

- **Anchoring (location/structure):** Give the concept a physical or spatial home. *Where does this live in the code? How does it relate to what's around it?* Works especially well for structural concepts — how code is organised, where definitions sit relative to calls, how files relate to each other. When the learner asked "where does a function definition actually go?", the concept of defining vs. calling became immediately more concrete and easier to hold. Spatial thinking is also how developers actually think — so this isn't just a memory aid, it's building a genuine mental model.
- **Analogy:** Map the concept onto something already familiar. Works best for abstract mechanics (e.g. def = writing a recipe card; calling = following it). Already built into the core approach, but worth naming explicitly as a concretising tool.
- **Real-world consequence:** Show what goes wrong when the concept is misunderstood or ignored. Particularly effective for data types, DRY, and return values — things where the cost of getting it wrong is tangible.
- **More to add as they emerge** — this list will grow as new techniques surface in lessons.

**On timing:** The quiz/retrieval phase is often the best moment to introduce a concretising technique — not the lesson itself. When a learner reaches for something and feels the gap, the anchor has somewhere to land. During the lesson, new information is the priority and an additional frame can be one thing too many. That said, some anchors (especially locational/structural ones) are worth building into the lesson from the start when the location *is* the point.

**Safeguard:** Don't wait for the learner to ask the right question. During retrieval, if there's a gap or a concept feels shaky, proactively ask: *"Do you have a sense of where this lives in the code, or how it relates to the things around it?"* — then apply whichever concretising technique fits the concept.

---

## How It Works: Lesson Structure & Grounding

### The lesson flow

1. **Opening quiz** — Retrieval practice on previous lesson's concepts (off the top of the head, no notes first)
2. **New concepts** — 2–3 topics, taught with intuition prompts and analogies
3. **Real-world grounding** — After each concept (or at natural moments), anchor it in professionally relevant context using the formats below. Inspired by Kahneman's *Thinking, Fast and Slow* chapter-end phrase guides — primes recognition and builds workplace confidence, not just technical recall.
4. **Lesson plan doc** — Generated as a .docx at the end of each lesson, including a Keywords block at the top
5. **Glossary update** — New vocabulary added to the running glossary .docx
6. **Field Guide update** — Real-world grounding content added to the running Field Guide doc, organised by concept

### Real-world grounding formats

Use 3–5 of these per concept, chosen for relevance. Always open with an orienting line: who is saying this, what role the learner is likely in, and what the situation is (e.g. *"You're in a sprint planning meeting as a PM and a developer says..."*).

- **"You'll hear this when..."** — a specific phrase someone might say, with context: who's saying it, what role the learner is in, what situation they're in
- **"You might say this when..."** — the flip side: a phrase the learner could use to signal fluency, framed around realistic scenarios (a meeting, an interview, a check-in)
- **"Dev-to-English translation"** — what a developer *means* vs. what it sounds like to a non-technical ear; useful for decoding conversations in real time
- **"What a non-technical person usually gets wrong about this"** — common misconceptions the learner can now quietly hold correctly
- **"In an interview, if asked..."** — how to deploy the concept when discussing past experience, answering a question with tech language sprinkled in, or demonstrating awareness
- **"So what" summary** — one sentence answering: why does a non-developer need to know this at all?
- **"Questions worth asking"** — 1–2 smart questions the learner could now ask in a relevant conversation (adapt to whoever they'd realistically be talking to — not always a developer)

---

## Course Documents

- **Lesson plans** (per lesson) — concepts, outcomes, questions, quiz notes. Keywords block at top. Includes real-world grounding content embedded in context, where it serves as a learning aid during and after the lesson.
- **Glossary** (per lesson + master) — vocabulary with definitions and code examples, updated each lesson. Per-lesson glossaries live inside each lesson folder; a master `GLOSSARY.md` compiles all terms across lessons.
- **Field Guide** (running) — real-world grounding organised by concept, not lesson. For pre-meeting and pre-interview skimming. Contains the same grounding content as the lesson plans, reformatted for quick reference rather than learning context.

> 💡 The Field Guide and lesson plans intentionally share content. The lesson plan is the learning context; the Field Guide is the reference layer. Same material, two reading modes.

---

## What's Working (& How We're Learning)

### Real-time observations

- Intuition-testing questions are building learner confidence in her own reasoning
- Learner explicitly said she struggles to trust her instincts — the mini self-assessment format is helping with this
- Corrections land better when framed as a "small tweak" rather than a wrong answer
- Anchoring (asking where something lives) converted a shaky concept into a solid one mid-quiz — worth applying proactively, not just reactively

### Spaced repetition strategy

- Track quiz results each lesson and flag shaky concepts for natural reinforcement in future lessons — not immediately, but woven into upcoming lessons organically
- **lesson 1 quiz (tested in lesson 2):** `print()` output location still fuzzy — doesn't feel concrete yet. Variable concept solid (reasoned independently). Data types solid but same "where does output go" question applies.
- **lesson 2 quiz (tested in lesson 3):** Functions — defining vs. calling gap filled during retrieval using anchoring (location question). Parameters not yet tested this lesson.
- The Excel analogy (formula runs silently, you only see what it chooses to display) landed well for `print()` — use similar framings going forward.

---

## Course Roadmap

**Language:** Python

**Goal:** AI/tech fluency for a non-technical professional — not to code, but to communicate confidently with technical people and understand the AI landscape

**Roadmap:**

1. Foundations — `print()`, variables, data types ✅
2. Making things happen — functions, loops, conditions
3. Reading and writing data — files, APIs
4. AI-specific literacy — models, training, prompts in code
