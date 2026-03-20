# Lesson 1 — Introduction to Python

**Keywords & Concepts**
`print()` · `output` · `variable` · `string` · `integer` · `float` · `boolean` · `data type` · `DRY` · `syntax` · `bug`

---

## Lesson Overview

| | |
|---|---|
| **Goal** | Build AI/tech literacy and fluency — enough to communicate confidently with technical people, not to become a developer |
| **Language** | Python — dominant in AI/data science, reads like plain English, ideal for these goals |
| **Approach** | Mix of concepts, real-world examples, and intuition-testing questions — sometimes explained, sometimes prompted |

---

## Learning Outcomes

By the end of this lesson, you can:

- Understand what `print()` does and why we need it
- Explain what a variable is and why it's useful
- Identify the four core data types in Python
- Understand why data types matter and what goes wrong when they're confused
- Grasp the core idea that code runs silently — output only appears when explicitly requested

---

## Part 1: print()

### The Concept

By default, code runs invisibly. Nothing appears on screen unless you explicitly tell Python to show it. `print()` is that instruction — it's how you make something visible.

Think of it like a chef cooking in a kitchen. All the work happens behind the scenes. Only what they consciously plate and send out reaches the dining room. `print()` is the decision to plate something.

### Syntax

```python
print("Hello, World!")
```

- `print` — the function (the command)
- `( )` — wrap what you want to show
- `"Hello, World!"` — the text to display. Quotes tell Python: this is text, not a command

### Key Insight

> 💡 `print()` is used constantly, even by senior engineers. When something breaks, the first instinct is still: "let me just print that and see what's in there."

### Where Does Output Appear?

It depends on context:

- In a sandbox or terminal → output box on screen
- In a web app → text on a webpage
- In a background process → a log file a developer checks later

The code and the display are always two separate things. `print()` is your window into the code.

---

## Part 2: Variables

### The Concept

A variable is a named container for storing a value. Instead of repeating information over and over, you give it a name once and refer to it by that name throughout your code.

### Analogy

> 📱 Like saving a contact as "Mum" instead of typing out her number every time. The name is the variable. The number is the value stored inside.

### Syntax

```python
name = "Amanda"
print(name)
print("Hello, " + name + "!")
```

- `name` — the variable (the container)
- `=` — means "store this" (not mathematical equals — think of it as an arrow pointing left)
- `"Amanda"` — the value being stored
- When you `print(name)` without quotes, Python looks up what's in the container and shows it
- `+` joins pieces of text together

### Why It Matters — The DRY Principle

> 🔑 DRY = Don't Repeat Yourself. If a value appears in 50 places and needs to change, a variable means you update it once and the whole program reflects it instantly.

### Your Intuition (Correct ✓)

*"Would the advantage be that you could change the text of the variable in one place and it would apply to all instances in the code?"*

Yes — that's precisely the point. That's the entire reason variables exist.

---

## Part 3: Data Types

### The Concept

Python can store different kinds of things, and it treats them differently depending on what they are. The type of data determines what Python can do with it.

### The Four Core Types

```python
name = "Amanda"      # String — text
age = 28             # Integer — whole number
height = 1.65        # Float — decimal number
is_learning = True   # Boolean — True or False
```

### Why Types Matter

```python
print(1 + 1)     # Output: 2 (maths)
print("1" + "1") # Output: 11 (joins text)
```

The same `+` symbol does completely different things depending on the type. Quotes turn a number into text — Python no longer knows it's a number, just a character on a page.

### Real-World Consequence

> ⚠️ If a user's age is stored as text instead of a number, Python can't subtract it from the current year to calculate birth year. This is one of the most common sources of bugs, even for experienced developers.

### Your Intuition (Correct ✓)

*"Maybe numbers can perform different functions — they might be an instruction within the code, or they can just be there to be displayed?"*

Exactly right. The quotes are telling Python: "don't try to do anything with this, just treat it as something to display." Without quotes, it's something Python can calculate with.

---

## Questions from This Lesson

### "Does print() mean you'll see text somewhere else?"

Not exactly — `print()` just means "make this visible." Where it appears depends on the environment. In a terminal, it's an output box. In an app, it might be a UI element. The point is that without it, nothing appears at all.

### "Are there lots of things in code we don't want to appear?"

It's not that we don't want them to appear — it's that nothing appears by default. All the work happens silently. `print()` is a deliberate choice to surface something. Most code runs and does its job without ever showing you anything directly.

---

## Big Ideas to Hold Onto

- Code runs invisibly. Output is always a deliberate choice.
- Variables let you write something once and use it everywhere — Don't Repeat Yourself.
- Data types determine what Python can do with a value. Quotes = text. No quotes = number Python can use.
- `print()` is your window into what's happening inside your code — beginners and experts use it constantly.

---

**Next Lesson:** Functions, loops, and conditions — making code do things more than once and make decisions.
