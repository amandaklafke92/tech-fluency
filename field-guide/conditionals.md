# Conditionals

*Lesson 3*

**Keywords:** `if` · `elif` · `else` · `conditional` · `Boolean check` · `comparison operators`

---

**YOU'LL HEAR THIS WHEN** *you're in a product or engineering discussion about feature behaviour*

A developer or PM says: "We need to handle the edge case" or "What happens if the user does X instead?" or "We need to add a guard for that."

You might be in a product review, a QA session, or a bug investigation as a product manager, operations lead, or business analyst. They're describing a conditional — a specific situation that needs its own code path. 'Edge cases' are almost always conditionals someone forgot to write.

---

**DEV-TO-ENGLISH** *translation layer*

"We need to handle that case" → we need an `if` statement for that specific situation.

"There's no guard on that" → there's no conditional checking for a problem before it causes one. The code just runs without checking if the inputs are valid.

"That's falling through to the default" → none of the `if`/`elif` conditions matched, so the `else` block ran — sometimes unexpectedly.

---

**WHAT A NON-TECHNICAL PERSON USUALLY GETS WRONG** *common misconception to quietly hold correctly*

That 'logic errors' are the same as crashes. A missing or wrong conditional doesn't necessarily crash a program — it just makes it do the wrong thing silently. A user gets accepted when they should be rejected, or a discount applies when it shouldn't. The code ran perfectly; it just had the wrong conditions.

---

**QUESTIONS WORTH ASKING** *in a product or QA discussion*

→ "What happens if none of the conditions are met — is there a fallback?"

Signal: you understand that code needs to handle every possible path, not just the expected one. This is the question that catches missing `else` blocks before they become bugs in production.

→ "Is that checking for equality or assignment?" (when something behaves unexpectedly)

Signal: you know the `==` vs `=` distinction — one of the most common sources of silent bugs in conditional logic.

---

**IN AN INTERVIEW, IF ASKED** *about attention to detail or systems thinking*

"I've learned to think about edge cases — not just what the system should do when everything goes right, but what it should do when inputs are unexpected, missing, or out of range. That's essentially conditional logic: defining a path for every meaningful scenario, not just the happy path."

---

**SO WHAT?** *the one-line reason this matters to you*

Conditionals are where software stops being mechanical and starts making decisions. Every feature that behaves differently for different users, every error message, every access control rule — it's all conditionals. Understanding this makes you sharper in conversations about product behaviour, QA, and edge cases.
