# Vendor Tiering Methodology

## 1. Purpose
To classify all third-party vendors by risk exposure so that assessment depth, contract
requirements, and review frequency are proportionate to the actual risk each vendor poses.

## 2. Tiering Criteria
Each vendor is tiered based on three factors:

| Factor | Consideration |
|---|---|
| **Data access** | Does the vendor access, store, or process customer PII, KYC data, or financial data? |
| **System integration depth** | Does the vendor have direct system/API access to production systems, or is it a standalone tool? |
| **Business criticality** | Would a vendor outage or failure disrupt ExampleOrg's ability to operate (lending, payments, support)? |

## 3. Tier Definitions

### Tier 1 — Critical
Vendor has access to sensitive customer data (PII, KYC, financial) AND/OR is critical to
core business operations. A failure or breach at this vendor would materially harm
customers or the business.
- **Assessment frequency:** Full questionnaire + evidence review annually, plus contract renewal review
- **Contractual requirements:** Mandatory DPA, breach notification clause (≤72 hours), right-to-audit clause, minimum security certification (SOC 2 Type II or ISO 27001) required or formally risk-accepted
- **Examples:** AWS (infrastructure), Payment gateway processor, KYC verification vendor

### Tier 2 — High
Vendor has access to some personal data (customer or employee) but is not core-operations
critical, or has limited system integration.
- **Assessment frequency:** Full questionnaire every 18 months
- **Contractual requirements:** DPA mandatory, breach notification clause required
- **Examples:** CRM (Salesforce), HRMS (Darwinbox), email/SMS gateway

### Tier 3 — Medium
Vendor has minimal or no access to personal data, limited integration, but processes some
business-relevant information (e.g., financial/operational tools).
- **Assessment frequency:** Lightweight questionnaire every 2 years
- **Contractual requirements:** Standard confidentiality clause
- **Examples:** Accounting software, project management tools

### Tier 4 — Low
No data access, no system integration, purely transactional vendor relationship (e.g.,
office supplies, facilities).
- **Assessment frequency:** No formal security assessment required
- **Contractual requirements:** Standard commercial terms only

## 4. Tiering Process
1. New vendor onboarding request submitted by requesting department
2. GRC applies the tiering criteria above to assign initial tier
3. Tier determines which questionnaire and contract requirements apply before onboarding proceeds
4. Tier is reassessed annually or upon material change in vendor relationship (new data types shared, new integration, etc.)

## 5. Escalation
Any Tier 1 or Tier 2 vendor assessed as High or Critical risk (per the scoring rubric)
requires CISO sign-off before onboarding or contract renewal proceeds.
