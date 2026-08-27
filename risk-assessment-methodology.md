# Risk Assessment Methodology

**Aligned to:** ISO/IEC 27001:2022 Clause 6.1.2, cross-referenced with ISO 27005 and NIST CSF 2.0 (Identify function)

## 1. Approach
ExampleOrg uses an **asset-based risk assessment methodology**. For each critical information
asset, we identify applicable threats and vulnerabilities, then score the resulting risk.

## 2. Process steps
1. **Asset identification** — inventory all information assets in scope (systems, data stores, processes)
2. **Threat & vulnerability identification** — for each asset, identify realistic threat sources and exploitable vulnerabilities
3. **Likelihood scoring** (1–5) — probability of the threat exploiting the vulnerability in the next 12 months
4. **Impact scoring** (1–5) — business impact across Confidentiality, Integrity, Availability if realized
5. **Risk score** = Likelihood × Impact (range 1–25)
6. **Risk rating band** applied
7. **Risk treatment decision** — Mitigate / Transfer / Avoid / Accept
8. **Control mapping** — map treatment to specific Annex A:2022 control(s)
9. **Owner assignment** and target closure date
10. **Residual risk re-scoring** post-treatment

## 3. Likelihood scale
| Score | Rating | Definition |
|---|---|---|
| 1 | Rare | Not expected to occur; no known precedent |
| 2 | Unlikely | Could occur but no history in this environment |
| 3 | Possible | Might occur at some point; some precedent in industry |
| 4 | Likely | Will probably occur; has occurred elsewhere in similar orgs |
| 5 | Almost Certain | Expected to occur; active exploitation trends observed |

## 4. Impact scale
| Score | Rating | Definition |
|---|---|---|
| 1 | Negligible | No material impact to operations, data, or reputation |
| 2 | Minor | Localized impact, no regulatory/customer notification required |
| 3 | Moderate | Service disruption or limited data exposure; internal escalation required |
| 4 | Major | Significant customer data exposure, regulatory notification triggered, media risk |
| 5 | Severe | Large-scale breach, RBI/regulatory action, material financial/reputational damage |

## 5. Risk rating bands
| Risk Score | Band | Response SLA |
|---|---|---|
| 1–4 | Low | Accept / monitor annually |
| 5–9 | Medium | Treat within 6 months |
| 10–15 | High | Treat within 90 days |
| 16–25 | Critical | Treat within 30 days, escalate to CISO immediately |

## 6. Risk treatment options
- **Mitigate** — implement/strengthen a control to reduce likelihood or impact
- **Transfer** — shift risk via insurance or contractual liability (e.g., vendor DPA/SLA)
- **Avoid** — discontinue the activity/process generating the risk
- **Accept** — formally accept residual risk (requires CISO/leadership sign-off, documented)

## 7. Review cadence
- Full risk register review: quarterly
- Critical/High risks: monthly progress check by CISO
- Ad hoc reassessment: triggered by new system launches, M&A, major incidents, or regulatory change
