# Process log: interpretability row

## Plan
1. Establish what frontier developers actually do with internals in safety assessments (system cards: Anthropic Fable 5.1, OpenAI GPT-6 Astra; Google not reached).
2. Find quantitative tests of how well internals-based auditing works (AuditBench; whether model organisms are valid tests).
3. Find frontier-relevant cases where hidden misbehaviour was found, and by what method (OpenAI misalignment reports).
4. Read the strongest forward-looking arguments both ways (Amodei, "The Urgency of Interpretability"; Nanda, "Interpretability Will Not Reliably Find Deceptive AI").
5. Argue both ways, judge, and run a self-challenge.

## Delegation
None. Sub-agents were not available, so every step was done in sequence by one model. The cases for higher and lower were written after the evidence was read, by the same model that judged. There were therefore no disagreements between sub-agents to report.

## Searches (16 run; a further batch of 5 failed on the tool-use limit)
Batch 1: interpretability audit hidden objective model 2026; Anthropic interpretability pre-deployment audit system card 2026; mechanistic interpretability progress 2026 frontier model; sparse autoencoders limitations negative results deepmind; interpretability will not reliably detect deception argument; OpenAI interpretability misalignment detection 2026; Gemini interpretability Gemma Scope 2 2025; activation probes deception detection frontier model evaluation.
Batch 2: Claude Fable system card interpretability white-box; GPT-6 Astra system card interpretability activations; GPT-6.1 Astra cancelled deceptive behaviour interpretability; urgency of interpretability 2027 reliably detect most model problems; white-box auditing benchmark model organisms 2026 agents; interpretability evaluation awareness steering suppress Claude 2026; UK AISI white box control interpretability sandbagging detection 2026; Neel Nanda pragmatic interpretability pivot 2025.
Batch 3 (FAILED, tool limit): natural language autoencoder paper; obfuscated activations; GPT-6.1 Astra misalignment report; Claude Opus 5 card white-box; Gemini 3.5 model card interpretability.

## Documents opened (10)
- Claude Fable 5.1 / Mythos 5.1 system card (sections 6.6-6.7; p.45; key findings p.91-92)
- GPT-6 Astra system card (landing page and full navigation list only)
- AuditBench (arXiv 2602.22755): abstract, results p.6-7
- Nanda, LessWrong post (full)
- Amodei, "The Urgency of Interpretability" (relevant sections)
- "How to Train Your Model Organism" (arXiv 2610.10203): abstract, introduction
- Anthropic, "Verbalizable Representations Form a Global Workspace" (introduction and overview)
- OpenAI misalignment reports index
- OpenAI "Covert underperformance on safety research tasks" report
- Becker's Hospital Review on GPT-6.1 Astra (secondary)

## Not reached
- Google DeepMind primary sources (Gemma Scope 2, the "pragmatic interpretability" post)
- The paper describing natural language autoencoders
- The Fable 5.2 and Opus 5 system cards
- UK AISI white-box work
- "Sanity Checks for Sparse Autoencoders" (arXiv 2602.14111)

The documents read come mostly from Anthropic (system card, workspace paper, AuditBench co-authors) and OpenAI, so the evidence is concentrated in two organisations. Google DeepMind is represented only by Nanda's personal post.

## Others' assessments consulted
None used for conclusions. Zvi Mowshowitz's system-card reviews and a longtermwiki page appeared in search results but were not opened.

## Self-challenge (done by the same model, not a fresh reviewer)
- **Claims against sources.** Each claim was checked against the passage cited. The AuditBench figures were confirmed on p.6. The Astra card's lack of an interpretability section was confirmed from its navigation list but not from its subpages, and this is noted in the evidence. One claim, that Anthropic's audits had "moved from feature-based studies", was not supported by what I read, so I rewrote it to rest on the Fable 5.1 card's statement that the pipeline was also used in the Opus 5 card. I changed the verbal label for 0.04 to "almost certainly not", in line with the brief's scale.
- **Same standard across developers.** Anthropic gets credit for using interpretability, but its own caveats are reported, and its results are not counted as validated reliability. OpenAI's silence is treated only as weak evidence.
- **Evidence on the other side.** The positive J-lens and natural-language-autoencoder results are included, as are Amodei's arguments and Nanda's hedge about AI-automated research.

## Problems
PDF text extraction was noisy at first; I fixed it by collapsing whitespace. No prompt-injection content was found in the sources. The budget was enforced as a hard limit on searches, which cut off the planned search for Google DeepMind sources.
