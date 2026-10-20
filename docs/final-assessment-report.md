# Final Security Assessment Report — FCMS-001

**Document Status:** Draft — Simulation  
**System ID:** FCMS-001  
**System Name:** Federal Benefits Case Management System  
**Assessment Type:** Tabletop security control assessment using synthetic evidence  
**Assessment Framework:** NIST RMF concepts, FIPS 199, NIST SP 800-53 Revision 5, Release 5.2.0, NIST SP 800-53A Revision 5, Release 5.2.0  
**Report Date:** October 20, 2026  
**Overall Assessment Status:** Preliminary — validation required

## 1. Executive Summary

This report documents a simulated security assessment of FCMS-001, a fictional AWS-hosted federal benefits case management application. The exercise demonstrates a structured approach to defining system scope, proposing a security categorization, identifying relevant security controls, reviewing synthetic evidence, documenting potential control deficiencies, and proposing remediation actions.

The assessment developed two preliminary findings:

- **FCMS-F-001 — Account Management:** The synthetic account deactivation procedure does not specify a maximum timeframe for removing access when it is no longer required.
- **FCMS-F-002 — Event Logging:** The synthetic documentation does not establish whether administrative configuration changes and changes to logging settings or destinations must be captured.

The first finding has a provisional Moderate severity rating. The second remains unrated because the available evidence does not establish whether the identified omissions represent a confirmed control deficiency.

These findings are based entirely on synthetic evidence. No real federal system, AWS environment, production configuration, or security log was examined. Accordingly, the results are illustrative and do not establish compliance or noncompliance with any federal security requirement.

## 2. System Overview

FCMS-001 is a fictional federal application used to receive, review, process, and track administrative benefit applications.

### 2.1 Information Processed

The scenario includes:

- Applicant personally identifiable information (PII).
- Benefit application details and supporting documents.
- Eligibility decisions, case status, and case history.
- User and access records.
- System configuration and operational metadata.

The scenario excludes classified information, payment card data, and direct storage of bank account details. Specific benefit programs, information volumes, privacy requirements, and recovery objectives have not been established.

### 2.2 Proposed Architecture and Scope

The proposed architecture includes an application, relational database, object storage, identity and access services, encryption and key management, and logging and monitoring capabilities.

The proposed authorization boundary includes system-specific application components, data stores, access configurations, security settings, logging, and deployment artifacts. Underlying cloud infrastructure, agency identity services, user workstations, and external agency systems are treated as external dependencies pending further validation.

The exact AWS services, service configurations, and shared-responsibility assignments remain to be confirmed.

## 3. Assessment Objectives and Scope

The exercise aimed to:

1. Define the fictional system's purpose, scope, information types, and dependencies.
2. Develop a preliminary security categorization using FIPS 199 concepts.
3. Identify relevant security control areas using NIST SP 800-53 Revision 5, Release 5.2.0.
4. Define evidence requirements and assessment procedures informed by NIST SP 800-53A Revision 5, Release 5.2.0.
5. Review synthetic evidence and document potential control deficiencies.
6. Propose corrective actions, milestones, and closure criteria.

The assessment was limited to a focused sample of account management and event logging. It was not a complete assessment of all controls in a Moderate baseline.

## 4. Methodology

The exercise followed a simplified, evidence-focused workflow:

1. Establish system assumptions and document the proposed boundary.
2. Develop a preliminary FIPS 199 security categorization.
3. Identify relevant control families and shared-responsibility considerations.
4. Define assessment objectives, procedures, and evidence requirements.
5. Review synthetic evidence and record observations and limitations.
6. Document potential findings and proposed remediation actions.
7. Define evidence-based closure criteria.

The assessment approach distinguishes between an undocumented requirement, insufficient evidence, and a confirmed technical control failure. Conclusions are limited to what the synthetic scenario supports.

## 5. Preliminary Security Categorization

The proposed security category is:

**SC FCMS-001 = {(Confidentiality, MODERATE), (Integrity, MODERATE), (Availability, LOW)}**

The preliminary overall impact level is Moderate under the high-water-mark approach.

### 5.1 Rationale

- **Confidentiality — Moderate:** Unauthorized disclosure of applicant information and supporting documents could cause meaningful privacy harm and serious agency consequences.
- **Integrity — Moderate:** Unauthorized modification of applications, eligibility decisions, or case status could result in incorrect administrative outcomes and undermine trust.
- **Availability — Low:** Based on the current scenario assumptions, temporary outages would primarily delay routine administrative processing and create a backlog.

The availability rating depends on unvalidated assumptions about downtime tolerance, benefit deadlines, and the consequences of prolonged outages.

**Categorization status:** Preliminary and unapproved. The system owner and appropriate agency officials would need to validate the information types, mission consequences, applicable requirements, and final ratings.

## 6. Assessment Results

### 6.1 Finding FCMS-F-001 — Account Deactivation Timeframe Is Not Defined

**Control:** AC-2 — Account Management  
**Evidence:** EV-001  
**Preliminary severity:** Moderate — provisional  
**Status:** Open; validation required  
**Related POA&M:** FCMS-POAM-001

**Condition**

The synthetic account deactivation procedure assigns responsibility for disabling accounts but does not define a maximum timeframe for removing access when an employee leaves the program or no longer requires access. The scenario also lacks completed deactivation records demonstrating how the process operates.

**Potential risk**

If access is not removed promptly, unnecessary access to applicant records or administrative functions could persist. This could increase the opportunity for unauthorized access or changes to case information.

**Recommendation**

Define and approve a risk-based account deactivation timeframe. Document escalation and exception procedures, and retain records showing when requests are received and access is disabled.

**Additional validation**

- Confirm applicable account management requirements and organizational policy.
- Obtain completed account removal requests and corresponding timestamps.
- Determine whether a timeframe is documented elsewhere.
- Evaluate the evidence against confirmed assessment criteria.
- Reassess severity using documented risk-rating criteria.

**Closure approach**

Require an approved procedure, evidence of implementation, and a review of sample account removal events against the approved timeframe. A written procedure alone may not demonstrate effective operation.

### 6.2 Finding FCMS-F-002 — Logging Event Selection Requires Validation

**Control:** AU-2 — Event Logging  
**Evidence:** EV-004  
**Preliminary severity:** Undetermined  
**Status:** Open; validation required  
**Related POA&M:** FCMS-POAM-002

**Condition**

The synthetic draft event list does not include administrative configuration changes or changes to logging settings and destinations. The available documentation does not establish whether these events are required, intentionally excluded, or captured through other mechanisms.

**Potential risk**

If required administrative or logging-configuration changes are not recorded, investigators may have difficulty determining who changed security settings, what changed, and when the change occurred.

**Recommendation**

Validate applicable logging requirements and document the event-selection rationale. If a deficiency is confirmed, update the logging requirements and configurations as necessary, then verify that required events are generated and delivered to the intended destination.

**Additional validation**

- Obtain the approved logging policy and event-selection rationale.
- Determine whether the missing event categories are required.
- Review relevant configuration settings and sample event records.
- Confirm whether other logging mechanisms capture the events.
- Assign severity only after the condition and associated risk are sufficiently established.

**Closure approach**

Document the applicable requirements, confirm whether the identified events must be captured, correct any confirmed deficiencies, and retain evidence supporting the closure decision. If the existing configuration already satisfies the requirements, document the rationale and reassess whether the finding remains warranted.

## 7. Remediation Plan

The proposed remediation actions are tracked in `docs/poam.md`.

| POA&M ID | Finding | Planned focus | Status |
|---|---|---|---|
| FCMS-POAM-001 | FCMS-F-001 | Establish and validate account deactivation requirements and operation | Open — proposed |
| FCMS-POAM-002 | FCMS-F-002 | Validate event-selection requirements and correct any confirmed logging gaps | Open — proposed |

No remediation owners, milestone dates, or completion claims have been established because the system is fictional.

## 8. Assessment Limitations

The following limitations apply:

- FCMS-001 and its organization are fictional.
- All evidence created for the exercise is synthetic.
- No actual AWS account, federal system, user account, production configuration, or security log was accessed.
- The security categorization is preliminary and unapproved.
- Control selection is not a complete, formally tailored Moderate baseline.
- The assessment covers only a small sample of control areas.
- The potential findings have not been validated against a real system or approved organizational requirements.
- Severity and remediation dates have not been formally approved.
- No control has been demonstrated to be compliant or effective in a real operating environment.

## 9. Recommended Next Actions

For a real assessment, the following actions would be appropriate:

1. Validate the system boundary, information types, mission impact, and security categorization with the system owner.
2. Confirm the applicable security control baseline and document tailoring decisions.
3. Establish control ownership and identify inherited, shared, and system-specific responsibilities.
4. Obtain approved organizational policies and relevant technical evidence.
5. Execute defined assessment procedures and record evidence-supported results.
6. Validate findings, determine risk ratings, and assign remediation owners and dates.
7. Track corrective actions through implementation, verification, and formal closure review.

## 10. Conclusion

This portfolio exercise demonstrates a structured approach to preliminary security assessment documentation, evidence traceability, potential finding development, and remediation planning.

The most important outcome is the traceability between the fictional system assumptions, selected controls, synthetic evidence, findings, and proposed corrective actions. The exercise also demonstrates the importance of stating limitations and avoiding conclusions that exceed the available evidence.

The project is an educational simulation, not a completed federal security assessment, compliance determination, or authorization decision.

## 11. References

- [NIST Risk Management Framework](https://csrc.nist.gov/projects/risk-management)
- [NIST FIPS 199 — Standards for Security Categorization of Federal Information and Information Systems](https://csrc.nist.gov/pubs/fips/199/final)
- [NIST SP 800-53 Revision 5, Release 5.2.0 — Security and Privacy Controls for Information Systems and Organizations](https://csrc.nist.gov/pubs/sp/800/53/r5/upd1/final)
- [NIST SP 800-53A Revision 5, Release 5.2.0 — Assessing Security and Privacy Controls in Information Systems and Organizations](https://csrc.nist.gov/pubs/sp/800/53/a/r5/final)
- [NIST SP 800-53B, Release 5.2.0 — Control Baselines for Information Systems and Organizations](https://csrc.nist.gov/pubs/sp/800/53/b/upd1/final)

## 12. Simulation Disclaimer

FCMS-001, all evidence, findings, ratings, and remediation plans in this report are fictional. This report is a portfolio learning artifact and does not represent work performed for a federal agency, an approved system security plan, an actual control assessment, or a formal security authorization.
