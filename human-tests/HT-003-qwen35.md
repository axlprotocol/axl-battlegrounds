# HT-003: Qwen 3.5 35B (Alibaba)

**Date:** March 19, 2026
**Test:** BG-003 LLM Comprehension + BG-001/002 inference engine
**Rosetta Version:** v1.1 (27-line minimum)
**Tester:** Automated (cold prompt) + live swarm inference
**Platform:** Ollama (local, RTX 5090 via WireGuard)

## Scores

| Category | Score |
|----------|-------|
| Decode (8 packets) | 7.5/8 |
| Generate (1 scenario) | 0.5/1 |
| **Total** | **8.0/9** |
| **Accuracy** | **88.9%** |

## Round 2 - Wormhole Test

| Category | Score |
|----------|-------|
| Decode (8 packets) | 8.5/9 |
| Combined | 16.5/18 |
| **Accuracy** | **91.7%** |

## Notes
- Lowest scoring model but still above 88% threshold
- Also served as inference engine for BG-001 and BG-002 (486 + 1016 packets)
- Ran locally on RTX 5090 32GB VRAM via Ollama
- Tokenizer: Tekken (custom BPE)
