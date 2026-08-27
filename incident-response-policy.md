# Incident Response Policy

| | |
|---|---|
| **Document Owner** | Head of GRC |
| **Approved By** | CISO |
| **Version** | 1.0 |
| **Maps to Annex A Controls** | A.5.24, A.5.25, A.5.26, A.5.27, A.5.28, A.6.8 |
| **Review Cycle** | Annual, or post-incident |
| **Note** | This policy directly closes gap identified as Risk R-011 in the ISMS risk register |

## 1. Purpose
To define a consistent process for identifying, reporting, assessing, containing, and
learning from information security incidents — including meeting statutory breach
notification timelines under the DPDP Act 2023 and RBI guidelines.

## 2. Definitions
- **Event**: Any observed occurrence in a system or network indicating a possible
  security-relevant condition.
- **Incident**: An event confirmed to represent an actual or imminent threat to
  confidentiality, integrity, or availability of information.
- **Breach**: An incident confirmed to involve unauthorized access, disclosure, or loss of
  personal data.

## 3. Incident Response Process

### Step 1: Detection & Reporting
Any employee, contractor, or automated monitoring system that identifies a suspected
incident must report it immediately to [email protected] or via the on-call escalation
channel. Target: report within 1 hour of detection.

### Step 2: Triage & Classification
The on-call security lead classifies the incident by severity (Critical / High / Medium /
Low) based on scope of data/systems affected, within 2 hours of report.

| Severity | Definition | Response Time |
|---|---|---|
| Critical | Confirmed customer data breach or full system compromise | Immediate, CISO paged |
| High | Suspected data exposure or significant service disruption | Within 4 hours |
| Medium | Contained security event, no confirmed data exposure | Within 1 business day |
| Low | Policy violation or minor anomaly, no security impact | Within 3 business days |

### Step 3: Containment
The response team isolates affected systems/accounts to prevent further impact
(e.g., revoke compromised credentials, isolate affected instances, block malicious IPs).

### Step 4: Investigation & Evidence Collection
Logs, system snapshots, and relevant evidence are collected and preserved per forensic
best practice (chain of custody maintained) to support root cause analysis and any
regulatory inquiry.

### Step 5: Eradication & Recovery
Root cause is remediated; affected systems are restored from clean state; enhanced
monitoring is applied to affected assets for a minimum of 30 days post-incident.

### Step 6: Regulatory & Customer Notification
For confirmed personal data breaches:
- **DPDP Act 2023**: Data Protection Board and affected Data Principals notified per
  timelines prescribed under the Act and its Rules.
- **RBI** (where applicable to lending operations): notification per RBI cybersecurity
  incident reporting framework.
- Notification content, timing, and approval routed through Head of GRC and Legal before
  external communication.

### Step 7: Post-Incident Review
A blameless post-incident review is conducted within 5 business days of resolution,
documenting root cause, timeline, response effectiveness, and corrective actions. Findings
feed back into the risk register.

## 4. Roles and Responsibilities
| Role | Responsibility |
|---|---|
| CISO | Overall incident commander for Critical/High severity |
| Head of GRC | Coordinates regulatory notification and evidence documentation |
| On-call Security Lead | First responder, triage, and containment |
| Legal | Reviews external notification language and regulatory obligations |
| Communications | Manages any required customer/public communication |

## 5. Testing
A tabletop incident response exercise is conducted at minimum annually to validate this
process, with findings documented and gaps remediated.

## 6. Related Documents
- Information Security Policy
- Business Continuity Policy
- Risk Register (R-011)
