---
name: chunk-for-retention
description: Breaks down long or complex material -- book chapters, articles, lectures, research papers, arguments, study notes -- into a small number of meaningful macro-chunks, grounded in John Sweller's Cognitive Load Theory and the working-memory research it builds on (Miller, Cowan, Baddeley & Hitch, Chase & Simon). Use this skill whenever the user wants help remembering, studying, summarizing, or outlining a book/chapter/article for retention; asks about chunking, cognitive load, working memory limits, study techniques, or note-taking strategies; wants a compact map of an argument's structure; or is writing educational/learning-science content that discusses chunking or cognitive load theory -- even if they never say the word "chunking" themselves.
---

# Chunk for Retention

## The problem this solves

Working memory can only hold a handful of things at once -- somewhere around four meaningful units, not forty (Cowan, 2001, refining Miller's earlier "seven plus or minus two," 1956). When a reader tries to hold thirty loose sentences in mind while also trying to understand what they add up to, most of that limited capacity gets spent just keeping the pieces from falling off the desk. Nothing is left over for the actual work of understanding.

Sweller's Cognitive Load Theory splits the load on working memory into two practical categories:

- **Intrinsic load** -- the load that comes from the real complexity of the material itself. You can't remove this without removing understanding.
- **Extraneous load** -- the load that comes from *how* the material is presented or organized, not from what it actually means. This is the load worth cutting.

Chunking is the main tool for cutting extraneous load without touching intrinsic load. It works by re-grouping many small, weakly-related units into fewer, larger units that are strongly related to each other internally (this is Gobet & Simon's definition of a chunk). Because working memory counts *chunks*, not raw elements, a reader holding "4 argumentative moves" in mind has more room to actually think than one holding "40 sentences" -- even though the underlying content is identical. This is the same mechanism Chase & Simon (1973) found in chess experts: masters don't remember more squares than novices, they recognize more meaningful *configurations* of squares.

Apply this to any material the user wants to study, remember, or summarize for retention -- not just "book chapters" narrowly. Lecture notes, research papers, meeting transcripts, and long arguments in an email thread all qualify.

## Workflow

1. **Read the whole source before chunking anything.** Chunking requires seeing the overall shape first; chunking sentence-by-sentence as you go produces structural groups (by paragraph or heading), not meaningful ones.

2. **Ask "what job is this doing?", not "what does this say?"** For each stretch of text, identify its function in the larger argument or narrative: does it state a problem, present evidence, give an example, rebut an objection, propose a solution, draw an implication, introduce a complication? Content that shares a function belongs in the same chunk, even if it's scattered across several paragraphs.

3. **Target 3-6 macro-chunks.** This range sits inside working memory's real capacity (~4±1 chunks, per Cowan 2001). If a first pass produces more than ~7, the chunking isn't finished -- find the next level up and group chunks into chunks (see "Scaling to longer material" below).

4. **Give each chunk a label that carries meaning, not a placeholder.** "Part 1" forces the reader to re-derive the content every time they recall it. "Diagnoses the housing crisis with data" doesn't -- the label itself is a usable memory cue. Aim for labels the user could recite from memory and still reconstruct the point.

5. **State the connective logic between chunks, not just the chunks.** Add a short phrase showing how one chunk leads to the next (contrast, cause, extension, response). Retention depends on remembering the *shape* of the argument, not a list of disconnected facts -- this is what separates chunking from an ordinary bullet-point summary.

6. **Cut extraneous load; protect intrinsic load.** Strip filler, throat-clearing, and redundant restatement. Do not flatten real complexity, technical distinctions, or caveats just to shrink the chunk count -- that trades comprehension for a smaller number, which defeats the purpose. If a topic is genuinely dense, it's fine for a chunk's *expansion* to run longer, as long as the chunk *label* stays compact.

7. **Close with a retrieval check.** Ask the user to restate the chunk labels from memory, or quiz them on the connective logic, before moving on. Chunking organizes information for storage; retrieval practice is what actually consolidates it into long-term memory -- pair the two rather than treating a well-organized chunk list as the finish line.

## Output template

Use this shape by default; adapt as needed for the material:

```markdown
# [Title of the chapter / article / argument]

**Core chunks (N):**

1. **[Meaningful label]** -- one-sentence expansion.
   ↳ [how this leads into the next chunk]
2. **[Meaningful label]** -- one-sentence expansion.
   ↳ [how this leads into the next chunk]
3. **[Meaningful label]** -- one-sentence expansion.

**The thread:** [one sentence tying all chunks into the overall argument]

**Recall check:** Can you restate these N chunks, in order, without looking?
```

## Worked example

**Input:** A ~40-sentence chapter that (1) cites housing-price statistics, (2) profiles one family's experience, (3) quotes an economist, (4) describes government policy, (5) shows a chart, plus ~35 more sentences of supporting detail.

**Output:**

```markdown
# Chapter 3: The Housing Squeeze

**Core chunks (4):**

1. **Diagnoses the crisis with data and a human face** -- statistics and one family's story establish that housing costs have become unaffordable.
   ↳ raises the question of why this happened
2. **Explains the cause via expert testimony** -- an economist attributes the rise to supply constraints and financialized ownership.
   ↳ sets up an evaluation of the response so far
3. **Critiques the existing policy response** -- current government measures are shown to be inadequate or misdirected.
   ↳ motivates the author's own proposal
4. **Proposes an alternative** -- the author argues for a specific policy shift, anticipating the main objection to it.

**The thread:** The chapter moves from "here's the problem" to "here's why" to "here's what's not working" to "here's what should happen instead."

**Recall check:** Can you restate these 4 moves, in order, without looking?
```

Four chunks instead of forty sentences -- and the four chunks preserve exactly the thing worth remembering: the argument's shape.

## Scaling to longer material

For book-length material, chunk twice, hierarchically:

1. Chunk each chapter into 3-5 moves (as above).
2. Chunk the chapters themselves into 3-5 higher-level "parts" (e.g., "sets up the problem" / "builds the case" / "answers objections" / "calls to action").

This mirrors how experts actually build knowledge: chunks that get reused become automated and can themselves be treated as a single element inside a bigger chunk (schema construction). Don't try to build the second-level chunking until the first level is solid -- holding both levels in mind before either is internalized just recreates the original overload problem.

## Common pitfalls

- **Over-chunking.** More than ~7 chunks isn't a finer-grained summary, it's a working-memory overload wearing a chunking costume. Regroup.
- **Structural chunking instead of meaning-based chunking.** Splitting by paragraph, heading, or page is not chunking -- it's just re-slicing at a different size. Group by function, not by layout.
- **Generic labels.** A label like "Section 2" gives the reader nothing to hang recall on. The label has to do real memory work on its own.
- **Flattening intrinsic complexity to hit a smaller number.** If a genuine technical distinction gets lost in the chunking, that's a comprehension cost, not a win -- only extraneous load should be cut.
- **Chunking material the reader has no foothold in.** Chunking helps most once the reader has some prior schema for the domain; a total novice may need a few key terms pre-taught before chunking the argument actually helps (related to the *expertise reversal effect* -- see references). Gauge roughly how familiar the user already is with the topic before over-scaffolding.

## Going deeper

For the fuller research background -- working memory capacity estimates, the original three-part cognitive load model and its 2019 revision, the expertise reversal effect, and adjacent Cognitive Load Theory techniques (worked examples, split-attention, redundancy, modality effects) -- read `references/research-foundations.md`. Load it when the user wants the theory explained or cited (e.g., they're writing an article about the technique), not when they just want a piece of text chunked.
