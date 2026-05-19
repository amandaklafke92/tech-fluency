# Lesson 04 — Loops

**Keywords:** loop, for loop, iteration, range, list, API, inputs, epoch

---

## Concepts covered

### 1. What a loop is and why it exists

A loop lets you write an instruction once and repeat it across a collection of things — rather than writing the same line ten times.

Without a loop:
```python
print(1)
print(2)
print(3)
# ... ten lines total
```

With a loop:
```python
for number in range(1, 11):
    print(number)
```

Same output. Two lines instead of ten.

### 2. Anatomy of a for loop

```python
for number in range(1, 11):
    print(number)
```

- `for` — keyword that starts the loop
- `number` — a variable Python fills in fresh each pass (first pass: 1, second pass: 2, etc.)
- `in` — connects the variable to the sequence
- `range(1, 11)` — the sequence to loop through; goes up to but *not including* 11
- Indented line — the instruction to repeat

### 3. Loops in real use: the Claude API example

The most concrete use case: you have a list of things and want to apply the same instruction to each one automatically.

```python
companies = [
    'Retail chain with 500 stores, wants to automate inventory reports',
    'Law firm, wants to summarise contracts faster',
    'Hospital network, wants to triage patient intake forms',
]

for company in companies:
    print('Sending to Claude:', company)
    print('---')
```

In a real version, the `print` line would be replaced by an API call — passing each company description to Claude and receiving a response. The loop handles the repetition; the API call handles the communication.

---

## Real-world grounding

**You'll hear this when:** a developer says *"we're iterating over the dataset"* — they mean a loop is going through each item in a collection and doing something to it.

**Dev-to-English:** *"We're just iterating over the results and filtering by confidence score"* = we're going through each result one by one and skipping the ones the model wasn't sure about. A loop with an `if` statement inside it.

**In AI specifically:** when a model is trained, it loops through the training data thousands of times. Each full pass is called an **epoch**. *"We ran it for 10 epochs"* = the loop ran 10 times over the full dataset.

**What non-technical people usually get wrong:** loops feel like conditionals — checking if something is true. They're not. A loop doesn't test anything; it just works through a collection in order.

**API / rate limits:** when someone says *"we hit the API rate limit,"* they usually mean a loop was calling Claude (or another service) too fast — too many requests in too short a time. Anthropic caps how frequently the door can be knocked on.

**So what:** loops are the mechanism underneath any automation at scale — bulk document processing, personalised outreach, model evaluation across a dataset. You don't need to write them, but knowing they exist explains *why* batch processing takes time and why scale changes the conversation.

---

## Spaced repetition notes

- Parameter vs argument — still shaky. Revisit naturally in L5.
- Loop vs conditional distinction — introduced but not drilled. Worth a quiz question in L5.
- API concept introduced informally — not assessed. Revisit when relevant.

---

## Format note

This lesson was run in the Cursor terminal (Claude Code) rather than a separate interface. The learner found it moderately interactive — the live code output helped but the concepts still felt somewhat abstract. Consider a more grounded real-world scenario as the entry point in future lessons before moving to syntax.
