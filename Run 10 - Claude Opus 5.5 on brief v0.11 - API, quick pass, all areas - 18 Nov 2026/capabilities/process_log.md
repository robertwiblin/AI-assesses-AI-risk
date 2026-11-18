# Process log: capability forecast, brief 0.11-draft, run 18 November 2026

Lead agent: Claude (Anthropic), exact version not exposed. All sub-agents are the same model.

## Plan followed

1. Steps 1 and 2 ran in parallel as separate sub-agents. Each received the full brief, unchanged except that section 7 was shortened to "return findings as text with sources", and was told which step was its own.
2. While they ran, the lead read Epoch's ECI data file directly and recomputed the record history and pace.
3. Steps 3 and 4 ran in parallel as separate sub-agents. Each received the same instructions and the same summary of the step 1–2 findings, and neither saw the other's work.
4. The lead then checked the key primary sources personally:
   - Epoch's Bayesian methodology post;
   - METR's Anthropic acceleration assessment;
   - the METR Frontier Risk Report (PDF);
   - Chan et al. (arXiv PDF);
   - Erdil;
   - Epoch's "Can AI scaling continue through 2030?";
   - Epoch's compute-crunch post;
   - Toby Ord;
   - METR Time Horizon 1.1;
   - Engadget (GPT-6.1 Astra);
   - The Motley Fool (capex);
   - The Decoder (GPT-6.2 Astra).
5. Step 5, the forecast, was made by a fresh sub-agent that wrote neither case. It received the brief, an evidence list with ids, summaries of both cases, and lead notes. The notes flagged the capex disagreement between the cases without saying how to resolve it.
6. Step 6, the challenge, went to a fresh reviewer. It received the brief, the draft forecast, the evidence list and the case summaries. It spot-checked 13 claims against sources.
7. The lead revised the forecast in response to the review and wrote the three files.

## Record of sub-agent work

The full sub-agent outputs are kept in the run transcript. Condensed records follow.

### Step 1 (released systems)

**What it found**
- The ECI table and anchors were confirmed against epoch.ai/data/eci_scores.csv. The lead re-checked them independently.
- Record history and pace:
  - 19.4 points per year endpoint to endpoint, 17.2 if starting from o1, and 16.95 on a straight-line fit.
  - Epoch's own trend estimate is 16.6.
- METR time horizons: about 12 hours at 50% success in February–March 2026; GPT-5.6 Sol about 11.3 hours, which METR calls not robust.
- Benchmark figures came mostly from aggregator snippets and are flagged as unverified:
  - FrontierMath Tier 4 reported as saturated;
  - Humanity's Last Exam 55–72% depending on version;
  - conflicting SWE-bench Pro figures.
- AI-in-research figures came via Chan et al. and the METR risk report.

**Activity**
- 14 searches. 10 page attempts, 9 succeeded; the Epoch model page for GPT-6.2 Astra could not be reached.
- No instructions addressed to the agent were found in sources.

**Brief problems it flagged**
- past_pace depends on the start date.
- The "floor" is uncertain because Epoch revises scores.
- It is unclear how to treat partner-only tiers.

### Step 2 (unreleased systems)

**What it found**
- METR measured the internal frontier about 2 months ahead in February–March 2026, measured against "publicly documented" systems, which included the partner-only Mythos Preview.
- Anthropic has internal Models 2–4 and is holding models "slightly longer".
- OpenAI withheld GPT-6.1 Astra; reports of a training pause are unconfirmed.
- An internal OpenAI maths model is reported in secondary sources only.
- Anthropic's internal exploit-chain model is reported in secondary sources only.
- Gemini 3.5 Pro was delayed but behind, showing that withheld does not always mean ahead.
- UK AISI blog.
- Estimate of the internal lead: 3 months (80% range 1–7).

**Activity**
- 15 searches; 8 pages read.
- Failed: CNBC, the Epoch Brief, and the Epoch X post (tool limit).
- No instructions were found in sources.

**Brief problems it flagged**
- The brief presupposes that internal models are ahead.
- "Released" differs from "publicly documented".

### Step 3 (slower case)

**The case**
- Reinforcement-learning gains are exhausted (Ord; You).
- Capex growth peaks in fiscal 2026 (FactSet).
- A compute crunch (Epoch).
- The METR acceleration finding is fragile: redacted, and 0.99x on public data.
- Possible compute–labour complementarity (Whitfill & Wu, abstract only).
- Benchmark saturation; financial correction; pauses.
- Implied ECI: about 204 at end-2028 and about 228 at end-2031.

**Activity**
- 14 searches; 6 pages read.
- Could not open Erdil or Epoch-2030 (tool limit). The lead later read both.

**Notes**
- It flagged honestly that Ord's and You's warnings have been wrong on timing so far.

### Step 4 (faster case)

**The case**
- The pace already doubled once.
- METR finds 1.9x at Anthropic, about 80% of it due to AI.
- Time-horizon doubling is shortening.
- Returns to research effort r > 1 (Chan et al.; Forethought).
- Revenue grew 3.5x in eight months; capex for 2027 is rising.
- Implied ECI if right: about 255 at end-2028 and about 450 at end-2031.

**Activity**
- 15 searches; 9 pages read.
- Compute and capex figures came from snippets only.
- Failed: SemiAnalysis; AI 2027 tracker.

### Step 5 (forecast)

**Draft forecast**

| Horizon | p1 | p50 | p99 |
|---|---|---|---|
| End-2028 | 193 | 229 | 320 |
| End-2031 | 210 | 305 | 760 |

- p_faster_than_before 0.65; p_less_than_half 0.07.
- Reference scenarios: A 0.20, B 0.52, C 0.28.

### Step 6 (review)

**Findings**
1. The capex disagreement was resolved on the false premise that the November figure revises the July one. Both trace to near-simultaneous forecasts (FactSet in July; S&P in August). S&P also projects negative free cash flow, which strengthens the downside.
2. The reviewer said Engadget credits the NYT rather than the WSJ.
3. The METR hedges were under-stated, and AECI is not the same scale as ECI.
4. The lower tail was too narrow given the 20% weight on scenario A and the ranges in the slower case.
5. Band task lengths contradicted the stated conversion of about 5–7 points per doubling.
6. The pace paths for Bands 1 and 2 landed in the next band up.
7. "Speed-up" was undefined.
8. Band 2's claim of "publishable maths" was close to today's level.

**Activity**
- 6 searches; 9 pages.

## How disagreements were resolved

- **Capex (step 3 vs step 4).** I accepted the reviewer's point. The two projections are near-simultaneous estimates with different coverage, so I treat 2027–28 compute as mostly funded and put the financial downside in 2029–31. The S&P negative-cash-flow item is added and marked "abstract only".
- **Engadget's source.** I rejected the reviewer's claim. I read the Engadget article myself, and it credits *The Wall Street Journal*, with a link to wsj.com. WSJ is kept.
- **Lower tail.** Accepted.
  - End-2028: p1 193→190, p5 201→199, p10 207→204, p25 217→215, p50 229→228.
  - End-2031: p1 210→203, p5 224→218, p10 236→230, p25 260→256, p50 305→302, p75 365→360.
  - p_less_than_half rose from 0.07 to 0.10, and p_faster_than_before fell from 0.65 to 0.63. I recomputed both against the percentiles.
- **Task lengths.** I adopted the reviewer's option (b): about 6 points per doubling up to week-scale tasks, rising to 10–15 points beyond month-scale tasks. This rule is now stated in beyond_benchmarks. The band task lengths were recomputed from it, which raised Band 1 to 4–8 months at 50% and Band 2 to 1–3 years.
- **Band pace paths.** Revised so that they land inside their bands:
  - Band 1: 8–12 points/yr in 2027, then 3–6.
  - Band 2: 17–20 points/yr through 2028, then about 7.
  - Band 3: about 22–25 points/yr throughout.
- **Speed-up.** Defined as the rate of capability gain relative to the same compute with no AI help, as the brief asks. Band values were revised to match: 1.2–1.5x, 1.5–2x, 2–3x, 4–8x, and 10x or more.
- **Scenario weights.** Revised to A 0.25, B 0.47, C 0.28. Scenario A's description (people direct most multi-day projects; modest speed-up) fits Bands 1–2 and part of the low end of Band 3.
- **Internal lead.** Step 2 gave 1–7 months and step 5 gave 1–6. I kept 1–7 because step 2's analysis was more detailed.
- **The faster case's high numbers (about 450 at 2031) and the slower case's (about 228).** Both are reported as given. The forecast sits between them because of how the evidence was weighed, not by averaging. The reasoning field sets out the weighing.

## Searches by the lead (13)

- Epoch Capabilities Index ECI (run twice: the first batch failed to print, then re-run)
- Epoch AI Capabilities Index top model score 2026
- METR Frontier Risk Report 2026
- Ege Erdil case for multi-decade AI timelines
- Epoch AI can AI scaling continue through 2030
- hyperscaler capex 2027 guidance November 2026
- Epoch AI is a compute crunch coming
- arXiv 2609.36054 automating AI R&D intelligence explosion
- Epoch AI FrontierMath Erdős GPT-6.2 Astra
- Toby Ord how well does RL scale
- METR time horizon 1.1 doubling time
- OpenAI GPT-6.1 Astra not released deception

## Pages opened by the lead

**Succeeded (13)**
- epoch.ai/data/eci_scores.csv
- epoch.ai/publications/eci-bayesian-methodology
- METR Anthropic assessment
- METR risk report PDF
- arXiv 2609.36054 PDF
- Erdil
- Epoch 2030
- Epoch compute crunch
- The Motley Fool
- The Decoder
- Toby Ord
- METR Time Horizon 1.1
- Engadget

**Failed (3)**
- The METR risk-report blog URL (not in prior context; I used the PDF instead).
- The GuruFocus capex article (not accessible).
- The Epoch model page for GPT-6.2 Astra (not accessible).

## Published forecasts consulted (evidence used, conclusions not used)

- AI Futures Project, Q3.5 update (step 4).
- AI 2027 forecasts and tracker (steps 2 and 4; snippets only).
- FutureSearch on release-gap timing (step 2; snippet only).
- Erdil (read by the lead; an argument piece containing a forecast).

## Sources containing instructions to agents

None found by any agent.

## Concentration of sources

Much of the core evidence comes from two organisations:
- **Epoch AI:** the data, method, compute and revenue pieces.
- **METR:** time horizons, the risk report and the Anthropic assessment.

The strongest acceleration evidence relates to Anthropic, the lead agent's developer.

## What went wrong or fell short

- Several sub-agents hit their tool limits before reading everything they planned.
- Compute, energy and capex evidence rests largely on secondary sources (FactSet, The Motley Fool, S&P via search results).
- Geopolitics was not researched.
- Hardest-benchmark results are unverified aggregator figures.
- I could not check whether capabilities.json parses as JSON with a program after writing it, because the output folder is not visible to the code sandbox. It was written by hand with care.
