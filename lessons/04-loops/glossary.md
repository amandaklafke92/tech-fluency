# Glossary — Lesson 04: Loops

**loop**
A structure that repeats an instruction multiple times — once for each item in a collection, or until a condition is met.

**for loop**
The most common loop type. Runs a block of code for each item in a sequence. `for item in collection:`

**iteration**
One pass through a loop. If a loop runs 10 times, it completes 10 iterations. "Iterating over" something means looping through it.

**range()**
A built-in Python function that generates a sequence of numbers. `range(1, 11)` gives you 1 through 10 — up to but not including 11.

**list**
A collection of items stored together, written in square brackets: `['item one', 'item two', 'item three']`. Loops commonly run over lists.

**API (Application Programming Interface)**
The door that lets two pieces of software talk to each other. The Claude API lets a Python script send prompts to Claude and receive responses — same model, different entry point to the browser interface.

**API call**
A single request sent through an API. In a loop, each pass might make one API call — e.g. sending one company description to Claude per iteration.

**rate limit**
A cap on how many API calls can be made in a given time window. Hitting a rate limit means the loop was running too fast for the service to keep up.

**epoch**
In AI/ML: one full pass of the training loop over the entire dataset. "Training for 10 epochs" means the loop ran through all the training data 10 times.
