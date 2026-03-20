# print() and Silent Code

*Lesson 1*

**Keywords:** `print()` · `output` · `silent execution` · `logs`

---

**YOU'LL HEAR THIS WHEN** *you're in a bug investigation or technical post-mortem*

A developer says: *"I just need to add a print statement and see what's coming through."* Or: *"The logs aren't showing anything."*

You might be a product manager, customer success lead, or operations manager sitting in on a debugging session. They're not doing something rudimentary — they're making the invisible visible.

---

**DEV-TO-ENGLISH** *translation layer*

*"The logs aren't showing anything"* → the code is running, but nothing is being explicitly surfaced. It's not broken — it's silent. Someone needs to add output.

---

**QUESTIONS WORTH ASKING** *when something 'isn't working' and no one knows why*

→ "What does the output actually show at that point?"

Signal: you understand that behaviour and visible output are two separate things. This is the question a technically-aware non-developer asks.

---

**SO WHAT?** *the one-line reason this matters to you*

When developers talk about 'logging' or 'checking the output,' they're not doing busywork — they're doing what all programmers do when something runs silently and they need to see inside it.
