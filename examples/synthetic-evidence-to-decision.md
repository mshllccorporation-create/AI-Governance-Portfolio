# Synthetic example | Evidence to governance decision

This original example illustrates how I would structure a limited AI governance review. The organization, system, records, and findings below are invented. It does not reproduce GuvFlow's private control catalog or imply a certification.

## Scenario and boundary

**Sample organization:** Northstar Services, a fictional 80-person company.  
**AI use:** A support assistant drafts replies for staff. A human sends each final message.  
**Decision under review:** Whether the assistant may recommend account credits to staff.  
**Period:** A hypothetical 30-day pilot. The review covers one workflow and does not assess the wider organization.

## Evidence register

| Evidence ID | Requested item | What it could establish | Limitation |
|---|---|---|---|
| E-01 | Approved workflow and role register | The intended authority boundary and named owner | A policy alone does not show that people followed it. |
| E-02 | Sample of 30 credit recommendations and final staff decisions | Whether review, changes, and overrides occurred | Sampling cannot prove every decision was handled correctly. |
| E-03 | Access and configuration change log | Who could change the assistant's permissions during the period | Completeness and clock synchronization need checking. |
| E-04 | Incident and customer correction records | Whether errors were identified and remediated | An empty register is not proof that no errors occurred. |

## Illustrative test and finding

**Control objective:** An AI recommendation must not issue a credit or change a customer account without an authorized person's decision.  
**Test:** Compare workflow permissions with E-01 and E-03; trace sampled recommendations through E-02 to the final staff action; check E-04 for exceptions.  
**Hypothetical observation:** The role register names a support lead, but six of the sampled records lack a stored approval reference. The sample does not establish whether those decisions were unreviewed or whether the evidence was lost.  
**Disposition:** **Insufficient evidence**, with a potential operating gap. Do not rate the control effective or assume a breach. The support lead should reconstruct those records, test log completeness, and decide whether a broader sample or incident review is needed.

## Decision record

| Field | Illustrative entry |
|---|---|
| Accountable owner | Support Operations Lead |
| Immediate authority | Staff retain final credit decisions; the assistant remains advisory |
| Remediation | Require an approval reference before a credit can be processed |
| Due date and verification | Owner sets a date; an independent reviewer retests the next sample and checks exception handling |
| Residual uncertainty | Missing historical references may prevent complete reconstruction |

The method separates a recommendation, a control claim, supporting evidence, a human decision, and a verified closure. It can be implemented with different model providers, ticketing tools, and evidence stores.
