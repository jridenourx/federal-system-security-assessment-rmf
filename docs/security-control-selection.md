# Security Control Selection — FCMS-001

**Document Status:** Draft — Simulation  
**System ID:** FCMS-001  
**Assessment Phase:** Security Control Selection  
**Reference Framework:** NIST SP 800-53 Revision 5  
**Categorization Basis:** Preliminary FIPS 199 assessment

## 1. Purpose

This document establishes a preliminary approach for selecting security controls for the fictional Federal Benefits Case Management System (FCMS-001).

The proposed system categorization is Moderate overall, based on Moderate confidentiality, Moderate integrity, and Low availability impact ratings. These ratings remain preliminary and require validation.

The control selection process considers the system's information, operational purpose, security risks, and reliance on external services.

## 2. Control Selection Approach

The assessment will use NIST SP 800-53 Revision 5 as the security control catalog.

The initial approach is to:

1. Use the validated system impact categorization to determine an appropriate starting control baseline.
2. Identify controls relevant to the system's architecture, information, and operating environment.
3. Identify responsibilities shared with the cloud service provider or agency enterprise services.
4. Document tailoring decisions and explain why controls are included, excluded, or inherited.
5. Assess whether selected controls are implemented and operating effectively during a later assessment phase.

**Important:** This document identifies proposed controls. It does not demonstrate that controls are implemented, tested, or compliant.

## 3. Proposed Control Areas

The following control areas are initial priorities for FCMS-001. They are not a complete or formally approved NIST baseline.

| Control family | Proposed focus | Reason for selection |
|---|---|---|
| Access Control (AC) | Least privilege, role-based permissions, account management | Restrict access to applicant records and administrative functions |
| Identification and Authentication (IA) | User authentication, administrator authentication, account lifecycle | Reduce unauthorized access to the system |
| Audit and Accountability (AU) | Event logging, log protection, review and retention | Support investigations and accountability for access and changes |
| Configuration Management (CM) | Secure configurations, configuration changes, baseline management | Reduce exposure from insecure or unauthorized changes |
| System and Communications Protection (SC) | Communications protection, boundary controls, encryption | Protect information in transit and at rest |
| System and Information Integrity (SI) | Vulnerability management, flaw remediation, security monitoring | Identify and address technical weaknesses |
| Contingency Planning (CP) | Backup, recovery, and contingency procedures | Support restoration following disruption |
| Risk Assessment (RA) | Risk assessment, vulnerability identification, risk documentation | Maintain visibility into security risks |
| Incident Response (IR) | Incident handling, reporting, and response procedures | Establish a response process for suspected security incidents |
| Supply Chain Risk Management (SR) | Cloud-service dependencies and third-party risk | Address risks arising from external service providers |

## 4. Shared and Inherited Responsibilities

FCMS-001 is assumed to operate in AWS and rely on separate agency services. Some security responsibilities may be provided by the cloud provider or agency, while others must be implemented by the system team.

| Responsibility area | Preliminary responsibility assumption | Evidence needed |
|---|---|---|
| Physical data center security | AWS-managed, subject to the selected service and applicable agreements | Relevant provider assurance documentation |
| Cloud infrastructure security | Shared; specific responsibilities depend on the AWS service model | Architecture and responsibility documentation |
| Application permissions and roles | System owner and application team | Role definitions and access configuration |
| Application logging and review | Shared depending on service configuration and agency procedures | Logging configuration, review procedures, and sample records |
| Database and object-storage permissions | Primarily system configuration, with provider-managed underlying infrastructure | Database and storage access settings |
| Agency identity integration | Agency and system team responsibilities to be confirmed | Identity architecture and integration configuration |
| Backup and recovery | System owner and cloud-service configuration responsibilities to be confirmed | Backup settings, recovery procedures, and test results |

These assignments are working assumptions, not verified control inheritance determinations. Responsibility must be confirmed for each selected AWS service and agency dependency.

## 5. Preliminary Tailoring and Validation Questions

Before finalizing the control set, the assessment should determine:

- Which NIST SP 800-53 Moderate baseline controls apply to this system?
- Which controls are not applicable, and what is the documented justification?
- Which controls are inherited from AWS or agency enterprise services?
- Which controls are shared between the provider and the agency?
- Which system-specific controls require implementation by the application team?
- Are additional controls necessary based on the system's risks, architecture, or mission?
- What evidence will be required to assess each control?

No control should be marked implemented, inherited, effective, or compliant without supporting evidence.

## 6. Next Assessment Activities

The next activities will be to:

1. Validate the system categorization and confirm the applicable baseline.
2. Build a control matrix that identifies selected controls, implementation responsibility, assessment procedures, and required evidence.
3. Develop assessment procedures using NIST SP 800-53A.
4. Record simulated assessment results and document any findings.
5. Develop a POA&M for findings requiring remediation.

## 7. References

- NIST SP 800-53 Revision 5 — Security and Privacy Controls for Information Systems and Organizations: https://csrc.nist.gov/pubs/sp/800/53/r5/upd1/final
- NIST SP 800-53A Revision 5 — Assessing Security and Privacy Controls in Information Systems and Organizations: https://csrc.nist.gov/pubs/sp/800/53/a/r5/final
- NIST FIPS 199 — Standards for Security Categorization of Federal Information and Information Systems: https://csrc.nist.gov/pubs/fips/199/final

## 8. Simulation Disclaimer

This document is an educational simulation based on a fictional system. It is not an approved federal security plan, a completed control selection, or evidence of actual compliance with NIST requirements.
