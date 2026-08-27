# Project 1: ISO/IEC 27001:2022 ISMS Implementation Kit

## Objective
Design and document a complete Information Security Management System (ISMS) for ExampleOrg
Financial Solutions Pvt Ltd, aligned to ISO/IEC 27001:2022, suitable for a Stage 1/Stage 2
certification audit.

## Scope of work
1. **ISMS Scope Statement** — defines the boundary of the management system
2. **Risk Assessment Methodology** — the repeatable process used to identify and score risk
3. **Risk Register** — 15 identified risks, scored, treated, and owned
4. **Statement of Applicability (SoA)** — all 93 Annex A:2022 controls, applicability decision, and justification
5. **Core Policies** — 5 policies that operationalize the ISMS

## Methodology used
Risk assessment follows an asset-based approach (ISO 27005-aligned): identify information
assets → identify threats/vulnerabilities per asset → score likelihood × impact → determine
risk treatment → map to Annex A controls in the SoA.

## Key findings (executive summary)
- 15 risks identified across the asset inventory; **4 rated Critical/High**, concentrated in
  cloud infrastructure access management and third-party data sharing
- SoA shows **88 of 93 controls applicable** (including 8 inherited via the AWS Shared
  Responsibility Model); only **5 controls marked Not Applicable**, all physical
  server-room/hardware controls that don't apply because ExampleOrg is fully cloud-hosted on AWS
- Two policy gaps closed: Incident Response and Business Continuity had no formal documentation
  prior to this exercise — both are now drafted and ready for management approval

## Files in this folder
| File | Purpose |
|---|---|
| `scope-statement.md` | ISMS boundary definition |
| `risk-assessment-methodology.md` | Scoring criteria and treatment process |
| `risk-register.csv` | 15 scored and treated risks |
| `statement-of-applicability.csv` | All 93 Annex A controls with applicability + justification |
| `policies/` | 5 core ISMS policies |
