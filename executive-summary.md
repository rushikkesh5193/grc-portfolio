# Executive Summary: DPDP Act 2023 Compliance Gap Assessment

**Prepared for:** ExampleOrg Pvt Ltd — Executive Leadership Team
**Prepared by:** GRC Function
**Date:** [Date]
**Classification:** Internal — Confidential

## Purpose
This assessment evaluated ExampleOrg's current data handling practices against the
requirements of the Digital Personal Data Protection Act, 2023, across 20 requirement
areas spanning consent, Data Principal rights, breach notification, retention, vendor
management, and governance obligations.

## Headline Findings
Of 20 requirement areas assessed:
- **7 are Non-Compliant** — no process or control currently exists
- **11 are Partially Compliant** — informal practice exists but is not formalized or complete
- **1 is fully Compliant**
- **1 is Not Applicable** to ExampleOrg's current product scope

**Bottom line:** ExampleOrg has strong underlying technical security controls (driven by
existing PCI DSS obligations), but has **not yet built the DPDP-specific governance layer**
— consent granularity, Data Principal rights fulfillment, breach notification timelines,
and Significant Data Fiduciary readiness are the areas of greatest exposure.

## Top 4 Risk Areas Requiring Immediate Attention

**1. No granular, purpose-specific consent mechanism (DP-01)**
Customers currently give one broad consent checkbox covering all processing purposes.
The Act requires consent to be specific to each purpose. This is a foundational lawful-basis
gap — nearly every downstream processing activity relies on this consent being valid.

**2. No operational process for Data Principal rights requests (DP-04, DP-05)**
There is currently no defined way for a customer to formally request access to, correction
of, or erasure of their data within a defined timeline. This is both a compliance gap and
an operational risk — if a request comes in today, there is no playbook to fulfill it
correctly, especially given the tension between erasure rights and the 7-year RBI retention
requirement on financial records.

**3. No formal breach notification process aligned to DPDP timelines (DP-08)**
This gap is also flagged in the parallel ISO 27001 risk assessment (Risk R-011). A breach
today would have no defined path to timely Board and Data Principal notification, creating
regulatory exposure on top of reputational risk.

**4. Significant Data Fiduciary status not yet assessed (DP-13)**
ExampleOrg processes financial and KYC data at meaningful scale. Whether this crosses the
threshold for "Significant Data Fiduciary" obligations (DPO appointment, DPIA, independent
audit) has not been formally evaluated — this should be resolved early, as it changes the
compliance obligations across several other requirement areas.

## Recommended Approach
Given resource constraints, remediation is sequenced by priority (P1 first) rather than
attempted simultaneously:

| Phase | Focus | Target |
|---|---|---|
| Phase 1 (0–90 days) | Close all P1 items: consent mechanism, DP rights process, breach notification, SDF assessment | 2026-10-31 |
| Phase 2 (90–180 days) | Close P2 items: notice redesign, vendor DPA updates, DPIA process, cross-border review | 2026-12-31 |
| Phase 3 (180+ days) | Close remaining P3/P4 items: training, cookie consent, form minimization | 2027-Q1 |

## Resourcing Ask
This roadmap requires coordinated effort across GRC, Legal, Product, and Engineering.
Recommend a dedicated cross-functional working group with biweekly check-ins against the
compliance gap tracker until Phase 1 items are closed.

## Next Steps
1. Leadership sign-off on this remediation roadmap and priority sequencing
2. Formal SDF threshold assessment (Legal + GRC) — this determines scope of several other items
3. Kick off consent mechanism redesign with Product (longest lead-time item)
