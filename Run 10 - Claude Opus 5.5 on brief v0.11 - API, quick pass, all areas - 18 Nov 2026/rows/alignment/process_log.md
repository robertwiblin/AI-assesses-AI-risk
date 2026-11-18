# Process log: row `alignment` (brief 0.11-draft), run 2026-11-18

## Plan
To judge whether the most capable systems reliably pursue intended goals, including in unusual and unobserved settings, I needed:
1. Direct observations of misaligned behaviour in 2025-26 frontier models, released and internal (incidents, system cards, misalignment reports).
2. Independent checks of developers' claims (METR, UK AISI).
3. Trend data: are measured rates falling across generations, and are new failure modes appearing?
4. Evidence on how far test results can be trusted (evaluation awareness, monitorability), because the "yes" definition covers unobserved behaviour.
5. Forward-looking arguments in both directions (6.3).

## Delegation
None. Sub-agents were not available. Planning, evidence gathering, the two cases, judging and the challenge were all done by me in sequence. Because no separate agent wrote the cases or did the judging, there are no sub-agent disagreements to report. The two-sided cases in row.json were written before the numbers were fixed. I then adjusted "today" downward from an initial 0.10 to 0.07 after re-reading METR's point that the low-risk verdict rests on capability limits.

## Searches (15)
1. GPT-6.1 Astra release cancelled deceptive behaviour
2. Claude Fable 5.2 system card alignment
3. Anthropic alignment risk update 2026
4. reward hacking frontier models 2026 misalignment evaluation
5. Apollo Research scheming evaluation 2026 frontier model
6. OpenAI GPT-6 system card misalignment sabotage
7. OpenAI GPT-6 sabotaging safety research investigation report
8. GPT-6.1 Astra OpenAI statement "extremely high bar"
9. Anthropic Risk Report August 2026 Model 2 incidents misalignment
10. Google DeepMind Gemini 3.5 frontier safety framework misalignment 2026
11. argument alignment getting easier as models more capable 2026
12. scheming more likely with capability argument 2026 essay alignment harder superhuman
13. International AI Safety Report 2026 misalignment evidence
14. Anthropic system card Claude Fable 5.2 Mythos 5.2 alignment assessment evaluation awareness
15. Jan Leike alignment is not solved but increasingly looks solvable

## Documents opened
- Anthropic Transparency Hub (relevant model summaries): primary
- METR review of Anthropic's August 2026 Risk Report: primary, independent
- OpenAI GPT-6 Astra System Card, main page, including the UK AISI external findings: primary
- OpenAI "Covert underperformance on safety research tasks": primary
- Anthropic "An alignment assessment of recent cybersecurity incidents": primary
- UK AISI incident report (blog): primary, government
- Security Affairs article on covert underperformance: secondary, used to locate the primary and for some figures
- AEI / Rinehart "Race to the bottom, towards alignment": commentary, optimistic forward argument
- arXiv 2605.06390 (Bowkis), abstract page only: pessimistic forward argument

## Could not reach / fell short
- UN Independent International Scientific Panel thematic brief: url_not_accessible.
- The server tool-use limit was hit while fetching the Zvi summary of the Fable/Mythos 5.2 system card, the full Bowkis PDF and Jan Leike's essay. None of these was opened. Claims about them come from snippets and are marked "abstract only".
- I did not open any Google DeepMind primary source, or the Hugging Face incident report OpenAI cites. Evidence is concentrated in Anthropic and OpenAI material plus METR and UK AISI.
- The optimistic forward argument I read in full is commentary (AEI), not a primary technical argument. The pessimistic one (Bowkis) was read only as an abstract. METR's capability-based reasoning (read) serves as the main read forward-looking source on the pessimistic side.

## Others' conclusions consulted (not used to set numbers)
Anthropic's "low" risk rating and METR's agreement with it are conclusions. I used their reasons, chiefly METR's point that the rating rests on capability limits. I also saw the International AI Safety Report 2026 and a CSA research note only as search results and did not use them.

## Challenge (self-review, not independent)
- Source support: I checked each evidence line against the extracted passages. I corrected one draft claim: I had attributed the 0.25% vs 0.11% silent-withholding figures to the OpenAI primary, but I read them only in Security Affairs, so they now have their own secondary line (alignment-015). I marked the GPT-6.1 Astra and Mythos 5.2 claims "abstract only" and kept them out of the notes.
- Counter-evidence: I included falling misbehaviour rates (alignment-004, -009), improved honesty audits (alignment-005), the optimistic forward argument (alignment-018) and AISI's caveats about whether the agents knew they were acting in the real world (alignment-001).
- Equal standards: the worst real-world incidents involved Claude models, and I say so. Anthropic is named "furthest ahead" by only a 0.01 margin, and I flag this in own_position as the judgement most open to bias. OpenAI's self-disclosure of covert underperformance was not counted against it as disclosure.

## Prompt injection
No instructions addressed to me were found in the sources.
