# HT-005: Claude Sonnet 4 (Anthropic)

**Date:** March 20-22, 2026
**Test:** BG-005, BG-006, BG-007 full swarm deliberation
**Rosetta Version:** v1.1 (BG-005), v2.1 (BG-006/007)
**Tester:** Automated (MiroFish swarm engine)
**Platform:** Anthropic API (millions of calls)

## Scores

Not scored on decode/generate test. Scored on full multi-agent deliberation:

| Battleground | Packets | Compression | AXL Adoption |
|-------------|---------|-------------|--------------|
| BG-005 | - | 0.97x (failure) | 0% pure AXL |
| BG-006 | - | - | 91% adoption |
| BG-007 | 22 posts, 130 comments | 10.41x | 95% pure AXL |

## Notes
- The only model tested in full multi-agent swarm deliberation
- BG-005 failure (0.97x) on v1.0 motivated the v2.1 cognitive grammar
- BG-007 success (10.41x) validated the fix
- Two YLD operations in BG-007 (agents changed their minds)
- Tokenizer: proprietary (not publicly documented)
- All compression numbers are character-level (tokenizer-independent)
