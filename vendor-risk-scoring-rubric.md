# Vendor Risk Scoring Rubric

## 1. Purpose
To convert questionnaire responses into a consistent risk score, enabling comparison
across vendors and a defensible basis for onboarding/renewal decisions.

## 2. Scoring Categories
Each questionnaire section is scored 0–4, then weighted by relevance to produce a
composite score out of 100.

| Section | Weight |
|---|---|
| A: Certification & Track Record | 20% |
| B: Data Handling | 20% |
| C: Access Control & Authentication | 15% |
| D: Application & Infrastructure Security | 20% |
| E: Incident Response & Business Continuity | 15% |
| F: Compliance & Legal | 5% |
| G: Right to Audit | 5% |

## 3. Section Scoring Guide (example: Section A)
| Score | Criteria |
|---|---|
| 4 (Excellent) | Current SOC 2 Type II or ISO 27001 certification, no breach history, evidence attached |
| 3 (Good) | Certification in progress / recently expired, no material breach history |
| 2 (Adequate) | No formal certification, but strong documented internal security program |
| 1 (Weak) | No certification, minimal documented security program |
| 0 (Unacceptable) | No certification, undisclosed or unresolved breach history |

*(Equivalent scoring guides are applied per section based on the specific questionnaire responses — e.g., Section B scores highest when data is encrypted at rest/in transit, retention/deletion is clearly defined, and no unreviewed subprocessors are used.)*

## 4. Composite Score → Risk Rating
| Composite Score | Risk Rating | Outcome |
|---|---|---|
| 85–100 | Low Risk | Approved for onboarding/renewal; standard review cycle applies |
| 65–84 | Medium Risk | Approved with conditions (remediation plan required within 90 days); enhanced monitoring |
| 45–64 | High Risk | Requires CISO approval; remediation plan mandatory before onboarding, or contract renewal held pending fixes |
| Below 45 | Critical Risk | Onboarding not recommended; existing vendors escalated for contract review/exit planning |

## 5. Weighting Rationale
Data Handling and Application/Infrastructure Security are weighted highest (20% each)
because they represent the areas most directly tied to likelihood and impact of a data
breach — consistent with the risk scoring approach used in the ISO 27001 risk register
(Project 1), keeping methodology consistent across ExampleOrg's GRC program.

## 6. Reassessment Triggers
A vendor is reassessed outside the normal cycle if: a security incident occurs at the
vendor, the vendor's certification lapses, the scope of data shared changes materially,
or a subprocessor change is disclosed.
