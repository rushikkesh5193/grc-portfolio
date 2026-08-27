# Business Continuity Policy

| | |
|---|---|
| **Document Owner** | Head of Infrastructure |
| **Approved By** | CISO |
| **Version** | 1.0 |
| **Maps to Annex A Controls** | A.5.29, A.5.30, A.8.14 |
| **Review Cycle** | Annual |
| **Note** | This policy directly closes gap identified as Risk R-012 in the ISMS risk register |

## 1. Purpose
To ensure ExampleOrg can maintain or rapidly restore critical business operations —
specifically the lending and payments platform — in the event of a disruptive incident.

## 2. Scope
Covers the AWS-hosted production environment, core lending microservices, payments gateway
integration, and the customer support function required to serve existing customers during
a disruption.

## 3. Business Impact Analysis (summary)
| System | Criticality | Max Tolerable Downtime (RTO) | Max Tolerable Data Loss (RPO) |
|---|---|---|---|
| Core lending platform (loan origination/servicing) | Critical | 4 hours | 15 minutes |
| Payments gateway integration | Critical | 2 hours | 5 minutes |
| Customer support (CRM access) | High | 8 hours | 1 hour |
| Internal corporate systems (email, HRMS) | Medium | 24 hours | 4 hours |
| Marketing website | Low | 72 hours | 24 hours |

## 4. Policy Statements
1. ExampleOrg shall maintain a documented and tested Disaster Recovery (DR) plan for all
   Critical and High criticality systems identified above.
2. Production data shall be backed up per the defined RPO, encrypted, and stored in a
   separate AWS Availability Zone / region from the primary environment.
3. A full DR failover test shall be conducted at minimum annually, with results documented
   and gaps remediated within 60 days.
4. An incident affecting service availability shall be handled jointly under this policy
   and the Incident Response Policy where the disruption has a security root cause.
5. A Business Continuity communication plan shall be maintained defining how customers,
   regulators, and employees are informed during an extended outage.

## 5. Roles and Responsibilities
| Role | Responsibility |
|---|---|
| Head of Infrastructure | Owns DR architecture, backup strategy, and failover testing |
| CISO | Approves BCP, ensures alignment with incident response |
| Head of Customer Support | Owns customer communication plan during outages |
| All department heads | Maintain department-level continuity procedures for critical functions |

## 6. Recovery Strategy (summary)
- **Infrastructure**: Multi-AZ deployment on AWS with automated failover for the production
  database and core services.
- **Data**: Automated encrypted backups per RPO targets above, tested via periodic
  restore drills.
- **Communication**: Status page and customer notification template pre-approved by Legal
  and Communications for use during an active incident.

## 7. Testing and Review
DR test results, along with any tabletop business continuity exercise, are reviewed by the
CISO and documented as evidence for the annual ISMS management review.

## 8. Related Documents
- Incident Response Policy
- Information Security Policy
- Risk Register (R-012)
