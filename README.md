# Project 2: DPDP Act 2023 Compliance Gap Assessment

## Objective
Assess ExampleOrg Pvt Ltd's current data handling practices against the
requirements of India's Digital Personal Data Protection Act, 2023 (DPDP Act) and identify
a prioritized remediation roadmap ahead of the Act's rules coming into full force.

## Why this matters
The DPDP Act is India's first comprehensive personal data protection law. As of the current
compliance timeline, most Indian companies — especially fintechs handling sensitive financial
and KYC data — are still building out their compliance posture. This assessment simulates the
kind of gap analysis a GRC analyst would be asked to produce as this law is operationalized.

## Scope of work
1. **Data Processing Inventory** — records what personal data ExampleOrg collects, why, and
   the legal basis for processing
2. **Gap Assessment Methodology** — the framework used to score compliance maturity
3. **Compliance Gap Tracker** — 20 requirement areas assessed against current state, with
   remediation owner and target date
4. **Executive Summary** — leadership-ready summary of findings and risk exposure

## Key findings (executive summary preview — full version in executive-summary.md)
- **7 of 20 requirement areas assessed as Non-Compliant**, concentrated in consent
  management granularity, Data Principal rights fulfillment (no formal process to handle
  access/erasure/nomination requests), grievance redressal, breach notification readiness,
  and Significant Data Fiduciary obligations (no DPO appointed, no SDF threshold assessment done)
- **11 areas Partially Compliant** — mostly requiring formalization of practices that exist
  informally today (notice design, vendor DPAs, DPIA process, cookie consent granularity)
- **1 area already fully Compliant** (RoPA/data processing inventory, built as part of this
  exercise) and **1 Not Applicable** (children's data — product requires 18+ KYC-verified customers)
- Highest-priority gap: **no Consent Manager / consent capture mechanism** distinguishing
  purpose-specific consent, required for lawful processing of customer data under Section 6

## Files in this folder
| File | Purpose |
|---|---|
| `data-processing-inventory.csv` | Record of Processing Activities (RoPA)-style inventory |
| `gap-assessment-methodology.md` | Scoring criteria used |
| `compliance-gap-tracker.csv` | 20 requirement areas scored and tracked to remediation |
| `executive-summary.md` | Leadership summary with risk framing |

## Disclaimer
This is a training/portfolio artifact built against a fictional company for skills
demonstration. It reflects a reasonable professional interpretation of the DPDP Act 2023
and draft Rules as understood at the time of writing, and is not legal advice.
