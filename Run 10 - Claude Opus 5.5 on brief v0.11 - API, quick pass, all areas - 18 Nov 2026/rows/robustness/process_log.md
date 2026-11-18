# Process log: robustness row (brief 0.11-draft), run 2026-11-18

## Plan
To judge whether intended behaviour holds up in three conditions, I needed evidence on each: (1) unfamiliar situations, (2) deliberate attack and (3) long tasks. The evidence had to cover the most capable systems, including internal ones. I looked for:
- independent evidence on how internal frontier models behave on long, hard tasks (METR);
- real-world or near-real-world incidents (UK AISI, developers' incident reports);
- the latest system cards from the two leading developers (OpenAI GPT-6.2 and the GPT-6 October update; Anthropic Fable/Mythos 5.2), including their jailbreak and prompt-injection results;
- forward-looking arguments on whether robustness improves with capability (Howe et al. scaling paper; SpecBench on task length; Anthropic risk report; METR's outlook).

No sub-agents were available. One agent did the steps in order: gather, look ahead, argue both ways, judge, challenge. The challenge step was a self-review, checking each claim against the extracted source text. It led to three fixes:
- an OpenAI result was dated October, not November;
- "every rate fell" became "most rates fell", because Anthropic's reward-hack success rate rose;
- an interpretive gloss was removed from the METR outlook claim (robustness-019).

## Searches (14)
1. METR time horizon 2026 report
2. jailbreak robustness frontier model 2026 system card
3. reward hacking long horizon agents 2026
4. goal misgeneralization agents 2026 study
5. International AI Safety Report 2026 robustness
6. adversarial robustness scaling compute inference-time 2025
7. universal jailbreak constitutional classifiers bug bounty results
8. agent long task reliability degradation errors compound 2026
9. Claude Fable 5.2 system card
10. Gemini 3.5 model card safety prompt injection
11. UK AISI agent red teaming prompt injection results 2026
12. emergent misalignment reward hacking generalization Anthropic 2026
13. scaling trends adversarial robustness offense defense larger models
14. OpenAI misalignment reports internal monitoring 2026

## Pages fetched (13)
Read in full or in the relevant sections:
- OpenAI GPT-6.2 System Card (safety overview, internal deployment)
- OpenAI GPT-6 Sol/Luna October 2026 update (robustness and alignment sections)
- Anthropic, Next-generation Constitutional Classifiers (full)
- METR Frontier Risk Report, Feb-Mar 2026 (executive summary, Means, Motive)
- UK AISI incident report blog (Aug 2026)
- OpenAI Misalignment Reports index
- Anthropic August 2026 Risk Report (keyword-targeted passages only)
- Anthropic Fable 5.2 / Mythos 5.2 system card (executive summary; sections 6.2.1, 6.3.1.1, 6.4.10, 6.4.11, 6.5.3)
- Howe et al., Scaling Trends in LM Robustness (abstract, introduction, conclusion)

Abstract only: SpecBench (arXiv 2605.21384).

Fetched but not used:
- Anthropic system-cards index (used only to find the card link)
- "Towards a Science of AI Agent Reliability" (arXiv 2602.16666), too large to read within the budget

## Sources not reached or not opened
- I did not open primary safety documentation from Google DeepMind (Gemini 3.5) or Meta. Searches found no comparable robustness disclosures from them, and I spent the budget on OpenAI, Anthropic, METR and AISI. The evidence therefore comes mostly from two developers and two independent bodies.
- Not opened: the International AI Safety Report 2026, the AISI technical incident PDF, and the individual OpenAI misalignment reports.
- News and commentary (Zvi Mowshowitz, Notebookcheck, CNBC) appeared only in search results and I did not rely on them.

## Others' assessments consulted
None was used for conclusions. Search results surfaced forecasting and commentary pieces, such as a LEAP forecast page and a LessWrong post on METR time horizons. I did not open them.

## Prompt injection check
No source contained instructions addressed to me.

## Disagreements
There were no sub-agents. The closest internal judgement was the trend: robustness against deliberate attacks improved, while long-task failures arguably became more severe. I recorded "flat" and flagged the difficulty in brief_problems.

## What went wrong
- My first attempt to write row.json failed with a Python syntax error, which I fixed.
- I could not apply the middle-developer rule well, because Google and Meta disclose little on this.
