# Security Control Selection — FCMS-001

**Document Status:** Draft — Simulation  
**Version:** 1.2  
**System ID:** FCMS-001  
**Assessment Phase:** Security Control Selection  
**Reference Framework:** NIST SP 800-53 Revision 5, Release 5.2.0  
**Baseline Reference:** NIST SP 800-53B, Release 5.2.0  
**Categorization Basis:** Preliminary FIPS 199 assessment

## 1. Purpose

This document establishes a preliminary approach for selecting security controls for the fictional Federal Benefits Case Management System (FCMS-001).

The current proposed system categorization is Moderate overall, based on Moderate confidentiality, Moderate integrity, and Low availability impact ratings. These ratings are preliminary and have not been approved.

The control selection process must use the validated security categorization, applicable federal requirements, system architecture, and organizational risk considerations to determine an appropriate starting baseline and any necessary tailoring.

This document describes a proposed selection process and priority control areas. It does not establish a formally approved control baseline or demonstrate that any control is implemented, inherited, effective, or compliant.

## 2. Control Selection Approach

NIST SP 800-53 Revision 5, Release 5.2.0 provides the security and privacy control catalog. NIST SP 800-53B, Release 5.2.0 provides the security and privacy control baselines and guidance for tailoring those baselines.

The proposed approach is to:

1. Validate the system categorization documented in `docs/security-categorization.md`.
2. Consult NIST SP 800-53B to identify the applicable starting security control baseline.
3. Confirm applicable federal requirements, agency policies, and organizational risk considerations.
4. Identify controls relevant to the system's architecture, information, and operating environment.
5. Document tailoring decisions, including controls that are applicable, not applicable, inherited, shared, or system-specific, with supporting rationale.
6. Identify implementation responsibilities for the system team, agency, and relevant service providers.
7. Develop assessment procedures and identify the evidence required to evaluate selected controls.
8. Assess control implementation and effectiveness during a subsequent assessment phase.

**Important:** The proposed Moderate categorization does not, by itself, constitute approval of a specific baseline. The applicable baseline and any tailoring decisions remain subject to validation and authorization.

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

These areas identify subjects for further analysis; they do not represent a complete list of applicable controls. Individual control identifiers, baseline assignments, enhancements, and tailoring decisions must be confirmed against the applicable NIST publications and agency requirements.

## 4. Shared and Inherited Responsibilities

FCMS-001 is assumed to operate in AWS and rely on separate agency services. Responsibilities may be divided among the cloud service provider, the agency, and the system team. The actual allocation depends on the selected services, deployment architecture, agreements, and applicable agency requirements.

| Responsibility area | Preliminary responsibility assumption | Evidence needed |
|---|---|---|
| Physical data center security | Expected to be provider-managed for the relevant AWS services, subject to verification | Applicable provider assurance documentation and service scope |
| Cloud infrastructure security | Responsibility depends on the selected AWS services and service model | Architecture documentation and applicable responsibility documentation |
| Application permissions and roles | Expected to require system-owner and application-team configuration and oversight | Role definitions, access configuration, and access-review records |
| Application logging and review | May involve provider capabilities, system configuration, and agency procedures | Logging configuration, review procedures, and sample records |
| Database and object-storage permissions | Access settings require system-level configuration and validation; underlying infrastructure responsibilities depend on the service | Database and storage access settings and relevant service documentation |
| Agency identity integration | Agency and system-team responsibilities remain to be confirmed | Identity architecture, integration configuration, and responsibility assignments |
| Backup and recovery | Responsibilities depend on service configuration, operating procedures, and agency requirements | Backup settings, recovery procedures, and recovery-test results |

These assignments are preliminary assumptions, not verified control inheritance determinations. A service provider's general security capabilities or assurance documentation does not automatically establish that a particular FCMS-001 control is inherited or adequately implemented.

Before designating a control as inherited or shared, the assessment must identify the applicable service, the specific control responsibility, the relevant supporting documentation, and any responsibilities retained by the agency or system team.

## 5. Preliminary Tailoring and Validation Questions

Before finalizing the control set, the assessment should determine:

- Has the proposed system categorization been validated and approved through the appropriate process?
- Which starting security control baseline in NIST SP 800-53B applies to the system?
- Which baseline controls and enhancements apply to FCMS-001?
- Which controls are not applicable, and what documented rationale supports each exclusion?
- Which controls are inherited from AWS or agency enterprise services, and what evidence supports each inheritance determination?
- Which controls are shared between the provider, agency, and system team?
- Which controls require implementation or operation by the application team?
- Are additional controls necessary based on system-specific risks, architecture, or mission requirements?
- What assessment procedures and evidence will be required to evaluate each selected control?

No control should be marked implemented, inherited, effective, or compliant without appropriate supporting evidence.

## 6. Next Assessment Activities

The next activities are to:

1. Validate the system categorization and determine the applicable starting baseline using NIST SP 800-53B.
2. Document selected controls, enhancements, tailoring decisions, implementation responsibilities, and evidence requirements.
3. Align the control assessment matrix with the validated control selection.
4. Develop and tailor assessment procedures using NIST SP 800-53A Revision 5, Release 5.2.0.
5. Record simulated assessment results and document potential findings with clear evidence references and limitations.
6. Develop and track proposed corrective actions through the POA&M.

Because FCMS-001 is a portfolio simulation, these activities demonstrate an assessment workflow rather than an actual federal authorization or compliance determination.

## 7. References

- [NIST SP 800-53 Revision 5, Release 5.2.0 — Security and Privacy Controls for Information Systems and Organizations](https://csrc.nist.gov/pubs/sp/800/53/r5/upd1/final)
- [NIST SP 800-53B, Release 5.2.0 — Control Baselines for Information Systems and Organizations](https://csrc.nist.gov/pubs/sp/800/53/b/upd1/final)
- [NIST SP 800-53A Revision 5, Release 5.2.0 — Assessing Security and Privacy Controls in Information Systems and Organizations](https://csrc.nist.gov/pubs/sp/800/53/a/r5/final)
- [NIST FIPS 199 — Standards for Security Categorization of Federal Information and Information Systems](https://csrc.nist.gov/pubs/fips/199/final)

## 8. Simulation Disclaimer

This document is an educational simulation based on a fictional system. It is not an approved federal security plan, a formally completed control selection, a verified control inheritance determination, or evidence of actual compliance with NIST requirements.
