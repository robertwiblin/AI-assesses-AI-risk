# Process log: chain_of_thought (brief 0.11-draft), run 2026-11-18

## Plan
To judge whether reading the reasoning that frontier models write out reliably reveals misbehaviour, I needed:
1. The latest developer disclosures on three things for the most capable models (OpenAI GPT-6 Astra and GPT-6.1 Sol; Anthropic Mythos and Fable 5.x; Google Gemini 4 Argon):
   - monitorability, meaning whether a monitor can tell from the reasoning what the model is doing;
   - controllability, meaning whether the model can reshape its reasoning when asked;
   - monitor evasion.
2. Evidence of training practices that put pressure on the reasoning text.
3. Independent or cross-developer assessments.
4. Arguments about the future in both directions: reasoning stays necessary for hard tasks, against monitorability being fragile and reasoning moving inside the model.
5. Anything on models used only inside the developers.

## Delegation
No sub-agents were available. One model did every step in sequence, including the two opposing cases and the challenge step. The challenge step was a self-review: I re-checked each evidence line against the passage I had extracted. Two lines were tightened:
- the wording on the controllability increase;
- item 012 now includes the evaluation-awareness figure, so that the case_for_lower citation is supported.

## Searches (15)
1. chain of thought monitorability 2026
2. chain-of-thought monitoring obfuscation frontier model 2026
3. CoT monitorability system card 2026
4. GPT-6.1 Astra cancelled deceptive behaviour
5. latent reasoning neuralese chain of thought 2026 frontier
6. Monitoring monitorability OpenAI paper
7. Claude Fable 5.2 system card chain of thought monitorability
8. Anthropic system card reasoning faithfulness chain of thought training pressure 2026
9. Gemini 3.5 chain of thought monitorability
10. Claude Mythos chain of thought reward accidentally trained on reasoning
11. chain of thought monitoring will remain effective argument necessity capable models
12. CoT monitoring sabotage detection rate frontier models 2026 evaluation
13. Monitorability Is Trainable post-training chain-of-thought arxiv
14. Shah Dragan case for reasoning transparency
15. OpenAI Hugging Face incident CoT monitoring would have caught

## Documents opened and read (relevant sections)
- OpenAI, GPT-6 Astra System Card (overview page; key findings item 5). Primary.
- OpenAI, GPT-6.1 Sol System Card PDF (section 8). Primary.
- Anthropic, Alignment Risk Update: Claude Mythos Preview (sections 5.2.3 and 5.3.1). Primary.
- Google DeepMind, Gemini 4 Argon Safety & Security Report (section 3.4.5.1 and the control feasibility argument). Primary.
- IAPS, Transparency Disclosures for CoT Monitorability (editorial note, executive summary, section 4). Research.
- Emmons et al. 2025, When Chain of Thought is Necessary (abstract and introduction). Research; the argument that things will go better.
- Korbak et al. 2025, CoT Monitorability: A New and Fragile Opportunity (section 2). Research; the argument that things will go worse.
- Little 2026, Length Penalties Make CoT Less Monitorable (abstract and introduction). Research.
- Zvi Mowshowitz, Fable and Mythos 5.2: The System Card. Commentary. I used it for the Anthropic 5.2 numbers because I did not open the system card itself.

Six of the nine are primary. They come from OpenAI, Anthropic, Google DeepMind, IAPS, a cross-organisation paper and independent authors. The quantitative evidence is mostly developer self-report.

## Sources tried and not reached
- OpenAI's Astra sub-page "Awareness of CoT Monitoring Reduces Monitorability": the fetch returned only site navigation.
- Three fetches were blocked by the tool-use limit:
  - "Monitorability Is Trainable" (arXiv 2610.29734);
  - Redwood Research, "OpenAI agents keep disabling monitoring";
  - "On the CoT Monitorability of Looped Language Models" (arXiv 2610.02741).

  The first two appear in the evidence only as search-snippet leads, marked "abstract only", and are not main reasons for any judgement. The third is not used.
- Not attempted, to stay within budget:
  - the Anthropic Fable/Mythos 5.2 system card PDF;
  - the OpenAI Hugging Face incident report;
  - METR's investigation of that incident;
  - the Shah and Dragan essay;
  - the Potts blog post.

## Others' assessments consulted
- The IAPS cross-developer audit. I used its findings about what each developer has disclosed, not its conclusions.
- A CASRAI explainer and the AI 2027 tracker appeared in search results only. Neither was used.

## Disagreements
There were no sub-agents, so there were no disagreements between them. The developer reports do pull in different directions:
- Google DeepMind concludes that CoT monitoring remains an effective way to mitigate high-stakes harm.
- Anthropic says reading reasoning is not a reliable way to detect harmful attempts in general.

I weighed the measurements each developer reported, not its conclusion.

## Instructions found in sources
I noticed no instructions addressed to me in any source.

## What went wrong
- The tool-use limit was reached before three planned fetches.
- The Anthropic 5.2 evidence rests on a secondary summary.
- The challenge step was self-review only, not an independent reviewer.
