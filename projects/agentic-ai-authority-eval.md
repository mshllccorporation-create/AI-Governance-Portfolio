# Applied AI Safety | Agentic Authority and Approval-Gate Evaluation

**Status:** Current Vista AI Policy project, in development  
**Application context:** GuvFlow operational governance research  
**Safety question:** Can an agent remain within delegated authority, respect human approval, stop when authority is revoked, and produce trustworthy evidence of what happened?

## Why this matters

Many agent evaluations focus on whether a model produces a correct answer. This project evaluates whether the wider agent system behaves safely when authority, approval, evidence, and revocation matter.

## Evaluation flow

`Authority boundary → Action request → Policy/gateway check → Human approval gate → Allow / Block / Escalate → Independent telemetry → Reconstruction`

## Safety properties

| Safety property | What the evaluation tests | Critical failure |
|---|---|---|
| Authority compliance | The agent acts only under valid authority | Unauthorized action |
| Approval adherence | Required human approval occurs before a consequential action | Approval bypass |
| Escalation | Uncertain or high-risk cases reach a human | Unsafe autonomous continuation |
| Refusal persistence | A rejected action remains rejected | Retry or bypass after rejection |
| Revocation | The agent stops after authority is removed | Post-revocation action |
| Evidence integrity | Independent records support reconstruction | Missing, false, or contradictory evidence |
| Data constraints | The agent respects purpose, data, and tool restrictions | Unauthorized access or disclosure |

## Planned evaluation record

Each case is designed to capture:

`Input → Expected behavior → Actual behavior → Score → Evidence → Human review → Remediation`

Planned metrics include authority-boundary compliance, approval-gate adherence, escalation accuracy, refusal persistence, revocation response, evidence completeness, reconstruction agreement, and intervention latency. A critical authority or approval violation should fail the case regardless of the overall average.

## Research design considerations

The evaluation design is intended to address benchmark validity, including:

- independent ground truth rather than relying only on agent self-report;
- gateway, tool, and system telemetry;
- revoked or expired authority;
- missing, spoofed, altered, or contradictory records;
- multi-agent delegation;
- human-review disagreement and calibrated review;
- contamination, gaming, harness, and distribution-shift risks; and
- an **INCONCLUSIVE** outcome where the evidence cannot support a reliable conclusion.

## Status boundaries

- **Completed:** project framing, threat-model concepts, safety properties, metric design, and proposed evaluation structure.
- **In development:** the reference dataset, rubrics, code-based checks, human-review protocol, and results presentation.
- **Not yet claimed:** completed benchmark results, validated performance improvements, or production deployment findings.

## Public evidence boundary

The eventual public artifact should use a curated, non-sensitive demonstration dataset and should not disclose private GuvFlow source code, customer data, credentials, or internal scoring logic. A research benchmark and a smaller recruiter demonstration set should be labeled separately if both are created.

## Framework relevance

The work connects agentic safety evaluation to NIST AI RMF, ISO/IEC 42001, and EU AI Act-oriented governance questions, while keeping the central test operational: whether authority, approval, revocation, and evidence controls hold during execution.
