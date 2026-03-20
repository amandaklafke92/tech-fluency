# Lesson 3 — Conditionals

**Keywords & Concepts**
`if` · `elif` · `else` · `conditional` · `Boolean check` · `comparison operators` · `==` `!=` `>` `<` `>=` `<=`

---

## Opening Quiz — Retrieval Practice

Results from Lesson 2 recall (5 minutes, no notes — fastest yet):

- **Defining vs. calling** — perfect. Defining = writing the instructions. Calling = running them. Recipe card analogy now fully owned.
- **Return values** — excellent, with a full real-world example built independently: `len()` checking password length, `print()` delivering the error message downstream. Joined-up thinking.
- **Parameter vs. argument** — correct. Also independently connected parameters back to variables and DRY without prompting.

> 📌 Spaced repetition: `print()` output location came up naturally and correctly in Q2 — 'deliver an error message to the UI' shows it's starting to feel right rather than just be remembered. Good sign. Continue reinforcing organically.

> 💡 Side note: learner noticed that a parameter is also a variable — both labels describe it correctly from different angles. Parked for now, will revisit when context makes it feel natural rather than abstract.

---

## Learning Outcomes

By the end of this Lesson, you can:

- Explain what a conditional is and why it exists
- Write a basic `if` / `elif` / `else` structure in Python
- Explain what a Boolean check is and how it connects to the Boolean data type
- Use comparison operators correctly and know what each one means
- Explain why order matters in `if` / `elif` / `else`
- Read a short conditional block and trace what it will do

---

## Part 1: What Is a Conditional?

### The Concept

A conditional is an 'if this, then that' instruction. Python checks whether something is true, and runs different code depending on the answer. Every condition resolves to a Boolean — True or False — which is why Booleans matter.

> 💡 Your definition before being taught: *"A conditional is something that occurs due to something else having occurred — an if this, then that scenario."* Spot on.

### The Syntax

```python
if age >= 18:
    print("You can vote.")
```

- `if` — the keyword that starts the conditional
- `age >= 18` — the condition: something Python evaluates as True or False
- `:` — the colon means 'then' — here comes what to do if this is true
- The indented line — the body: runs only if the condition is met

> 💡 Your insight: *"The colon is essentially saying then."* Exactly right. Hold onto that.

### The Boolean Check

Every time Python evaluates a condition, it performs what's called a Boolean check — it resolves the condition to either True or False, then decides what to run. You arrived at the term 'Boolean check' independently before it was introduced. That's the right term. Developers also say 'Boolean test' — both are used.

---

## Part 2: if / elif / else

### The Structure

Python gives you three keywords for handling different paths:

```python
if age >= 18:
    print("You can vote.")
elif age >= 16:
    print("You can vote in some elections.")
else:
    print("You can't vote yet.")
```

- `if` — check this first
- `elif` — short for 'else if': if the first wasn't true, check this next
- `else` — if nothing above matched, do this. No condition needed — it's the catch-all

### Your Intuition (Correct ✓)

Before `elif` was introduced, you independently wrote two separate `if` conditions to handle both cases. That works — but `elif` is the cleaner, more Pythonic version. Same logic, better structure.

### Why Order Matters

Asked why order matters, you reasoned it out: *"If you put else before elif, elif is discarded — it would've already run the previous conditional, which would render the elif redundant."* Exactly right.

The rule: `if` must come first, `elif` must come before `else`, `else` must come last. `else` is a catch-all with no condition — Python has nowhere to go once it hits `else`, so anything after it would be unreachable.

---

## Part 3: Comparison Operators

### The Full Set

```python
age == 18    # equal to
age != 18    # not equal to
age > 18     # greater than
age < 18     # less than
age >= 18    # greater than or equal to
age <= 18    # less than or equal to
```

> ⚠️ The one that catches everyone: `==` means 'are these equal?' Single `=` means 'store this value.' Two completely different jobs. Python will not warn you if you use the wrong one — the logic will just behave unexpectedly.

The only one that felt new: `!=` for 'not equal to'. The rest mapped naturally to existing maths knowledge.

---

## Bringing It All Together

The password checker you invented in Lesson 2, now written properly with everything from Lessons 1, 2, and 3:

```python
password = "cat"

if len(password) >= 8:
    print("Password accepted.")
elif len(password) >= 6:
    print("Password weak — consider making it longer.")
else:
    print("Password too short. Minimum 6 characters.")
```

That's `len()`, a return value, a conditional, `elif`, `else`, and a comparison operator — all in six lines. Everything from Lessons 1, 2, and 3 working together.

---

## Questions from This Lesson

### "Is a parameter also a variable?"

Yes — both labels are correct, describing different things. It's a variable because it's a named container storing a value. It's a parameter because of the specific role it plays — sitting in the function definition as the input slot. All parameters are variables. Not all variables are parameters. Parked for now — will feel more natural with more context.

### "Would you call it a Boolean check rather than a Boolean search?"

Boolean check is exactly right — and you landed on it before being told. Developers say 'Boolean check' or 'Boolean test.' Both are standard. 'Boolean search' isn't a term used in this context.

---

## Big Ideas to Hold Onto

- A conditional is if this, then that. Python checks a condition, gets True or False, and runs the matching block.
- `if` / `elif` / `else` must always appear in that order. `else` is the catch-all — no condition, just 'everything else.'
- Every condition is a Boolean check — it resolves to True or False. That's your Boolean data type from Lesson 1 doing its job.
- `==` means 'are these equal?' Single `=` means 'store this value.' Different jobs, easy to confuse.
- `!=` means 'not equal to' — the one operator that didn't map to prior maths knowledge.
- Everything connects: data types → variables → functions → return values → conditionals. Six lines of code can use all of it at once.

---

**Next Lesson:** Loops — making code repeat actions, and combining repetition with conditionals.
