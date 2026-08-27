# Sample Completed Vendor Risk Assessment

**Vendor:** [KYC Verification Vendor] (fictional, referred to as "VerifyID Pvt Ltd")
**Assessment Date:** [Date]
**Assessed By:** GRC Analyst
**Vendor Tier:** Tier 1 — Critical (per Vendor Tiering Methodology: handles KYC identity documents, direct API integration with lending platform)

## 1. Summary of Vendor Responses

| Section | Key Findings | Section Score (0-4) |
|---|---|---|
| A: Certification & Track Record | No SOC 2 or ISO 27001 certification held; vendor states certification is "in progress, targeting completion in 8 months." No disclosed breach history. | 2 |
| B: Data Handling | Data stored in India-based data center (good). AES-256 encryption at rest confirmed. TLS 1.2 in transit. Retention policy exists but deletion process is manual, not automated — flagged. One subprocessor (OCR/document parsing tool) disclosed, no independent assessment done by vendor. | 3 |
| C: Access Control & Authentication | MFA enforced for all staff. RBAC model documented. Access reviewed quarterly. Background checks confirmed for all staff with data access. | 4 |
| D: Application & Infrastructure Security | Annual penetration test conducted (report reviewed, no critical findings open >30 days). Patch SLA: 14 days for critical vulnerabilities — acceptable but not best-in-class. No formal SSDLC documentation provided. | 3 |
| E: Incident Response & Business Continuity | Documented incident response plan exists, last tested 14 months ago (slightly overdue against typical 12-month cadence). Breach notification commitment: 48 hours. DR plan exists, RTO of 8 hours for their core verification service. | 3 |
| F: Compliance & Legal | Willing to sign ExampleOrg DPA with minor negotiated changes. No designated DPO, but has a named privacy contact. Vendor is not yet DPDP Act compliant in a documented way — in progress. | 2 |
| G: Right to Audit | Accepts right-to-audit clause with 30 days' notice. | 4 |

## 2. Composite Score Calculation

| Section | Score | Weight | Weighted Score |
|---|---|---|---|
| A | 2 | 20% | 0.40 |
| B | 3 | 20% | 0.60 |
| C | 4 | 15% | 0.60 |
| D | 3 | 20% | 0.60 |
| E | 3 | 15% | 0.45 |
| F | 2 | 5% | 0.10 |
| G | 4 | 5% | 0.20 |
| **Total (out of 4, scaled to 100)** | | | **2.95 / 4 → 74/100** |

## 3. Risk Rating: **Medium Risk (65-84 band)**

## 4. Assessment Narrative
VerifyID demonstrates solid operational security practices — strong access control,
reasonable infrastructure security, and a functioning incident response and BCP program.
However, the **absence of an independent security certification (SOC 2/ISO 27001)** is a
material gap for a vendor entrusted with government ID documents and KYC data — this is
the single factor most holding back a higher score, and is consistent with what an
attentive reviewer would flag as the top follow-up item.

The **manual data deletion process** (Section B) is also a concern: without automation,
retention-period enforcement is subject to human error, creating a downstream DPDP Act
compliance risk for ExampleOrg (this links to Gap DP-10 in the DPDP Gap Assessment project).

## 5. Conditions for Approval
Per the scoring rubric, a Medium Risk rating permits approval with conditions. The
following remediation plan is required within 90 days of contract execution/renewal:

| Action | Owner (Vendor) | Target Date |
|---|---|---|
| Provide quarterly progress updates on SOC 2/ISO 27001 certification timeline | VerifyID | Ongoing |
| Automate data deletion process at retention expiry | VerifyID | Within 90 days |
| Conduct independent security assessment of OCR subprocessor | VerifyID | Within 120 days |
| Re-test incident response plan (currently 14 months since last test) | VerifyID | Within 60 days |
| Provide documented DPDP Act compliance status update | VerifyID | Within 90 days |

## 6. Recommendation
**Approve for continued engagement with conditions above.** Escalate to CISO for
sign-off per Tier 1 vendor requirement. Schedule follow-up review at 90 days to confirm
remediation progress; if certification progress stalls beyond the vendor's stated timeline,
recommend re-scoring and evaluating alternative vendors given the sensitivity of data involved.

## 7. Approval
| Role | Name | Decision | Date |
|---|---|---|---|
| GRC Analyst (Assessor) | [Name] | Recommend Approve with Conditions | [Date] |
| CISO | [Name] | [Pending] | [Date] |
