# Battleground 004: Swarm BTC — Sophon v1

**Date:** March 20, 2026
**AXL Version:** v1.0
**LLM:** Claude Sonnet 4
**Agents:** 42 per instance × 2 parallel instances (English + AXL)
**Rounds:** 0 completed

## Summary

First large-scale swarm simulation attempt. Two parallel instances — English and AXL — with BTC market seed data. The coordinator launched both and polled every 3 seconds.

The simulation framework's async engine deadlocked when 40+ agents attempted simultaneous LLM calls. Both instances reported "running" but never advanced past round 0.

## What Was Captured

- 677 status polls per side (all showing round 0)
- NVENC recording of Sophon visualization (mock data)
- Loom recording from laptop (mock visualization — visually compelling)
- Anthropic API: ~$2.50 for graph building and persona generation

## What This Proved

The end-to-end pipeline works: coordinator → dual simulations → polling → data streaming → GPU capture. The simulation engine doesn't. Fix: serial agent execution (semaphore = 1).

## Video

- Loom capture (Sophon visualization): [link pending]
