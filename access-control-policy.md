# Access Control Policy

| | |
|---|---|
| **Document Owner** | Head of Infrastructure |
| **Approved By** | CISO |
| **Version** | 1.0 |
| **Maps to Annex A Controls** | A.5.15, A.5.16, A.5.17, A.5.18, A.8.2, A.8.3, A.8.5 |
| **Review Cycle** | Annual |

## 1. Purpose
To ensure access to ExampleOrg's systems and data is granted, reviewed, and revoked in a
manner that enforces least privilege and prevents unauthorized access to customer and
corporate data.

## 2. Policy Statements

### 2.1 Access provisioning
- Access is granted strictly on a need-to-know, least-privilege basis, tied to job role.
- All access requests require manager approval and are logged in the access management system.
- Standard access is provisioned within 2 business days of approval; privileged/admin access
  requires additional CISO sign-off.

### 2.2 Authentication
- Multi-factor authentication (MFA) is mandatory for all systems containing customer PII,
  all cloud infrastructure admin consoles, and all privileged/root accounts, without exception.
- Passwords must meet minimum complexity (12+ characters, no dictionary words) and are
  never shared or reused across systems.
- Service accounts must use rotated credentials or short-lived tokens, not static passwords.

### 2.3 Privileged access
- Privileged (admin/root) access is restricted to a named list of approved personnel,
  reviewed monthly.
- All privileged actions on production systems are logged and retained for a minimum of 12 months.
- Break-glass emergency access procedures require post-use justification within 24 hours.

### 2.4 Access review
- All user access is formally reviewed quarterly by the relevant department head and Head of GRC.
- Access that is no longer required is revoked within 5 business days of the review.

### 2.5 Access revocation (offboarding)
- Upon termination or role change, system access must be revoked or adjusted within
  24 hours, coordinated between HR and IT per the automated deprovisioning workflow.
- Immediate revocation applies for involuntary terminations, coordinated in real time
  between HR and IT.

### 2.6 Third-party access
- Any third party requiring access to ExampleOrg systems must be covered by a signed NDA
  and, where applicable, a Data Processing Agreement.
- Third-party access is time-bound and reviewed at the same cadence as employee access.

## 3. Exceptions
Any exception to this policy requires documented, time-bound approval from the CISO and
must be logged in the risk register if it introduces residual risk.

## 4. Related Documents
- Information Security Policy
- Incident Response Policy
- Risk Register (see R-001, R-006 for related identified gaps)
