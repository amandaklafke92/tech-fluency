# Lesson 2 — Functions

**Keywords & Concepts**
`function` · `def` · `define` · `call` · `parameter` · `argument` · `built-in function` · `user-defined function` · `return value` · `len()` · `conditional` · `indentation`

---

## Opening Quiz — Retrieval Practice

Results from Lesson 1 recall (no notes):

- **print()** — mostly right. Core idea solid. Small gap: output location still not fully concrete ("UI" was too specific). The Excel analogy landed well: formula runs silently, you only see what it chooses to display.
- **Variables** — fully correct, reasoned independently from scratch. Cascade of memory mid-answer. Strong.
- **Data types (number vs string)** — correct. Same "where does output go" nuance applies.

> 📌 Flag for spaced repetition: the idea that `print()` output can appear in many places — not just a UI — needs to become concrete through seeing it in a real context. Will revisit naturally in a future Lesson.

---

## Learning Outcomes

By the end of this Lesson, you can:

- Explain what a function is and why it exists
- Distinguish between defining a function and calling it
- Understand what parameters are and why they make functions flexible
- Tell the difference between built-in functions (like `print`) and user-defined functions
- Explain what a return value is and why it matters
- Describe how return values can be caught and used in further logic

---

## Part 1: What Is a Function?

### The Concept

A function is a reusable block of code that does a specific job. You define it once and call it as many times as you like. It's the DRY principle applied to actions, not just values.

### Syntax

```python
def greet():
    print("Hello, Amanda!")
```

- `def` — short for "define". Tells Python: I'm about to describe a function.
- `greet` — the name you choose. Like naming a variable, but for a block of code.
- `()` — the input slot. More on this below.
- The indented line — the body. What the function actually does.

### Defining vs. Calling

Writing a function does nothing by itself. To make it run, you have to call it:

```python
greet()
```

> 🍰 Analogy: `def` is writing a recipe card. `greet()` is actually following it. The cake doesn't bake itself just because you wrote the instructions.

---

## Part 2: Parameters — The Input Slot

### The Concept

The parentheses are the function's input slot. You feed something in, the function does its job with it. When the parentheses are empty, the function always does the same thing. When they contain a parameter, the function becomes flexible.

### Empty vs. Parameterised

```python
def greet():
    print("Hello, Amanda!")   # always the same

def greet(name):
    print("Hello, " + name + "!")   # flexible

greet("Amanda")   # Hello, Amanda!
greet("Priya")    # Hello, Priya!
greet("Sam")      # Hello, Sam!
```

### Your Intuition (Correct ✓)

*"Variables are like different flavours — same recipe, different ingredient each time."*

Exactly right. A parameter is the flavouring. The function is the cake. Same structure, different result depending on what you pass in.

### When to Use Each

- **No parameter** — when the output is always identical (e.g. a fixed footer, a standard error message, a logo)
- **With parameter** — when the output needs to vary based on input (e.g. personalised greetings, calculations, lookups)

> 💡 Rule of thumb: if a function doesn't need input, don't give it an input slot. Simplicity reduces bugs.

---

## Part 3: Built-in vs. User-Defined Functions

### The Concept

You've been using functions since your very first line of code. `print()` is a function — one Python wrote for you. `greet()` is a function you wrote yourself. The syntax for calling them is identical.

> 🔌 Analogy: `print()` is like a microwave — it came with the kitchen, someone else built it, you just use it. `greet()` is a recipe you wrote yourself — you decide what it does and can change it whenever you want.

### Other Built-in Examples

```python
len("Amanda")   # returns 6 — counts characters in a string
type(28)        # returns int — tells you the data type
```

Same pattern every time: name + parentheses + input. That's all a function call ever is.

---

## Part 4: Return Values

### The Concept

Functions can send something back after doing their job. That's called a return value. It's the difference between a function that just does something and a function that gives you something back to use.

### print() vs. len()

```python
print("Hello!")           # takes something IN, shows it, returns nothing
result = len("Amanda")    # takes something IN, returns 6 back OUT
print(result)             # 6
```

> 🎰 Analogy: like a vending machine. Some machines just flash a light — nothing comes out (like `print`). Others give you something back — a snack, a number, a result (like `len`).

### Why Return Values Matter

If a function just printed something, that value disappears — you can't do anything with it. A return value stays alive in your code. You can catch it in a variable and use it in further logic.

### Your Intuition (Correct ✓)

*"If a password is too short, the length could trigger a print function for an error message."*

Yes — you just independently described a conditional. Here's roughly what that looks like:

```python
password = "cat"
length = len(password)
if length < 8:
    print("Password too short!")
```

> 🚀 That chain — measure something, check it against a condition, trigger another action — is the skeleton of how most real programs work. We'll cover conditionals properly in a future Lesson.

---

## Questions from This Lesson

### "What is print — now that I know greet is a function?"

`print()` is also a function — one Python built for you. You've been using functions since your very first line of code. The only difference between `print()` and `greet()` is who wrote them.

### "Do we need to do anything else in the code to set up def?"

Great instinct to park this rather than lose the thread. Short answer: no — `def` is all you need to start defining a function in Python. There's no setup required before it. We'll come back to the fuller picture when it's relevant.

### "Is a string only alphanumeric characters?"

No — a string is any text inside quotation marks, including spaces, punctuation, symbols, and emojis. The defining feature is the quotes, not the content.

### "Why is it called len?"

Short for length. Programming culture abbreviates things that get typed constantly — `def` (define), `str` (string), `int` (integer), `len` (length). Once you know the pattern, the abbreviations stop looking like typos.

---

## Big Ideas to Hold Onto

- A function is a reusable named block of code. Define it once with `def`, call it as many times as you like.
- Defining and calling are two separate steps. Writing a recipe card is not the same as following it.
- Parameters are the input slot. Empty parentheses = no input. Named parameter = flexible, reusable.
- `print()` and `greet()` are both functions. The only difference is who wrote them.
- Return values let you catch a result and use it elsewhere. `print()` doesn't return anything — it just shows something and disappears.
- Measure → check → act. That chain is the skeleton of most real programs. Coming next: conditionals.

---

**Next Lesson:** Conditionals (if/else) — making code make decisions based on values and logic.
