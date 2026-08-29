# Research Foundations: Chunking and Cognitive Load Theory

This file expands on the research behind the chunk-for-retention skill. Read it when the user wants the theoretical grounding explained (e.g., they're writing an article about the technique, not just asking for a chapter to be chunked), or when a chunking decision needs to be justified against the literature.

## Working memory capacity

- **Miller (1956), "The Magical Number Seven, Plus or Minus Two."** The original, widely-cited estimate that short-term/working memory holds about seven meaningful units. This paper is also the origin of the term "chunk" in this literature: recoding many small units into fewer, larger meaningful units increases the effective amount of information held, even though the number of *chunks* stays roughly constant.
- **Cowan (2001), "The Magical Number 4 in Short-Term Memory."** A later, more carefully controlled estimate (using tasks that prevent rehearsal and grouping strategies) puts real capacity closer to about four chunks, not seven. This is the number worth designing around in practice -- it's why the main skill targets 3-6 chunks rather than up to seven.
- **Baddeley & Hitch (1974), the multi-component working memory model.** Splits working memory into a phonological loop (verbal/acoustic information), a visuospatial sketchpad (visual/spatial information), and a central executive that coordinates them. Relevant in practice: text and diagrams draw on different subsystems, which is part of why the split-attention effect (below) matters -- chunking purely verbal material doesn't automatically help a reader who also has to make sense of an accompanying chart.

## Chunking and expertise

- **Chase & Simon (1973), chess memory studies.** Chess masters could reconstruct a mid-game board almost perfectly after a brief glance; with randomly-scattered, non-game-legal pieces, their recall dropped to roughly the same level as novices. The masters weren't remembering more *pieces* -- they were recognizing familiar *configurations* (chunks) built from thousands of hours of pattern exposure. This is the classic demonstration that chunking capacity in a domain is a learned, acquired skill, not a fixed trait.
- **Gobet & Simon**, in later work formalizing chunking theory, define a chunk as a set of elements with strong internal associations to each other and weak associations to elements outside the chunk -- a useful practical test for deciding where chunk boundaries belong in a text: put the boundary where the internal connections weaken.

## Cognitive Load Theory (Sweller)

- **Sweller (1988), "Cognitive Load During Problem Solving: Effects on Learning."** The foundational paper. Introduces the idea that instructional design should be evaluated by how much of the learner's limited working memory it consumes on things that aren't the material itself.
- **The original three-part model** distinguished:
  - *Intrinsic load* -- inherent to the material's complexity and the learner's existing expertise in the domain (the same material is higher intrinsic load for a novice than for an expert).
  - *Extraneous load* -- imposed by how the material is presented; wasted load that instructional design should minimize.
  - *Germane load* -- load devoted to actually building schemas (learning), originally treated as a third, separate quantity to be maximized.
- **Sweller, van Merriënboer & Paas (2019), "Cognitive Architecture and Instructional Design: 20 Years Later."** A significant revision: germane load is no longer treated as a separate load category, but as the productive redirection of *freed-up* working-memory capacity toward intrinsic processing, once extraneous load has been cut. In this updated view, chunking doesn't add a third kind of load -- it simply reduces extraneous load and thereby leaves more room for intrinsic (germane) processing to happen. This is the version of the theory the main skill assumes.

## The expertise reversal effect

- **Kalyuga, Ayres, Chandler & Sweller (2003), "The Expertise Reversal Effect."** Instructional supports that help novices (worked examples, heavy scaffolding, and by extension aggressive chunking) can measurably *slow down* or clutter processing for learners who already have relevant expertise, because the support now duplicates knowledge the expert already holds as an automated schema -- adding redundant load instead of removing extraneous load. Practical implication: check the user's existing familiarity with a topic before chunking hard; a lighter touch may serve an expert reader better than a maximally-compressed chunk structure.

## Adjacent Cognitive Load Theory effects worth pairing with chunking

- **Worked example effect** -- showing a fully solved example before asking someone to solve a similar problem reduces load for novices, compared to discovery-first approaches. Relevant when chunking instructional or technical material that contains procedures, not just prose arguments.
- **Split-attention effect** -- when related text and a diagram, chart, or table must both be held in mind to make sense of either, keep them physically adjacent. Separating them (e.g., a caption on one page, the chart on another) forces the reader to spend working memory just searching and holding, on top of understanding.
- **Redundancy effect** -- presenting the same information twice in different forms at the same time (e.g., a diagram that is also fully narrated in prose) adds load rather than reducing it, because the reader has to reconcile two channels saying the same thing. A chunked summary should replace redundant detail, not sit alongside it as an extra restatement.
- **Modality effect** -- when material genuinely needs both a visual and a verbal channel, splitting them across visual and auditory modalities (e.g., a diagram plus spoken narration) uses two separate working-memory subsystems (per Baddeley & Hitch) instead of overloading one.

## Retrieval practice as chunking's natural partner

- **The testing-effect literature (Roediger & Karpicke and related work).** Chunking is a storage and organization strategy -- it changes how information is structured, not whether it has been consolidated into long-term memory. Actively retrieving information (being quizzed, restating from memory) produces more durable retention than re-reading the same well-organized material, even when re-reading feels more fluent at the time. This is why the workflow in SKILL.md ends every chunking pass with a recall check rather than treating a well-organized chunk list as the finish line.
