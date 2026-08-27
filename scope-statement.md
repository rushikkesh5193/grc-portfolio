# ISMS Scope Statement

**Document Owner:** CISO / Head of GRC
**Version:** 1.0
**Status:** Approved for certification audit
**Review cycle:** Annual, or upon material change to business/infrastructure

## 1. Purpose
This document defines the boundary of the Information Security Management System (ISMS) for
ExampleOrg Pvt Ltd, in accordance with ISO/IEC 27001:2022 Clause 4.3.

## 2. Scope Statement
The ISMS covers the people, processes, and technology involved in the design, development,
hosting, and operation of ExampleOrg's digital lending and payments aggregation platform,
including the handling of customer PII, KYC data, and transaction data, for all operations
conducted from ExampleOrg's Bengaluru office and remote engineering locations within India.

## 3. In-scope boundaries

### 3.1 Organizational
- Engineering, Product, Customer Support, and GRC/Security functions
- Bengaluru HQ and all remote employees accessing corporate systems

### 3.2 Systems & Infrastructure
- AWS-hosted production and staging environments (ap-south-1 region)
- Core lending microservices platform
- Payments gateway integration layer
- Salesforce CRM (customer data)
- Darwinbox HRMS (employee data)
- Corporate endpoints (laptops) issued to employees

### 3.3 Data
- Customer PII (name, address, phone, email)
- KYC documents (PAN, Aadhaar-linked identifiers, bank statements)
- Bank account and transaction data
- Employee personal data

### 3.4 Third parties in scope
- Cloud infrastructure provider (AWS)
- Payment gateway processor
- KYC verification vendor
- Cloud-based CRM and HRMS vendors

## 4. Out of scope
- Physical data center controls (ExampleOrg does not own or operate physical data centers;
  physical/environmental security is inherited from AWS and assessed via their SOC 2 report,
  not independently audited by ExampleOrg)
- Marketing website (public, no authentication, no customer data collected)
- Any subsidiary or group company outside ExampleOrg Pvt Ltd

## 5. Interfaces and dependencies
| Interface | Dependency | Owner |
|---|---|---|
| AWS Shared Responsibility Model | Physical/infrastructure security controls | AWS (inherited, reviewed via SOC 2) |
| Payment gateway PCI DSS compliance | Card data environment security | Payment gateway vendor (attested via AOC) |
| KYC vendor data handling | Identity verification data processing | KYC vendor (contractual DPA in place) |

## 6. Justification for exclusions
Physical/environmental controls (ISO Annex A.7 series) are largely marked "applicable via
inherited control" rather than "not applicable" — see Statement of Applicability for the
control-by-control justification.

## 7. Approval
| Role | Name | Date |
|---|---|---|
| CISO | [Name] | [Date] |
| CEO | [Name] | [Date] |
