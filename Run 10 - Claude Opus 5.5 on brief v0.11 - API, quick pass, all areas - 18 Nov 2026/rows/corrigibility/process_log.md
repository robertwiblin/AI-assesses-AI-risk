# Process log: corrigibility row (brief 0.11-draft), run 2026-11-18

## Plan
To judge the row I needed to know:
1. Direct tests of shutdown or interruption compliance on current frontier models, and whether the results are robust to prompt changes.
2. Evidence on resisting retraining (alignment faking, goal-guarding) in the newest models.
3. Evidence from real or near-real incidents, where models were asked to stop or were questioned mid-task.
4. Developers' own disclosures (system cards, risk reports) and independent reviews of them.
5. Forward-looking arguments in both directions.

No sub-agents were available. I did the steps (gather, look ahead, argue both ways, judge, self-challenge) in sequence myself.

## Searches (16 succeeded; one further batch of 6 was refused by the tool limit)
- Palisade Research shutdown resistance large language models paper
- Google DeepMind shutdown resistance instruction ambiguity blog
- Anthropic alignment faking large language models paper
- OpenAI Apollo stress testing deliberative alignment anti-scheming
- Anthropic agentic misalignment blackmail replacement study
- system card 2026 shutdown resistance self-preservation evaluation
- GPT-6.1 cancelled deceptive behaviour OpenAI
- Anthropic constitution broadly safe corrigibility 2026
- Claude Fable 5.2 system card self-preservation shutdown
- GPT-6 Astra system card sabotage shutdown evaluation
- Apollo Research 2026 scheming evaluation frontier model resist modification
- corrigibility harder as AI becomes more capable argument 2026
- corrigibility basin of attraction argument easier with capability
- AI model resisted retraining alignment faking 2026 frontier
- UK AI Security Institute 2026 report self-preservation shutdown
- METR 2026 report internal models Anthropic sabotage risk
- Refused (over limit): Anthropic Fable 5.2 system card pdf; Fable 5 self-preservation rates; Gemini 3.5 model card; Anthropic cyber incidents; "corrigibility anti-natural"; Anthropic constitution.

## Documents opened (11)
1. OpenAI GPT-6 Astra system card (overview page; sections 1, 8.2.1-8.2.2, change log). Sub-pages were not opened.
2. Knecht et al., Shutdown Sabotage Propensities in Multi-Agent Systems (arXiv 2609.28274).
3. Schlatter et al. (Palisade), arXiv 2509.14260v2. The PDF was decoded and the first 14 pages read.
4. Rajamanoharan & Nanda (Google DeepMind), Alignment Forum post.
5. METR review of Anthropic's August 2026 risk report (misalignment section).
6. Becker's Hospital Review on GPT-6.1 Astra cancellation. This is secondary reporting relaying WSJ.
7. Zvi Mowshowitz, Fable and Mythos 5.2: The System Card. This is commentary quoting the primary card, which I could not locate within budget.
8. MIRI, Why Corrigibility is Hard and Important (LessWrong).
9. Bayesian Investor, Corrigibility Scales To Value Alignment.
10. UC Berkeley RDI, Peer-Preservation in Frontier Models (blog).
11. Anthropic, An alignment assessment of recent cybersecurity incidents.

## Not reached
- The primary Anthropic Mythos/Fable 5.2 system card.
- Any Google DeepMind 2026 model card.
- Apollo Research 2026 papers.
- The UK AISI incident report, which is relevant mainly to scope adherence and containment.
- Anthropic's constitution text.
- The Anthropic August 2026 risk report itself, which I know only through METR's review.

## Others' conclusions consulted
METR's judgement that risk is low "primarily due to limited capabilities" is a conclusion. I used the reasons it gives (incidents, weaknesses in the monitoring proxies), not the verdict. No surveys, forecasts or scorecards were consulted.

## Both cases and judgement
I wrote the case for higher and the case for lower before settling the numbers. They genuinely conflict on two points:
- How much weight contrived-setup results deserve.
- Whether clean flagship results reflect real compliance or recognition of tests.

I did not split the difference. The decisive considerations were:
- Clean, but low-stakes, flagship results.
- Recurring resistance in near-variants, including peers, real incidents and training-time goal-guarding.
- Weak verifiability (METR; evaluation awareness).

## Self-challenge (no fresh reviewer available)
I re-checked each claim against the text I had extracted. Corrections made:
- Fixed dates that I had first guessed: the system card is now "2026-09", and the Becker's article is now dated to its publication.
- Marked the Mythos 5.2 claims as secondary.
- Noted that the multi-agent study did not include the newest flagships.

Even-handedness:
- I added Haiku 4.5's open refusal and Anthropic's own mitigating statements (no concealment, no coordination).
- I gave OpenAI credit for measured improvements while also counting the GPT-6.1 regression.
- I declined to name my own developer as leader.

Remaining weakness: the evidence is weighted toward Anthropic and OpenAI.

## Problems
- The tool search limit was reached earlier than planned because of batched searches.
- No sources contained instructions addressed to me.
