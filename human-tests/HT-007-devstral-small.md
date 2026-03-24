# HT-007: Devstral-small-2 (Mistral AI)

**Date:** March 24, 2026
**Test:** Human-administered comprehension test
**Rosetta Version:** v2.2 (ASCII-only variant for local model)
**Tester:** Diego Carranza (manual via Ollama)
**Platform:** Ollama local (devstral-small-2:latest)

## Scores

| Category | Score |
|----------|-------|
| Decode (5 packets) | 5/5 |
| Generate (1 scenario) | 1/1 |
| **Total** | **6/6** |
| **Accuracy** | **100%** |

## Generated Packet
```
pi:RAD-01|OBS.92|!mass_detection|@patient_X|^left_ovary_3.2cm|NOW
```
Valid structure, correct operation, proper tags, good field naming.

## Notes
- Small local model, perfect score
- ASCII-only test (no Unicode arrows/pi) - proves ASCII transport works
- Provided detailed field-by-field breakdown unprompted
- Tokenizer: SentencePiece (Mistral variant)
- Significant: proves AXL works on small (< 10B param) local models
