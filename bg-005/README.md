# Battleground 005: Swarm BTC — Sophon v2

**Date:** March 20-21, 2026
**AXL Version:** v1.0 (pre-cognitive grammar)
**Rosetta:** 133 lines (v1.1)
**LLM:** Claude Sonnet 4
**Agents:** 12 per instance × 2 parallel instances (English + AXL)
**Rounds:** 13
**Duration:** 3h 38m
**Cost:** ~$10

## Summary

After fixing the simulation deadlock, both instances ran to completion. 13 rounds of real multi-agent debate about BTC price direction. Agents wrote substantive analysis — gamma exposure, whale positioning, funding rate arbitrage, ETF flow analysis.

## Results

| Metric | English | AXL v1.0 |
|--------|---------|----------|
| Posts | 26 | 21 |
| Comments | 59 | 43 |
| Likes | 3 | 9 |
| Dislikes | 0 | 3 |
| Total interactions | 88 | 76 |
| Compression ratio | — | 0.97x |

## The Failure That Changed Everything

Compression ratio: 0.97x. No compression. AXL agents wrote full English paragraphs with Greek-letter prefixes (ΣDATA, ΣOPS). The protocol had vocabulary for data but not for reasoning. Agents could say "$BTC is at $70,200" in AXL but could not say "I disagree with your analysis" in AXL.

This failure directly motivated:
- **v2.1** — Universal Cognitive Grammar (7 reasoning operations: OBS, INF, CON, MRG, SEK, YLD, PRD)
- **v2.2** — Geometric foundation (Platonic Representation Hypothesis, dimensional analysis)

## Video

- [YouTube](link pending)
