# Emergent Specialization in Autonomous Multi-Agent Legal Discourse

## What we did

We ran a single 150-turn conversation among five frontier AI models (GPT, Fable, Opus, GLM, Gemini) on the future of legal technology. No personas, no scripts, no moderator. Just one neutral prompt and AgentScope as the orchestration framework with a file-based IPC bridge for turn-based autonomous flow.

The conversation produced 49,401 words across roughly 10 hours.

## What we found

The agents spontaneously developed distinct roles within 15 turns:

| Agent | Model | Emergent Role | Key Behavior |
|-------|-------|--------------|--------------|
| Agent One | GPT | Rights-Floor Minimalist | 2 paragraphs every turn, 0 outbound mentions, σ=11.7 words |
| Agent Two | Fable | Proposal Hub | Authored central funding mechanism, received 49% of all mentions |
| Agent Three | Opus | Doctrinal Empiricist | Longest turns (476 avg words), 29 self-corrections |
| Agent Four | GLM | Connector | 83 outbound mentions (highest), synthesis role |
| Agent Five | Gemini | Questioner | 56% question rate, forgot it proposed key ideas under compression |

### Six core findings

1. **Role differentiation is free** - Agents sorted into distinct functional roles without instruction
2. **Attention hierarchies form around artifacts** - Fable's 49% mention share came from authoring one proposal, not from accuracy
3. **Structural personality is a stable model property** - Each model's turn-length variance, paragraph count, and question rate stayed consistent across 150 turns
4. **Influence dissociates from citation** - GPT shaped the conversation through constraints but received almost no mentions
5. **Context compression degrades agents differentially** - 66 compression events at 26K-token threshold, each model failed differently
6. **The conversation produced a coherent institutional theory** - A connected theory of legal tech funding, measurement, and governance emerged from uncoordinated agent turns

### The institutional theory that emerged

- Legal tech's real value is making the cost of injustice visible on institutional balance sheets
- Hospitals and credit unions already track downstream costs of eviction and debt
- Funding legal defense through existing community-benefit obligations (501(r)/CRA) makes the economics work
- The audit office is the load-bearing institution with no natural constituency
- AI changes exactly two things: marginal cost collapse and inspectability

## Interesting agent behaviors for production

- **GPT's rigidity** is useful for compliance gatekeeping (never drifts from rules)
- **Fable's artifact-first behavior** captures agenda - deploy proposal-generators early
- **Opus's explicit self-correction** ("I was wrong") is valuable for transparency
- **Gemini's question-asking** works as natural moderation but needs memory safeguards
- **GLM's connector behavior** enables cross-pollination between specialized agents

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
├── submission/         # submission-ready submission package
│   ├── main.tex
│   ├── main.bbl
│   ├── references.bib
│   ├── figures/
│   └── 00_README_Submission.txt
└── debate/
    └── freeflow/
        └── transcript/
            ├── full_recovered.json    # 150-turn transcript
            ├── computed_stats.json    # Turn distribution, mention matrix, stats
            └── extended_stats.json    # Paragraph, question, correction stats
```

## Models used

| Agent | Model | Provider |
|-------|-------|----------|
| Agent One | GPT 5.6 | OpenAI |
| Agent Two | Claude Fable 5 | Anthropic |
| Agent Three | Claude Opus 5 | Anthropic |
| Agent Four | GLM 5.2 | Zhipu |
| Agent Five | Gemini 3.1 Pro | Google |

## Key statistics

- 150 turns, 49,401 words
- 42.3% self-consecutive transitions
- 66 context compression activations (26K-token threshold)
- 240 total cross-agent mentions
- Fable received 118/240 (49%) of all mentions

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
