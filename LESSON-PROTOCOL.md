# Lesson Protocol

*Instructions for Claude at the start and end of every lesson.*

---

## Start of lesson

1. Read `PROGRESS.md` — check what's been covered, what's next, and spaced repetition flags
2. Read `methodology/teaching-framework.md` — confirm pedagogical approach
3. Run opening quiz based on spaced repetition flags (5 mins, no notes)
4. Proceed with new concepts using intuition-first, analogy-led teaching

---

## End of lesson

Generate the following files:

1. `lessons/NN-topic-name/lesson-plan.md` — Keywords block at top, concepts covered, real-world grounding embedded
2. `lessons/NN-topic-name/glossary.md` — vocabulary for this lesson only
3. `field-guide/concept-name.md` — one file per concept covered, formatted for pre-meeting skimming
4. Updated `PROGRESS.md` — mark lesson complete, update spaced repetition flags

Then close the lesson by prompting the learner to write a Learning Journal entry — what clicked, what felt slippery, any moment where something suddenly made sense.

---

## Ad hoc

- Flag any updates needed to `methodology/teaching-framework.md` at end of lesson

---

## Folder structure and file naming

```
tech-fluency/
├── field-guide/          # one .md file per concept (e.g. loops.md)
├── lessons/
│   └── NN-topic-name/    # e.g. 04-loops
│       ├── lesson-plan.md
│       └── glossary.md
├── methodology/
│   └── teaching-framework.md
├── LESSON-PROTOCOL.md
├── PROGRESS.md
└── README.md
```
