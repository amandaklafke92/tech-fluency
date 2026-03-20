# Python Vocabulary — Lesson 2

*Functions*

> **How to use this:** This is the Lesson 2 addition to your running glossary. Add it alongside your Lesson 1 terms for a complete reference.

---

| Term | Type | Definition & Example |
|---|---|---|
| **Function** | *noun* | A named, reusable block of code that does a specific job. You define it once and call it as many times as you need. The DRY principle applied to actions, not just values. |
| **def** | *keyword* | Short for "define". The keyword that tells Python you're about to describe a function. Always followed by the function name and parentheses. `def greet():` |
| **Define** | *verb* | Writing out what a function does — its name, input slot, and body. Defining a function does not run it. It's writing the recipe card, not following it. |
| **Call** | *verb* | Actually running a function by writing its name followed by parentheses. Until you call a function, nothing happens. `greet()` |
| **Parameter** | *noun* | A variable inside a function's parentheses that acts as a placeholder for input. Makes the function flexible — the same function can produce different results depending on what's passed in. `def greet(name):` |
| **Argument** | *noun* | The actual value you pass into a function when you call it. The parameter is the placeholder; the argument is the real thing. In `greet("Amanda")`, `"Amanda"` is the argument. `greet("Amanda")` |
| **Built-in function** | *noun* | A function Python provides out of the box — you don't need to write it yourself, just use it. `print()`, `len()`, and `type()` are all built-in functions. `len("Amanda")` |
| **User-defined function** | *noun* | A function you write yourself using `def`. You choose the name, the parameters, and what it does. `def greet(name):` |
| **Return value** | *noun* | What a function sends back after doing its job. Not all functions return something — `print()` just displays and disappears. `len()` returns a number you can catch and use. `result = len("Amanda")` |
| **len()** | *built-in function* | Returns the number of characters in a string (or items in a list). Always returns an integer. `len("Amanda")  # 6` |
| **Conditional** | *noun* | A piece of logic that says: if this condition is met, do this; otherwise, do something else. You described this independently this session — we'll cover it properly next time. `if length < 8: ...` |
| **Indentation** | *noun* | The spaces at the start of a line inside a function (or other block). Python uses indentation to know which lines belong to which block. Get it wrong and the code breaks. |
