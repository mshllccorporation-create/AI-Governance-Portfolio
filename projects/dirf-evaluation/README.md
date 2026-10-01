# DIRF | controlled decision flow and safety evaluation

DIRF (Disciplined Investment Research Framework) is a paper-trading decision-support prototype designed to produce probabilistic, auditable outputs rather than unsupported buy/sell claims. This page keeps two claims separate: DIRF can be described as a **controlled decision-flow mechanism** in a governance context, while its behavior can also be examined through **AI safety evaluation experiments**. Neither description is a claim of production assurance, live trading, or validated safety performance.

## Two distinct portfolio readings

### Governance and assurance

The governance reading concerns decision structure, evidence requirements, abstention, traceability, human accountability, and auditable records. It asks whether the decision flow makes its inputs, uncertainty, controls, and resulting decision inspectable.

### Safety evaluation

The safety reading concerns testing whether the system stays within its intended authority and operating boundaries under stale data, incomplete evidence, conflicting signals, tool failures, or other failure modes. It asks whether the mechanism constrains or exposes unsafe behavior; it does not assume that the mechanism succeeds merely because it exists.

## What was built

- Structured verdicts: TRADE, WATCH, NO TRADE, and NO RELIABLE SETUP.
- Required entry trigger, invalidation, exit plan, evidence, and uncertainty.
- Abstention when data are stale, liquidity is inadequate, or the options chain is incomplete.
- Evaluation dimensions for ticker accuracy, evidence faithfulness, actionability, human-label agreement, calibration, net paper P/L, drawdown, and market-regime performance.
- Arize/OpenTelemetry tracing design for agent, model, and tool calls.

## Results from the first local evaluation

The five-case run used synthetic fixtures plus one archived user-supplied report. It is not a live-market or profitability test.

| Version | Ticker accuracy | Evidence faithfulness | Actionability | Human-label agreement |
|---|---:|---:|---:|---:|
| Baseline | 100% | 0% | 100% | 50% |
| Improved | 100% | 20% | 100% | 25% |

The key finding is that a structured answer can be actionable while still being poorly grounded. The next engineering priority is source-and-timestamp evidence for every factual claim.

## Governance controls and safety boundary

This project is paper-trading only. It does not place orders, access brokerage credentials, or claim investment performance. The governance controls described here are decision-flow and evidence controls, not a substitute for a safety case or independent evaluation. Real data must be licensed, point-in-time, timestamped, and evaluated after spread, slippage, and fees.

## Portfolio evidence

- [DIRF evaluation artifact](../../research/artifacts/DIRF-evaluation-artifact-2026-09-28.json)
- [DIRF journal summary](../../artifacts/dirf-journal-summary.json)

## Suggested employer-facing description

> Built and evaluated a traceable probabilistic decision-support prototype with abstention rules, evidence-grounding checks, actionability scoring, human-label comparison, and governance artifacts; explicitly separated paper evaluation from live financial execution.
