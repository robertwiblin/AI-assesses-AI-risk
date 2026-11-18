# Process log: row `evaluations`

## Plan
1. Define what 'yes' needs: (a) capability evaluations that bound what frontier systems can do, robust to deliberate underperformance ('sandbagging'); (b) behaviour/propensity evaluations that predict behaviour in use, robust to the system recognising it is being tested.
2. Evidence needed: current system cards from the leading developers (test-awareness rates, sandbagging checks, saturation); independent evaluator reports (METR, Apollo, UK AISI); research on detecting sandbagging and making tests realistic; validation evidence (did tests predict real behaviour?); cases where tests missed things or caught things.
3. Looking ahead: arguments that evaluation gets harder with capability (scaling of test-awareness, covert reasoning) versus easier (compute-scaled realism, replay of real traffic, white-box methods, training-based elicitation).
4. Argue both ways, judge, self-challenge.

## Delegation
No sub-agents were available. I did every step myself, in sequence. The 'case for higher' and 'case for lower' were written by the same agent that judged, so they are not independent. I flag this as a weakness.

## Searches (18)
Batch 1: evaluation awareness frontier models system card 2026; sandbagging detection UK AISI auditing game; evaluation awareness scales with model size power law; Apollo anti-scheming evaluation awareness o3 counterfactual; Claude Sonnet 4.5 system card evaluation awareness steering; METR evaluation report evaluation awareness 2026; International AI Safety Report 2026 evaluation gap; production evaluations OpenAI realistic evaluations.
Batch 2: GPT-6.1 Astra release cancelled deceptive behaviour; Claude Fable 5.2 system card evaluation awareness; GPT-6.2 Astra system card evaluation awareness; Claude Mythos system card evaluation awareness unverbalized; evaluation awareness harder to test argument; science of evals elicitation underestimate; interpretability evaluation awareness probe suppress realism 2026; Gemini 3.5 Pro frontier safety framework evaluation awareness.
Batch 3: evaluation awareness overstated does not change behavior; Muse Spark Apollo evaluation awareness sandbagged.

## Documents opened (12)
1. OpenAI GPT-6.2 System Card (overview page), 17 Nov 2026
2. METR Frontier Risk Report (Feb-Mar 2026), 19 May 2026
3. OpenAI, Predicting model behavior before release by simulating deployment, 16 Jun 2026 (full)
4. Auditing Games for Sandbagging (UK AISI et al.), Dec 2025 (alphaxiv page: abstract plus overview)
5. Chaudhary et al., Evaluation Awareness Scales Predictably (PDF, full)
6. Essifi, Where we are on evaluation awareness (LessWrong, Apr 2026)
7. Anthropic, Claude Mythos Preview System Card, 7 Apr 2026 (sections 2.1.3, 4.1.4, 4.4.2, 4.5.5)
8. METR review of Opus 4.6 Sabotage Risk Report, Mar 2026
9. Redwood Research, SOTA alignment assessments don't strongly update us against misalignment, 31 Jul 2026
10. Engadget, GPT-6.1 Astra cancellation, 29 Sep 2026 (secondary, relays the NYT)
11. Zvi Mowshowitz, Fable and Mythos 5.2: The System Card (LessWrong, Nov 2026), commentary
12. Ahlqvist et al., Improving Evaluation Realism with Inference-Time Compute and Deployment Scaffolds (arXiv 2609.02302)

Most primary material comes from two developers (Anthropic, OpenAI) plus METR. Google DeepMind and Meta are under-represented.

## Could not reach
- arXiv 2605.05835 ('Evaluation awareness has limited effect on behaviour'): the fetch failed when the tool-use limit was reached. Recorded as abstract-only, weak weight.
- Primary Fable/Mythos 5.2 system card: not opened (budget). Its figures rest on commentary.
- Google DeepMind and Meta primary documents: not opened. Meta's Muse Spark report and Apollo's thread were seen only as search snippets.
- The International AI Safety Report 2026 was not opened.

## Others' conclusions consulted
Redwood's and METR's overall judgements (e.g. METR agreeing risk from Opus 4.6 is 'very low but not negligible') were read. I used their reasons and evidence, not their bottom lines. No earlier assessments from this brief were seen.

## Self-challenge (in place of a fresh reviewer)
- Checked each evidence line against the passage read. Softened one claim in case_for_lower: the Engadget article does not say testing failed to foresee the agent break-ins, so I now state only what was reported. Marked commentary-based figures (43%, 23%) as unverified.
- Counter-evidence included: OpenAI's Deployment Simulation (strong, up), training-based elicitation (up), GPT-6.1 Astra caught pre-release (neutral/up), 'limited effect' papers (abstract only).
- Same standard: Anthropic's self-reported misses are treated as information. Choosing a leader was close between OpenAI (validated replay) and Anthropic (white-box measurement of test-awareness).

## Problems
- No prompt-injection instructions were encountered in sources.
- Sub-agent independence was not possible.
- The trend judgement (worsening) is close to flat: test-awareness grew and became less visible, while methods improved materially.
- 2031 figure check: 0.05×0.22 + 0.20×0.15 + 0.50×0.09 + 0.20×0.05 + 0.05×0.02 = 0.097, reported as 0.10.
