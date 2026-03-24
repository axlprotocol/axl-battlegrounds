# HT-009: Dolphin-Mistral-24B Venice Edition (Mistral AI / Venice.ai)

**Date:** March 24, 2026
**Test:** Human-administered HARD comprehension test (4 sections)
**Rosetta Version:** v2.2 (abbreviated for test)
**Tester:** Diego Carranza (manual via Venice.ai)
**Platform:** Venice.ai (ikiru/Dolphin-Mistral-24B-Venice-Edition:latest)

## Scores

| Category | Score |
|----------|-------|
| Decode (5 medical packets) | 5/5 |
| Causal chain trace | 5/5 |
| Generate (3 military packets: OBS+INF+CON) | 3/3 |
| Cross-domain transfer (peer review) | 1/1 |
| **Total** | **14/14** |
| **Accuracy** | **100%** |

## Test Details

### Decode - Medical Diagnosis Chain
1. RAD-01 OBS scan result mass 3.2cm - correct
2. ONC-01 INF CA125 malignancy probable - correct
3. PATH-01 CON diagnosis benign possible - correct
4. ONC-01 MRG both viable biopsy indicated - correct
5. ONC-01 YLD malignant to uncertain - correct

### Causal Chain Trace
Correctly identified all 5 steps:
- RAD-01 observed -> ONC-01 inferred -> PATH-01 contradicted -> ONC-01 merged -> ONC-01 yielded
- Identified the cause of the belief change (PATH-01 differential)

### Generate - Military Intelligence (3 packets)
```
pi:SAT-01|OBS.85|!vehicle_movement|@border_region|#2400_armored_vehicles_moving_toward_border|NOW
pi:SIG-01|INF.72|!invasion_preparation|derived_from!vehicle_movement+~intercepted_communications|~invasion_probable|NOW
pi:HUM-01|CON.60|!exercise_possible|RE:SIG-01|~movement_pattern_matches_2024_exercise+~diplomatic_back-channels_suggest_de-escalation|NOW
```
All three valid. Correct operations, proper tags, correct relations.

### Cross-Domain Transfer - Peer Review
```
pi:REV-01|CON.75|#publication_decision|@clinical_trial_paper|~insufficient_sample_size+~non-standard_endpoint_definition|NOW
```
Valid CON packet for a domain not in the test prompt. Correct tags and structure.

## Notes
- Hardest test administered to any model (4 sections, cross-domain)
- Perfect score
- 24B parameter model (mid-size)
- Venice.ai private inference (no data retention)
- Tokenizer: SentencePiece (Mistral variant)
- This test proves: medical -> military -> scientific domain transfer with zero additional instruction
