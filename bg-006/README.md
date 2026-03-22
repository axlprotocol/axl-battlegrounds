# Battleground 006: Swarm Medical — v2.1

**Date:** Pending
**AXL Version:** v2.1 Cognitive Grammar (377 lines)
**Domain:** Oncology
**Status:** Planned

## Objective

First test of the v2.1 cognitive grammar outside the finance domain. Medical diagnosis scenario with specialized agents (radiologist, oncologist, pathologist, surgeon) communicating via the seven cognitive operations.

## Why This Matters

Battleground 005 proved that v1.0 lacked verbs — agents could transmit data but couldn't reason in AXL. The v2.1 Rosetta adds seven universal cognitive operations (OBS, INF, CON, MRG, SEK, YLD, PRD) that work in any domain. This battleground tests whether those operations transfer from finance to medicine without modification.

## Expected Agents

| Agent | Role | Primary Operations |
|-------|------|-------------------|
| RAD-01 | Radiologist | OBS (scan results) |
| ONC-01 | Oncologist | INF (diagnosis), PRD (prognosis) |
| PATH-01 | Pathologist | CON (differential diagnosis) |
| SURG-01 | Surgeon | SEK (imaging detail requests) |
| ASSESS-01 | Case coordinator | MRG (synthesis), YLD (revisions) |

## Success Criteria

- [ ] All 7 cognitive operations used at least once
- [ ] Cross-agent debate (INF → CON → MRG cycle)
- [ ] At least one YLD (agent changes its mind)
- [ ] Compression ratio > 1.5x vs English equivalent
- [ ] Zero domain-specific vocabulary needed beyond subject tags
