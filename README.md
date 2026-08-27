# GRC Portfolio — ExampleOrg Pvt Ltd

This repository contains three end-to-end GRC work products built against a single fictional
organization, **ExampleOrg Pvt Ltd**, to demonstrate applied GRC capability
across information security management, Indian data protection compliance, and third-party risk.

## Why one fictional company across all three projects
Real GRC work never happens in isolation — an ISMS risk register, a DPDP gap assessment, and a
vendor risk program for the same organization all reference the same assets, the same data flows,
and the same risk appetite. Using one consistent company profile across all three projects
demonstrates how these programs interlock in practice, the way they would inside a real
GRC function.

## Company Profile (fictional, used across all projects)
| Attribute | Detail |
|---|---|
| Name | ExampleOrg Pvt Ltd |
| Sector | Fintech — digital lending & payments aggregation |
| HQ | Bengaluru, India, with a remote engineering team |
| Size | ~220 employees |
| Regulatory exposure | RBI (NBFC-adjacent lending guidelines), DPDP Act 2023, PCI DSS (card data via payment aggregator model) |
| Core systems | AWS-hosted microservices platform, Salesforce CRM, a payments gateway integration, HR system (Darwinbox), 12 active third-party vendors |
| Data handled | Customer PII, KYC documents, bank account details, transaction history |

## Repository Structure

```
grc-portfolio/
├── 01-iso27001-isms/              # Full ISO 27001:2022 ISMS implementation kit
│   ├── README.md
│   ├── scope-statement.md
│   ├── risk-assessment-methodology.md
│   ├── risk-register.csv
│   ├── statement-of-applicability.csv
│   └── policies/                  # 5 core ISMS policies
│
├── 02-dpdp-act-gap-assessment/    # DPDP Act 2023 compliance gap assessment
│   ├── README.md
│   ├── gap-assessment-methodology.md
│   ├── data-processing-inventory.csv
│   ├── compliance-gap-tracker.csv
│   └── executive-summary.md
│
└── 03-vendor-risk-management/     # Third-Party Risk Management (TPRM) program
    ├── README.md
    ├── vendor-tiering-methodology.md
    ├── vendor-risk-questionnaire.md
    ├── vendor-risk-scoring-rubric.md
    ├── sample-vendor-assessment.md
    └── vendor-risk-register.csv
```

## How to read this repository
Each project folder has its own README explaining the objective, methodology, and key findings —
read that first, then the supporting artifacts. The CSV registers open cleanly in Excel/Google
Sheets and are also viewable directly on GitHub.

## Frameworks referenced
ISO/IEC 27001:2022 (Annex A controls), NIST CSF 2.0 (cross-referenced in the ISMS risk methodology),
DPDP Act 2023 & draft DPDP Rules, RBI IT Governance & digital lending guidelines, PCI DSS v4.0
(vendor tiering context).

## About this portfolio
Built to demonstrate applied GRC skills: risk assessment methodology design, control mapping,
policy authorship, regulatory gap analysis, and third-party risk program design — the day-to-day
output of a GRC analyst/associate role.


