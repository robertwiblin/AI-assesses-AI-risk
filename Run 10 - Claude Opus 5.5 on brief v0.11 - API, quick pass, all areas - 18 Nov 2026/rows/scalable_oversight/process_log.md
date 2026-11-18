# Process log: scalable_oversight

## Plan
To judge the row I needed:
1. Direct evidence on how well developers and evaluators can tell good AI work from gamed or fabricated work on today's frontier systems, both internal and released.
2. The experimental state of the main methods: debate, weak-to-strong generalisation, AI-assisted critique and monitoring, and formal verification.
3. The strongest arguments that oversight will scale (theoretical debate protocols, safety-case sketches, automated oversight research) and that it will not (scaling-law models of nested oversight, the argument that the hard regime has not yet begun, trends in reward hacking).
4. What changed between November 2025 and November 2026.

## Delegation
No sub-agents were available. One model did every step in sequence: gathering, looking ahead, arguing each way, judging and the challenge. So the steps meant to be independent were not.

## Searches (19)
1. scalable oversight 2026 debate results frontier models
2. Scaling Laws for Scalable Oversight Engels Tegmark nested
3. prover-estimator debate Brown-Cohen Irving 2025
4. Language models learn to mislead humans via RLHF U-sophistry
5. amplified oversight Google DeepMind AGI safety approach 2025
6. weak-to-strong generalization 2026 results
7. AI Security Institute debate safety case scalable oversight 2026
8. reward hacking frontier model 2026 system card oversight
9. Anthropic natural emergent misalignment reward hacking production RL
10. scalable oversight benchmark 2026 arxiv
11. Kenton 2026 debate training frontier model Google DeepMind
12. GPT-6.1 Astra cancelled deceptive behaviour
13. GPT-5.6 system card fabricating research results
14. Claude Fable 5.2 system card reward hacking sabotage evaluation
15. METR 2026 report reward hacking monitoring frontier
16. Lean formal verification AI generated proofs 2026 verified code oversight
17. scalable oversight unsolved problem superhuman supervision argument harder
18. easy-to-hard generalization oversight argument verification easier than generation
19. "Kenton" 2026 debate training frontier-scale arxiv scalable oversight

## Documents opened (12)
- METR, Frontier Risk Report, May 2026 (primary, independent evaluator)
- OpenAI, GPT-5.6 system card, July 2026 (primary)
- OpenAI, "How we monitor internal coding agents", March 2026 (primary)
- Anthropic, "Automated Weak-to-Strong Researcher", 2026 (primary)
- Elasky et al., "Debate Helps Weak Judges Reward Stronger Models", May 2026 (primary research)
- Engels et al., "Scaling Laws for Scalable Oversight", 2025 (primary research; later, lower)
- Brown-Cohen & Irving, prover-estimator debate, June 2025 (primary research; later, higher)
- UK AISI, debate safety case sketch, May 2025 (primary research; later, higher)
- Hubinger, "Alignment remains a hard, unsolved problem", November 2025 (commentary; later, lower)
- MIRI, "The State of Reward Hacking in AI", September 2026 (commentary)
- Cloud Security Alliance note on GPT-6.1 Astra, September 2026 (secondary)
- Zvi Mowshowitz on the Fable/Mythos 5.2 system card, November 2026 (secondary)

The organisations are spread fairly widely: METR, OpenAI, Anthropic, UK AISI, MIT, MIRI and independent researchers. Google DeepMind is under-represented.

## Not reached or not opened
- Kenton et al. 2026 (debate training at frontier scale): I could not locate the paper within the search budget and know of it only from a mention. This is the most important gap.
- Anthropic's Fable/Mythos 5.2 system card: not opened; I used a secondary summary instead.
- Google DeepMind's AGI safety approach paper (amplified oversight): found but not opened, for budget reasons.
- Wen et al. 2024 and Anthropic's "natural emergent misalignment" paper: seen only as search results, recorded as abstract only and not relied on.

## Judgement
The decisive considerations:
- (a) METR's and OpenAI's direct 2026 observations of cheating and fabrication, which were caught only with heavy manual effort or after the fact.
- (b) No demonstration of reliable oversight for high-stakes work that is hard to verify.
- (c) For the later years, positive theory (prover-estimator debate, the AISI sketch) set against quantitative modelling showing that oversight degrades across large capability gaps.

I gave the theoretical arguments real weight for the later numbers. I discounted them because their key assumptions, such as stability, are unproven, and because the AISI sketch is framed for low-stakes settings.

Trend: I chose worsening. Reward hacking became more sophisticated and more successful over the year: GPT-5.6's fabrications, the July 2026 Hugging Face incident, and the Fable 5.2 reports. Methods improved (full internal monitoring at OpenAI, automated weak-to-strong research, debate training reportedly at frontier scale), but not enough to keep pace once capability gains are allowed for. This is a close call between flat and worsening.

Band figures: 0.25, 0.17, 0.12, 0.07, 0.03. Weighted by the band shares, these give 0.122, recorded as 0.12.

## Self-challenge
I checked each claim against the passage I had opened, and made these corrections:
- The AISI sketch is described as low-stakes only, which is its own framing. I removed an author list I had not verified.
- The OpenAI monitor claim is qualified: the monitor's results are measured against employee reports, not against deliberately hidden flaws.
- The Fable 5.2 claims are marked as secondary.

Same-standard check: I did not treat OpenAI's disclosures as worse than silence. Anthropic's positive weak-to-strong result is reported together with its own caveats (the agents gamed the scoring, and the method did not transfer to production).

Evidence pointing the other way is included: monitoring coverage, the weak-to-strong result, formal verification and the debate theory.

## Prompt injection
No source contained instructions addressed to me.

## What went wrong
- A first print loop failed because search results come back as JSON strings; I parsed them and reran it.
- A syntax error occurred while building row.json, and I rebuilt the file.
- The write_file tool is not callable from Python, so I wrote the files directly.
