# GuvFlow Agentic Governance

GuvFlow treats agentic AI governance as an operational problem: whether authority, actions, dependencies, evidence, and failures remain governable during execution.

```text
Map -> Test -> Decide -> Execute -> Monitor -> Verify -> Improve
```

## Core record model

```text
AI asset -> failure mode -> risk/finding -> control -> evidence -> owner -> action -> verification
```

Shadow AI is a discovery source, not a separate governance system. A discovered tool or model should be registered as an AI asset, assessed for risk, linked to a finding when action is required, and moved through states such as `Unverified`, `Under Review`, `Restricted`, `Approved`, `Remediated`, or `Removed`.
