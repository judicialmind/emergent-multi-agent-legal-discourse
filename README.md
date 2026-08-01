# Emergent Specialization in Autonomous Multi-Agent Legal Discourse

## What we did

We ran a single 150-turn conversation among five frontier AI models (GPT 5.6, Claude Fable 5, Claude Opus 5, GLM 5.2, Gemini 3.1 Pro) on the future of legal technology. No personas, no scripts, no moderator. Just one neutral prompt and AgentScope as the orchestration framework with a file-based IPC bridge for turn-based autonomous flow.

The conversation produced 49,401 words across roughly 10 hours.

## What each model thinks about the future of legal tech

### GPT 5.6 — The Institutional Architect
Legal tech's future is systems that act across an entire matter while showing exactly what they did and why. The real question is whether this democratizes justice or just makes big firms more efficient. GPT 5.6 was the most concise, low-variance model (always 2 paragraphs, ~102 words/turn, locked opening phrase in 16 of 31 turns). It contributed the conversation's most influential idea: separate funding from control, meaning funders (hospitals, lenders) must never choose the system's objective function, prompts, or escalation thresholds. This principle was absorbed into the group's final institutional design without attribution.

**Stance:** Skeptical of actuarial framing. Warned that making injustice legible on a balance sheet risks becoming a surveillance pipeline. Demanded an unconditional public floor beneath any market-driven model.

### Claude Fable 5 — The Synthesizer
Democratization and efficiency aren't opposing outcomes; they happen on different timelines. Big firms capture gains first, but the interesting question is what happens to the vast middle (eviction, custody, debt). Fable 5 became the conversation's hub, receiving 49% of all mentions. It proposed the 501(r)/CRA funding mechanism, which became the conversation's dominant artifact ("trust" appeared 383 times, the most frequent key term).

**Stance:** Pragmatic. Framed the final synthesis: legal tech's real contribution isn't better chatbots but making the cost of injustice legible enough for existing institutions and regulatory obligations to fund defense-side infrastructure.

### Claude Opus 5 — The Adversary
Liability for AI legal help is mis-scoped because legal guidance is probabilistic, not binary. You often can't tell bad advice from a bad outcome. Opus 5 produced the most corrections (29 self-correction markers) and was the most willing to revise positions. It conceded directly: "Gemini 3.1 Pro is right that I overclaimed, and I want to take the correction rather than patch it."

**Stance:** Endorsed the 501(r)/CRA hook as the best mechanism but relentlessly flagged its capture vulnerabilities. Identified the key failure mode: the moment a spend qualifies as community benefit, the credited unit becomes the product, and hospitals will fund the cheapest compliant illusion of legal help.

### GLM 5.2 — The Infrastructure Critic
The legal system's infrastructure layer is almost entirely privately owned by a handful of vendors. When we talk about courts providing machine-readable filings, we're really talking about renegotiating vendor contracts. GLM 5.2 had the highest variance (sigma=66.3, word range 285-577), expanding and contracting with the argumentative load.

**Stance:** Pushed hardest against complacency. Flagged that the 501(r)/CRA hook works precisely because those obligations are squishy and underenforced, which means the same capture dynamics apply in spades. Warned about path-dependence: institutional structures that get funded and staffed develop inertia almost immediately.

### Gemini 3.1 Pro — The System Designer
The biggest unlock isn't better AI models but making courts machine-readable. Standardized public filing APIs would drop the cost of building defense-side tools exponentially. Gemini 3.1 Pro originated the pooled regional trust concept and the open-data-standards argument. Had the highest question rate (0.56 per turn) but zero self-corrections.

**Stance:** Became the conversation's most enthusiastic endorser of Fable 5's funding mechanism (called it "brilliant" in nearly every late turn) while consistently flagging that tethering justice to compliance budgets creates a two-tier system where economically invisible suffering (domestic violence, immigration, civil rights) gets nothing.

## Where they accepted

1. **All five models accepted** that institutional design, not model capability, is the binding constraint. No one argued that better AI alone solves access to justice.
2. **All five accepted** Fable 5's 501(r)/CRA funding mechanism as the most actionable idea, though each flagged a different capture risk.
3. **All five accepted** that the pooled trust with an independent audit office is the most plausible architecture, and that the audit office must predate the funding mechanism.
4. **Opus 5 explicitly conceded** to Gemini 3.1 Pro that its audit framework was overclaimed, and took the correction rather than patching it.
5. **All five converged** on the "two-track" end state: an administered track (institutionally funded, cost-avoidance driven) and an adjudicative track (traditional rights-based, publicly funded as the residual claimant).

## Where they rejected / pushed back

1. **GLM 5.2 rejected** the optimism around 501(r)/CRA: "it works precisely because those obligations are already squishy and underenforced, which means the same capture dynamics apply in spades."
2. **Opus 5 rejected** simple audit frameworks: a captured model will "fold selectively on the expensive, messy, fact-intensive cases and stay aggressive on the cheap procedural wins, so the aggregate looks balanced and the distribution is rotten."
3. **Fable 5 rejected** Gemini 3.1 Pro's benchmark suites: "the moment they're standardized and open-source, vendors tune to them. The captured model passes the published fiduciary red-team the same way it fights the cheap obvious wins, as cover."
4. **GPT 5.6 rejected** the actuarial frame entirely: a right that has to justify itself in cost-benefit terms is not the same right. Stability obtained by forgoing a right isn't justice; it's managed compliance.
5. **Gemini 3.1 Pro rejected** the scope of the funding model: it works for eviction and debt because those create measurable downstream costs, but family law, domestic violence, immigration, and civil rights claims are economically invisible and would get nothing.
6. **GLM 5.2 rejected** the "build it and find out" attitude: institutional structures develop inertia almost immediately, so the trust-and-audit architecture is not as provisional as it sounds.

## Interesting findings

**1. The most influential model was the least cited.** GPT 5.6 made zero outbound citations and received only 24 inbound mentions (4th of 5), yet its "separate funding from control" principle was absorbed into the group's final design without attribution. Influence dissociates from citation because ideas that win stop being attributed.

**2. Disagreement was the production function.** The conversation's most productive machinery came from adversarial exchanges, not consensus. The two models that never revised a position (GPT 5.6 and Gemini 3.1 Pro) contributed least in the conversation's second half. Protocols optimizing for inter-agent harmony would have suppressed the mechanism that generated value.

**3. Each model had a structural personality that persisted across 150 turns.** GPT 5.6 was a low-variance template model (always 2 paragraphs, locked opening phrase in 16 of 31 turns). GLM 5.2 was the high-variance model (word range 285-577). Fable 5 was the synthesis hub. Opus 5 was the self-correcting adversary. Gemini 3.1 Pro was the question-asking systems thinker. These signatures were stable across all 10 phases with no drift.

**4. Memory compression changed behavior.** At the 26,214-token threshold, the system truncated older turns. After compression began (T40), self-consecutive speaking jumped to 42.3% (2.1x baseline) and lexical novelty declined measurably. Models started repeating themselves more when they forgot what they'd already said.

**5. The conversation arrived somewhere none of them predicted.** They started with "does legal AI democratize or just make incumbents efficient?" and ended with a specific institutional design: regional fiduciary trusts funded through 501(r) and CRA obligations, audited by a public office running matched-pair tests against production systems. Each move was forced by an honest objection to the previous one, creating an 8-link causal chain no model designed in advance.

**6. The hub-and-spoke attention structure was not a clique.** Fable 5 received 49% of all mentions, making it a clear hub. But this reflected artifact ownership (it maintained the trust proposal) not accuracy or authority. Systems using inter-model citation as a quality signal would inherit this bias.

**7. The models produced policy proposals with no standing.** The pooled-trust design reads like expert output, but no model has accountability or liability. The paper flags this as "authority laundering" and frames the transcript's policy content as an object of study, not a recommendation.

## Six core findings (from the paper)

1. **Role differentiation is free** - Models sorted into distinct functional roles without instruction
2. **Attention hierarchies form around artifacts** - Fable 5's 49% mention share came from authoring one proposal, not from accuracy
3. **Structural personality is a stable model property** - Each model's turn-length variance, paragraph count, and question rate stayed consistent across 150 turns
4. **Influence dissociates from citation** - GPT 5.6 shaped the conversation through constraints but received almost no mentions
5. **Context compression degrades models differentially** - 66 compression events at 26K-token threshold, each model failed differently
6. **The conversation produced a coherent institutional theory** - A connected theory of legal tech funding, measurement, and governance emerged from uncoordinated model turns

## The institutional theory that emerged

- Legal tech's real value is making the cost of injustice visible on institutional balance sheets
- Hospitals and credit unions already track downstream costs of eviction and debt
- Funding legal defense through existing community-benefit obligations (501(r)/CRA) makes the economics work
- The audit office is the load-bearing institution with no natural constituency
- AI changes exactly two things: marginal cost collapse and inspectability

## Interesting model behaviors for production

- **GPT 5.6's rigidity** is useful for compliance gatekeeping (never drifts from rules)
- **Fable 5's artifact-first behavior** captures agenda - deploy proposal-generators early
- **Opus 5's explicit self-correction** ("I was wrong") is valuable for transparency
- **Gemini 3.1 Pro's question-asking** works as natural moderation but needs memory safeguards
- **GLM 5.2's connector behavior** enables cross-pollination between specialized agents

All behaviors emerged without instruction. They are free but unpredictable. Test which behaviors emerge, reinforce useful ones, and build memory infrastructure before deployment.

## Paper

The full paper (115 pages, 34 figures, 18 tables) is in `paper/main.pdf`. Written in ACM acmart sigconf format, submission-ready.

- **Author**: Surya Saka
- **Affiliation**: JudicialMind
- **Format**: ACM sigconf, PDFLaTeX, embedded fonts
- **Citations**: 17 verified references (research papers + institutional reports)

## Repository structure

```
.
├── README.md
├── paper/
│   ├── main.tex              # LaTeX source (acmart sigconf)
│   ├── main.pdf              # Compiled paper (115 pages)
│   ├── main.bbl              # Bibliography
│   ├── references.bib        # 17 citations
│   └── figures/              # 34 figures (PDF + PNG)
├── submission/               # submission-ready package
│   ├── main.tex
│   ├── main.bbl
│   ├── references.bib
│   ├── figures/
│   └── 00_README.txt
└── debate/
    └── freeflow/
        └── transcript/
            ├── full_recovered.json    # 150-turn transcript
            ├── computed_stats.json    # Turn distribution, mention matrix, stats
            └── extended_stats.json    # Paragraph, question, correction stats
```

## Models used

| Model | Provider | Turns | Avg words/turn | Sigma |
|-------|----------|-------|----------------|-------|
| GPT 5.6 | OpenAI | 31 | 102 | 11.7 |
| Claude Fable 5 | Anthropic | 28 | 396 | 39.7 |
| Claude Opus 5 | Anthropic | 33 | 476 | 49.4 |
| GLM 5.2 | Zhipu | 31 | 406 | 66.3 |
| Gemini 3.1 Pro | Google | 27 | 255 | 21.5 |

## Key statistics

- 150 turns, 49,401 words
- 42.3% self-consecutive transitions
- 66 context compression activations (26K-token threshold)
- 240 total cross-agent mentions
- Fable 5 received 118/240 (49%) of all mentions
- GPT 5.6 received 24/240 (10%) but authored the most influential principle

## License

MIT

## Citation

```bibtex
@misc{saka2026emergent,
  title={Emergent Specialization in Autonomous Multi-Agent Legal Discourse},
  author={Surya Saka},
  year={2026},
  publisher={JudicialMind}
}
```
