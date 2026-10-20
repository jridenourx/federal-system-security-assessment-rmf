# Federal System Security Assessment & RMF Package

**Project ID:** FCMS-001  
**Project Type:** Fictional federal security assessment simulation  
**Frameworks:** NIST Risk Management Framework (RMF), FIPS 199, NIST SP 800-53, and NIST SP 800-53A

## Project Overview

This portfolio project demonstrates a structured security assessment of a fictional AWS-hosted Federal Benefits Case Management System (FCMS-001).

The scenario follows a simplified federal security assessment workflow: define the system and its boundaries, develop a preliminary security categorization, identify relevant security controls, examine synthetic evidence, document potential findings, and propose remediation actions.

The project emphasizes evidence traceability, risk-based reasoning, documentation quality, and the distinction between assumptions and supported conclusions.

**Important:** This is an educational simulation. No actual federal system, AWS environment, or production security evidence has been assessed.

## Scenario

FCMS-001 is a fictional federal application used to receive, review, process, and track administrative benefit applications.

The scenario includes applicant information, application details, supporting documents, eligibility decisions, case status, and case history.

The proposed architecture includes an application, relational database, object storage, identity and access services, encryption, and logging. Specific AWS services and detailed implementation configurations remain subject to further definition.

The initial security categorization is a preliminary hypothesis and has not been approved by a system owner.

## Project Objectives

- Define system scope, boundaries, information types, and external dependencies.
- Develop a preliminary FIPS 199 security categorization with documented assumptions.
- Identify relevant NIST security control areas and shared-responsibility considerations.
- Define assessment procedures and evidence requirements.
- Review synthetic evidence and document potential control deficiencies.
- Connect findings to proposed corrective actions and closure criteria.
- Maintain traceability between system assumptions, evidence, findings, and remediation planning.

## Repository Guide

### System Definition and Planning

| Artifact | Description |
|---|---|
| `docs/system-profile-and-scope.md` | System purpose, scope, information types, and boundaries |
| `docs/decision-log.md` | Key scenario decisions and assumptions |
| `docs/diagrams/system-boundary-and-data-flow.md` | System boundary and data-flow diagram |
| `docs/security-categorization.md` | Preliminary FIPS 199 security categorization |
| `docs/security-control-selection.md` | Proposed security control selection approach |
| `docs/control-assessment-matrix.md` | Selected controls, assessment objectives, procedures, and evidence needs |

### Evidence and Assessment

| Artifact | Description |
|---|---|
| `docs/evidence-register.md` | Evidence inventory and evidence-handling requirements |
| `evidence/ev-001-account-management.md` | Synthetic account management evidence |
| `evidence/ev-004-event-logging.md` | Synthetic event logging evidence |
| `docs/workpapers/wp-001-account-management.md` | Account management assessment workpaper |

### Findings and Remediation

| Artifact | Description |
|---|---|
| `docs/findings-register.md` | Preliminary findings, risks, recommendations, and closure criteria |
| `docs/poam.md` | Proposed remediation actions and milestones |

## Current Assessment Highlights

### Account Management — AC-2

The synthetic account deactivation procedure assigns responsibility for disabling accounts but does not define a maximum deactivation timeframe. The scenario also lacks completed deactivation records.

The project documents this as a potential control deficiency requiring validation. It does not claim that unauthorized accounts exist or that a real control failed.

### Event Logging — AU-2

The synthetic event list does not establish whether administrative configuration changes or changes to logging settings must be captured.

The project identifies this as an issue requiring validation against applicable requirements and technical evidence. No actual logging configuration has been examined.

## Methodology

The project uses a simplified, evidence-focused assessment workflow:

1. Define the system and record assumptions.
2. Develop a preliminary security categorization.
3. Identify relevant control areas and assessment objectives.
4. Identify and review synthetic evidence.
5. Document observations, limitations, and potential findings.
6. Propose corrective actions and closure criteria.
7. Maintain traceability across evidence, findings, and remediation.

The approach is informed by NIST publications. It is not a complete implementation of the federal RMF process and does not establish compliance or authorization readiness.

## Limitations

- The system and organization are fictional.
- Evidence is synthetic and created for educational purposes.
- No real cloud configuration, security logs, user accounts, or production records were accessed.
- Control selection and categorization remain preliminary.
- Finding severity and remediation dates are not approved.
- The assessment is not a substitute for an authorized security assessment or formal authorization process.

## References

- [NIST Risk Management Framework](https://csrc.nist.gov/projects/risk-management)
- [FIPS 199 — Standards for Security Categorization of Federal Information and Information Systems](https://csrc.nist.gov/pubs/fips/199/final)
- [NIST SP 800-53 Rev. 5 — Security and Privacy Controls](https://csrc.nist.gov/pubs/sp/800/53/r5/upd1/final)
- [NIST SP 800-53A Rev. 5 — Assessing Security and Privacy Controls](https://csrc.nist.gov/pubs/sp/800/53/a/r5/final)

## Disclaimer

This repository is a fictional portfolio simulation created to demonstrate learning and assessment methodology. It does not represent work performed for a federal agency, an approved system security plan, an actual control assessment, or a formal security authorization.
