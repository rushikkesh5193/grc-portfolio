# Gap Assessment Methodology

## 1. Approach
Each requirement area under the DPDP Act 2023 is assessed against ExampleOrg's current
practice and scored on a 4-point compliance maturity scale, then assigned a remediation
priority based on both the compliance gap and the underlying data risk.

## 2. Compliance Maturity Scale
| Rating | Definition |
|---|---|
| **Compliant** | Requirement is met, with a documented and operational process/control |
| **Partially Compliant** | Practice exists informally, or is met for some but not all data flows; needs formalization |
| **Non-Compliant** | No process or control currently exists to meet this requirement |
| **Not Applicable** | Requirement does not apply to ExampleOrg's data processing activities |

## 3. Priority Scoring
Remediation priority = f(Compliance Gap, Data Sensitivity, Regulatory/Enforcement Risk)

| Priority | Criteria |
|---|---|
| **P1 - Critical** | Non-Compliant AND involves sensitive personal/financial data, or core lawful-basis requirement (consent) |
| **P2 - High** | Non-Compliant on a lower-sensitivity area, OR Partially Compliant on a high-sensitivity area |
| **P3 - Medium** | Partially Compliant on a lower-sensitivity/procedural requirement |
| **P4 - Low** | Minor documentation or process refinement needed |

## 4. Requirement Areas Assessed
Requirement areas were derived from the core obligations under the DPDP Act 2023:
consent and notice (Sections 5-7), Data Principal rights (Sections 11-14), significant
data fiduciary obligations (Section 10), data breach notification (Section 8(6)),
data retention and erasure (Section 8(7)), cross-border data transfer (Section 16),
children's data (Section 9), and grievance redressal (Section 13).

## 5. Data Sources Used for Assessment
- Interviews (simulated) with Engineering, Customer Support, and Vendor Management leads
- Review of existing privacy notice / terms of service language
- Review of data flows into and out of the KYC vendor and payment gateway
- Review of current customer support process for data-related requests

## 6. Review Cadence
This gap assessment is a point-in-time exercise; ExampleOrg's GRC function re-runs the full
assessment upon: (a) finalization of DPDP Rules, (b) any material change to data processing
activities, or (c) annually at minimum.
