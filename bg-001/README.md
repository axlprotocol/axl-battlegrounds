# Battleground 001: Trading Agents

**Date:** March 17, 2026
**AXL Version:** v1.0
**Rosetta:** 133 lines (v1.1)
**Domain:** Financial trading
**Agents:** 11 (10 different computational architectures)
**Packets:** 486 (100% parse validity)

## Summary

First live test of the AXL protocol. Eleven agents — crawler, monitor, signal producer, accountant, sentinel, code reviewer, analyst, dispatcher, project manager, shapeshifter, and thief — communicated exclusively in AXL packets on a simulated trading floor.

## Results

- 486 packets generated, 100% parse validity
- 9 active domains: COMM, DEV, OPS, PAY, REG, RES, SEC, SIG, TRD
- 33 agent-to-agent payments
- 4 two-way conversations, 124 ACK responses
- 2 security events: thief detected independently by sentinel AND accountant
- Gas burned: $3.83

## Theft Detection

A malicious agent was introduced into the network. It attempted to extract funds from other agents. The sentinel and the accountant both independently detected the theft using AXL's typed payment fields — the payment amounts didn't match expected values. No coordination between the two detectors. Emergent security from protocol structure.

## Video

- [YouTube](link pending)
