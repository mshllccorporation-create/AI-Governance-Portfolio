# AI Governance Control Stack for Operational Stability

**Author:** Horatio Morgan  
**Type:** Conceptual research paper, March 2026  
**Public record:** [arXiv:2604.03262](https://arxiv.org/abs/2604.03262)

The paper proposes that operational stability in AI depends on more than consistent model outputs. It connects version governance, evidence-based control verification, decision-time explanation records, drift monitoring, and escalation to accountable organizational behavior.

The methodology is a conceptual architecture and pattern-based analysis. It offers a design rationale, not empirical validation of GuvFlow or proof of a measured risk reduction. The public arXiv record contains the paper.

## Canadian regulatory extension

The control stack can be extended through a jurisdiction-aware crosswalk that separates legal source, applicability, candidate control, evidence expectation, operational verification, and human review. For Canadian deployments, the workflow should preserve the relevant instrument and version, organization and provincial scope, sector and decision type, data use, official source key, mapping rationale, uncertainty, and next review action.

The crosswalk should link obligations to controls such as applicability and instrument scope; accountability and authority; impact assessment and change review; data permissions and lifecycle; security and approved access; quality, bias and outcome testing; notice and meaningful explanation; human review and approval; monitoring and remediation; recourse and privacy requests; and evidence and decision trace.

This extension does not turn a mapping into a compliance determination. Federal Algorithmic Impact Assessment results must be linked to the relevant system and confirmed impact level, while a separate privacy impact assessment may be required for Québec obligations. Unmapped provincial or sector coverage remains a review backlog, and historical legislative proposals must not be treated as enacted duties. The Canadian crosswalk therefore strengthens the framework’s applicability, provenance, evidence, and legal-review layers without claiming verified implementation or legal advice.

## Visibility into agentic systems

The framework is further strengthened by Chan et al., *Visibility into AI Agents* (FAccT 2024, arXiv:2401.13138). The paper identifies agent identifiers, real-time monitoring, and activity logs as complementary ways to make agent deployment observable. The control stack extends those measures by linking them to delegated authority, tool permissions, human approvals, interventions, evidence custody, attribution, and remediation.

This extension treats visibility as an accountability precondition rather than as accountability itself. A robust record should identify the deployed agent and configuration, developer and deployer context, user or principal, tools and services, other agents or sub-agents, instructions, actions, monitoring alerts, human interventions, and relevant system state. It should support review of human-removal risks, delayed or diffuse effects, multi-agent feedback, common dependencies, sub-agent creation, and containment or shutdown.

The framework also preserves the paper’s cautions: more visibility can create privacy costs and concentrate power. Monitoring and logging should therefore be risk-proportionate, purpose-limited, access-controlled, retention-limited, and subject to independent review. The paper is research grounding for technical governance, not an official legal source, compliance determination, or proof of liability.

## Country-level multinational operation

For a multinational deployment, the control stack treats jurisdiction as a first-class system boundary. A country selection does not produce a compliance answer by itself. The workflow must resolve legal entity, public or private status, federal or provincial authority, province or territory, sector, decision type, affected persons, data and cross-border flows, system and model version, agent and tool boundary, applicable instruments, source currency, evidence, human approval, and legal review.

The Canadian profile is therefore fail-closed. It can return assessment-ready only when selected federal, provincial, territorial, sectoral, privacy, contractual, and policy requirements have an applicability decision and evidence route. Unmapped or unresolved areas remain visible as incomplete or reassessment-required; they are not converted into a passing score. This makes the framework usable as one country module within a multinational evidence register while preserving each jurisdiction’s source, legal basis, and review history.

The corresponding GuvFlow implementation exposes explicit readiness states: `CANADA_ASSESSMENT_READY`, `CANADA_INCOMPLETE`, `CANADA_REQUIRES_LEGAL_REVIEW`, and `CANADA_REQUIRES_REASSESSMENT`. The ready state is gated by required context, current official sources, verified requirement records, operational evidence, human approval, and legal review. This is an assurance control for workflow behavior, not a claim that the framework itself determines Canadian law.
