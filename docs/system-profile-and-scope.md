# FCMS-001 — System Profile and Scope

**Document status:** Draft  
**Version:** 1.0  
**System ID:** FCMS-001  
**Environment:** Simulated AWS-hosted federal information system

## 1. Purpose

This document establishes the purpose, scope, information types, conceptual architecture, system boundary, assumptions, and external dependencies for the fictional Federal Case Management System (FCMS-001).

The document will provide the foundation for subsequent security categorization, control selection, assessment planning, risk analysis, and remediation documentation.

This is a portfolio simulation. It does not describe an actual federal system or an approved security authorization.

## 2. System Overview

### 2.1 Business Purpose

FCMS-001 is a fictional application used by authorized federal agency employees to create, review, update, and track administrative case records.

The system stores case-related personal information, maintains case histories, and supports the storage and retrieval of documents associated with individual cases.

### 2.2 Business Objectives

- **Confidentiality:** Protect personal information and case documents from unauthorized disclosure.
- **Integrity:** Preserve the accuracy and completeness of case records, decisions, and action histories.
- **Availability:** Maintain access to case processing capabilities consistent with mission requirements.
- **Accountability:** Record relevant user and administrative actions to support review and investigation.
- **Operational continuity:** Support recovery from service disruptions and data loss.

### 2.3 Primary Users

- Case-processing employees
- Supervisors and case reviewers
- Authorized system administrators
- Security personnel responsible for monitoring and investigation

Specific roles and permissions remain to be defined during control selection.

## 3. Information Inventory

The proposed system processes or maintains the following information types:

| Information type | Example contents | Primary security concerns |
|---|---|---|
| Personally identifiable information (PII) | Names, contact details, case identifiers | Confidentiality and privacy |
| Case records | Case status, notes, supporting facts | Confidentiality and integrity |
| Decisions and case history | Decisions, dates, action history | Integrity and accountability |
| Supporting documents | Forms and attachments | Confidentiality and integrity |
| User and access records | User identifiers, roles, access assignments | Confidentiality and unauthorized access |
| Audit logs | Login events, administrative actions, record changes | Accountability and investigation |
| System configuration | Application settings and security configuration | Integrity and security |
| Operational metadata | Service health and error records | Availability and troubleshooting |

The exact data elements, retention requirements, and applicable privacy or information-handling requirements have not yet been established.

**Initial assumption:** The system contains sensitive case-related PII but does not process classified information. This assumption must be revisited if the scenario's information requirements change.

## 4. Conceptual Architecture

The proposed architecture consists of:

- A web-based case management application.
- A managed relational database for structured case records.
- Object storage for supporting documents.
- Identity and access management services.
- Encryption and key-management capabilities.
- Logging and monitoring services.
- External agency or cloud-provider services supporting the system.

The architecture is conceptual. Specific AWS services, network paths, account structure, and implementation details have not yet been validated.

Intended security capabilities are design requirements, not verified evidence of implementation.

## 5. Proposed System Boundary

### 5.1 Components Within Scope

The initial proposed authorization boundary includes:

- The case management application and application runtime.
- The managed database containing case records.
- Object storage containing case documents.
- System-specific identity and access configuration.
- System-specific encryption configuration and key usage.
- System-specific logging and monitoring configuration.
- Relevant deployment artifacts, system configuration, and administrative interfaces.

### 5.2 External Dependencies

The following are treated as external dependencies pending confirmation of ownership and authorization boundaries:

- Underlying AWS cloud infrastructure.
- Separately managed agency identity services.
- Employee workstations and the general agency network.
- External systems exchanging approved case information.
- Organization-wide security services operated by separate control providers.

These exclusions do not remove their security relevance. Connections, responsibilities, and potentially inherited controls must be documented.

### 5.3 Boundary Limitations

The boundary is provisional. It must be refined after identifying the specific cloud services, data flows, system interfaces, administrative responsibilities, and applicable common controls.

## 6. Initial Security Considerations

The following areas require further analysis:

- Unauthorized disclosure of case-related PII.
- Unauthorized modification or deletion of case records.
- Compromise of user or administrator credentials.
- Inadequate logging or delayed detection of suspicious activity.
- Loss of access caused by service disruption or data loss.
- Risks associated with external connections and inherited cloud controls.

These are preliminary risk areas, not confirmed findings.

## 7. Initial Security Categorization Hypothesis

Moderate impact is the initial hypothesis for confidentiality, integrity, and availability. No final FIPS 199 categorization has been established.

Each security objective must be evaluated against the potential consequences of unauthorized disclosure, modification, or loss of availability. The rationale and resulting overall categorization will be documented separately in the Security Categorization Worksheet.

## 8. Assumptions and Open Questions

1. What exact categories of personal information are processed?
2. What harm could disclosure cause to affected individuals or agency operations?
3. What consequences could result from inaccurate or unauthorized changes to case records?
4. How long could the system be unavailable before mission operations are seriously affected?
5. Which AWS services, accounts, regions, and network components are in scope?
6. Which identity, logging, encryption, and security services are managed externally?
7. What external interfaces and data exchanges exist?
8. What backup, restoration, retention, and audit-log requirements apply?
9. Which privacy and information-handling requirements apply?
10. Which controls are inherited, shared, or implemented directly by the system owner?

## 9. Document Limitations

This document describes a fictional system and a proposed scope. It does not establish that any security control is implemented or effective. All future evidence, test results, findings, and authorization recommendations must be clearly identified as simulated or synthetic.

The system boundary, impact categorization, and control responsibilities remain subject to refinement as the project develops.
