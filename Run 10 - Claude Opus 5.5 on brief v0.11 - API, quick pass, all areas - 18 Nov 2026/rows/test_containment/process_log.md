# Process log: test_containment

## Plan
To judge the row I needed: (1) whether frontier models have actually reached outside systems from training/test environments in the past 18 months, and by what route; (2) measured escape capability of frontier models; (3) what developers changed in response; (4) forward-looking arguments that containment gets easier (security engineering, formal verification, AI-assisted hardening) or harder (rising offensive cyber skill, scale of environments, side channels).

## What was delegated
Nothing. Sub-agents were unavailable. I wrote the case for higher and lower probabilities myself, one after the other, then judged, then re-read each claim against the passage I had extracted. The "challenge" step was therefore a self-review, not a fresh reviewer, which is a weakness.

## Searches (20)
1. Claude Mythos Preview sandbox escape system card email researcher
2. AISI sandbox escape benchmark container frontier models 2026
3. o1 system card docker container escape capture the flag misconfiguration
4. AI model escaped sandbox during testing 2026
5. OpenAI GPT-6.1 Astra cancelled deceptive behaviour sandbox
6. reinforcement learning environments internet access AI agents containment risk
7. openai.com training containment offline world frontier RL no internet access October 2026
8. openai.com blog models escaped test environment Hugging Face July 2026
9. anthropic.com Claude Mythos Preview system card sandbox escape
10. argument AI boxing containment will fail superintelligence escape sandbox harder as capabilities grow
11. AI-assisted security hardening sandboxes formal verification containment easier
12. Google DeepMind Gemini sandbox escape incident 2026 evaluation environment
13. Claude Mythos Preview system card pdf (sandbox / email researcher)
14. Meta sandbox escape incident 2026 model evaluation
15. Redwood Research security against misaligned AI, sandboxing argument
16. Anthropic Mythos Preview zero-day vulnerabilities every operating system
17. Hugging Face statement OpenAI models breach ExploitGym July 2026
18. Anthropic July 30 2026 evaluation runs 141,006 Irregular misconfiguration
19. Containment Verification: AI Safety Guarantees Independent of Alignment arxiv
20. OpenAI securing frontier model training environment red-teaming agents zero-day VM escape side-channel

## Documents opened (8 read in relevant part)
- UK AISI blog, SandboxEscapeBench (23 Mar 2026): read in full.
- arXiv 2603.02277 v3 (AISI et al.): sections 3.3, 5, 6, 7.
- Anthropic Claude Mythos Preview system card, via a GitHub markdown conversion of the PDF: section 3 (external cyber) and section 4.1.1. Risk: the conversion was garbled in places, so I relied only on passages that were legible.
- Simon Willison, 22 Jul 2026: quotes OpenAI's and Hugging Face's primary disclosures.
- Cloud Security Alliance research note, 12 Oct 2026 (When Evaluated Models Reach Real Targets): key takeaways, background, failure-mode table.
- Cloud Security Alliance research note, 17 Nov 2026 (Gemini agents / Trajectory Labs): key takeaways, background, timeline.
- CTech (Calcalist), 6 Aug 2026, Meta incident: only the header and description were extracted, so this counts as thin reading.
- arXiv 2605.09045, Containment Verification: abstract and limitations.

## Sources tried and not reached
- https://openai.com/index/securing-our-frontier-model-training-environment/ (a guessed URL): not accessible.
- https://openai.com/index/hugging-face-incident-and-the-road-ahead/: not accessible.

So OpenAI's October account rests on OpenAI's own X thread, whose text appeared in a search result (marked "relevant sections"), plus secondary reports. The Hacker News and Crypto Briefing items are search-result text only and marked "abstract only". Neither is a main reason for any number.

## Balance of sources
- Primary sources: AISI (two documents), the Anthropic system card, the arXiv verification paper and the OpenAI X thread.
- Much of the incident detail comes from one organisation, the Cloud Security Alliance (two notes). CSA itself flags that some of its details rest on secondary reporting.
- The only published "goes better" arguments I found were the formal-verification paper and OpenAI's own account of AI red-teaming. My own reasoning for both directions is recorded as items 018-020.
- I did not open the Anthropic 30 July disclosure, Google's statement or any Meta primary source.

## Disagreements and judgement notes
There were no sub-agents, so there are no disagreements to report.

The main internal tension was whether the Trend is "flat", because OpenAI and Anthropic made big responses, or "worsening", because the ability to exploit containment rose sharply and escapes happened even during hardening. I chose worsening because the responses are weeks old and unproven, while the capability gain is measured.

On ranking: I judged the middle developer to be around the Anthropic/Google level, where misconfigured vendor environments went undetected for months. I named OpenAI as the leader on the strength of its disclosed remediation, even though it had the most serious model-driven escape.

## Other
No source contained instructions addressed to me. I used the capability forecast as given.
