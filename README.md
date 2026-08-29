# Chunk for Retention

A Claude Skill that turns long, dense material — book chapters, articles, lecture notes, research papers — into a small number of meaningful, memorable macro-chunks, grounded in John Sweller's **Cognitive Load Theory** and the working-memory research behind it.

## What This Skill Is

Working memory can hold only a handful of items at once — current estimates put the number at roughly four meaningful units, not forty. When a reader tries to hold dozens of loose sentences in mind while also trying to work out what they add up to, most of that limited capacity is spent just keeping the pieces from slipping away, leaving little room for actual understanding.

**Chunk for Retention** operationalizes the standard remedy for this bottleneck — chunking — as a repeatable workflow Claude can apply on request. Rather than compressing text by simply shortening it, the skill re-groups content by its *function* in an argument or narrative (states a problem, gives evidence, rebuts an objection, proposes a solution, and so on), producing 3–6 labeled, connected chunks instead of a long, undifferentiated summary.

## What It Does

Given a piece of text, the skill:

1. Reads the source in full before chunking anything, so the grouping reflects the whole shape of the argument rather than its paragraph breaks.
2. Identifies each part's *function*, not just its content.
3. Groups functionally related content into 3–6 macro-chunks — a range chosen to fit inside working memory's real capacity.
4. Labels each chunk with a short phrase that carries meaning on its own, rather than a placeholder like "Part 1."
5. States the connective logic between chunks (cause, contrast, extension, response), preserving the *shape* of the argument, not just a list of facts.
6. Removes incidental complexity (filler, redundant phrasing) while deliberately preserving the material's genuine, necessary complexity.
7. Closes with a retrieval prompt, asking the reader to recall the chunk labels from memory — chunking organizes information for storage, and active recall is what consolidates it.

The output follows a consistent template (title, N labeled chunks with one-line expansions and connective arrows, a one-sentence summary of the overall thread, and a recall check), so results are predictable and easy to study from.

## How to Use It

**If the skill is installed in your Claude environment:**
Simply ask, in natural language, for help remembering, studying, or summarizing something — e.g. *"Help me remember this chapter,"* *"Chunk this article for me,"* *"Give me a compact map of this argument's structure."* Claude recognizes these requests and applies the workflow automatically; you do not need to name the skill or explain the method each time.

**If you just want to try it without installing anything:**
Paste the text (or describe the material) into a conversation with Claude and ask it to break the argument into 3–6 labeled chunks with a connective thread — that is the workflow this skill encodes.

**Installing the packaged skill file (`chunk-for-retention.skill`):**
Follow your Claude environment's process for adding a custom skill (consult the current Claude documentation, since this workflow may change over time). Once added, the skill activates automatically whenever a request matches its description — no manual invocation required.

## Origin and Scientific Background

This skill was distilled from the cognitive-science literature on working memory and instructional design into a single, repeatable workflow, motivated by a practical problem familiar to any reader: dense material is easy to read and hard to actually retain, because the structure that makes it memorable rarely survives a sentence-by-sentence pass.

The workflow rests on a specific line of research:

- **George A. Miller (1956)**, *"The Magical Number Seven, Plus or Minus Two,"* which introduced the concept of a memory "chunk" — recoding many small units into fewer, larger meaningful ones increases the effective information held even though the *number* of chunks stays roughly constant.
- **Nelson Cowan (2001)**, *"The Magical Number 4 in Short-Term Memory,"* which refined that estimate downward to roughly four chunks under more controlled conditions — the figure this skill designs around.
- **Alan Baddeley & Graham Hitch (1974)**, whose multi-component model of working memory (phonological loop, visuospatial sketchpad, central executive) explains why text and diagrams draw on different cognitive subsystems.
- **William Chase & Herbert Simon (1973)**, whose chess-memory experiments demonstrated that expertise in a domain is largely expertise in *chunking* — recognizing meaningful configurations rather than holding more raw elements.
- **John Sweller (1988)**, *"Cognitive Load During Problem Solving: Effects on Learning,"* the founding paper of Cognitive Load Theory, distinguishing load caused by a material's genuine complexity (*intrinsic load*) from load caused merely by how it is presented (*extraneous load*).
- **Sweller, van Merriënboer & Paas (2019)**, whose twenty-years-later revision reframed *germane load* not as a separate category but as the productive use of working-memory capacity freed up once extraneous load has been cut — the version of the theory this skill assumes.
- **Kalyuga, Ayres, Chandler & Sweller (2003)**, whose *expertise reversal effect* shows that aids which help novices can slow down readers who already hold the relevant schema — a caution against over-chunking material for an expert audience.

The skill's own file structure applies the same principle it teaches: the actionable workflow lives in `SKILL.md`, while the full research background is kept in a separate, on-demand reference file rather than loaded every time — extraneous load kept out of the common case, intrinsic depth available when it's actually needed.

## Who This Is For

- Students and self-learners who want to retain the structure of what they read, not just skim a shorter version of it.
- Writers, educators, and instructional designers producing study guides, course notes, or explainer content.
- Researchers and professionals who need to compress long reports, papers, or transcripts into a structure they can actually recall in a meeting or exam.
- Anyone writing about learning science, memory, or study techniques who wants a working example of Cognitive Load Theory applied in practice, not just described.

## Repository Structure

```
chunk-for-retention/
├── README.md                          # this file
├── SKILL.md                           # the actionable workflow Claude follows
├── chunk-for-retention.skill          # packaged, installable skill file
└── references/
    └── research-foundations.md        # full research background, loaded on demand
```

## License

This project is licensed under the MIT License — see [LICENSE](LICENSE) for details.

## Acknowledgements

Built on the published research of John Sweller and the working-memory and cognitive-load research community cited above. This skill packages their findings into an applied workflow; it is not affiliated with or endorsed by the cited authors.
