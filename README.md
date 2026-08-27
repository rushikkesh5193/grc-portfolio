# Project 3: Third-Party Risk Management (TPRM) Program

## Objective
Design and demonstrate a functioning vendor/third-party risk management program for
ExampleOrg Pvt Ltd, covering vendor tiering, risk assessment
questionnaire design, scoring, and an example completed assessment.

## Why this matters
ExampleOrg's data flows through several third parties — a cloud provider, a payment gateway,
a KYC verification vendor, and SaaS tools handling customer and employee data. Vendor risk
is consistently one of the most commonly tested areas in GRC interviews and one of the most
underbuilt programs at growing companies, making it a high-signal project for a portfolio.

## Scope of work
1. **Vendor Tiering Methodology** — how vendors are classified by risk exposure
2. **Vendor Risk Questionnaire** — the actual assessment sent to vendors
3. **Scoring Rubric** — how questionnaire responses convert to a risk tier/score
4. **Sample Completed Assessment** — a full worked example for ExampleOrg's KYC vendor
5. **Vendor Risk Register** — tracks all 12 vendors, their tier, and review status

## Key findings (from the sample assessment + register)
- Of ExampleOrg's 12 active vendors, **3 are Tier 1 (Critical)**: the KYC verification
  vendor, the payment gateway processor, and AWS
- The KYC vendor (sample assessment) scored **Medium-High risk** — strong technical
  controls but **no evidence of an independent security certification** (no SOC 2 or
  ISO 27001), which is a material gap for a vendor handling identity documents
- **2 of 12 vendors have never had a formal risk assessment conducted**, both onboarded
  before the TPRM program existed — flagged for retrospective assessment

## Files in this folder
| File | Purpose |
|---|---|
| `vendor-tiering-methodology.md` | How vendors are classified into risk tiers |
| `vendor-risk-questionnaire.md` | The standard vendor security questionnaire |
| `vendor-risk-scoring-rubric.md` | How responses are scored |
| `sample-vendor-assessment.md` | Worked example — KYC verification vendor |
| `vendor-risk-register.csv` | All 12 vendors tracked by tier and assessment status |
