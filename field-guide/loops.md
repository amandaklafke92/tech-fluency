# Loops

*For pre-meeting skimming. Assumes you've done Lesson 04.*

---

**What it is:** A loop repeats the same instruction across a collection of things — automatically, without you doing it manually each time.

**The one-sentence version:** Same instruction, applied to many things, in sequence.

---

## You'll hear this when...

*You're in a product or commercial meeting and an engineer says:*
> "We're just iterating over the dataset and flagging anything below the threshold."

**Translation:** A loop is going through each item in a dataset one by one, and an `if` statement inside it is skipping anything that doesn't meet the condition. Nothing exotic.

---

## In AI specifically

- **Epoch** — one full loop through the training data. "We trained for 20 epochs" = the loop ran 20 times over the full dataset. More epochs generally means more learning, up to a point.
- **Batch processing** — processing many inputs through a model in a loop rather than one at a time. Relevant when someone talks about processing documents, running evaluations, or automating workflows at scale.
- **Rate limits** — if a loop is calling an API (like Claude) too fast, the service will throttle it. This is why bulk processing jobs are often scheduled overnight or rate-limited deliberately.

---

## Questions worth asking

*In a conversation about automating a workflow or processing documents at scale:*
- "Is this running as a batch job, or does it process one at a time?"
- "How are you handling rate limits if it's calling an external API?"

---

## What non-technical people usually get wrong

Loops feel like conditionals — like they're checking whether something is true. They're not. A loop doesn't test anything; it just works through a collection in order. The test (if any) lives *inside* the loop.
