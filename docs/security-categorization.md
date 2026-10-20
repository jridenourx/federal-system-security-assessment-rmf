# FCMS-001 — Security Categorization Worksheet

**Document status:** Draft — Simulation  
**Version:** 1.1  
**System ID:** FCMS-001  
**Methodology:** FIPS 199, informed by NIST SP 800-60  
**Assessment type:** Portfolio simulation

## 1. Purpose

This worksheet documents a preliminary security categorization for the fictional Federal Benefits Case Management System (FCMS-001).

The analysis considers the potential adverse effects on individuals, organizational operations, and assets resulting from unauthorized disclosure, modification, or disruption of the information and system.

The proposed impact ratings are based on the fictional system's information types, operational purpose, and expected consequences. They are preliminary assumptions for this portfolio exercise and require validation before being treated as final.

NIST SP 800-60 provides guidance for mapping information types to security categories and recommended impact levels. For a real federal system, the categorization would also need to reflect the agency's mission, applicable requirements, and documented risk judgments.

## 2. System and Information Summary

FCMS-001 is a fictional AWS-hosted federal application used to process administrative benefit applications.

The system stores:

- Applicant personally identifiable information (PII)
- Application details and responses
- Supporting documents
- Eligibility decisions and their rationale
- Application status, effective dates, and case history
- User and access records, logs, configuration information, and operational metadata

The system supports routine administrative benefits processing. Under the current scenario assumptions, a temporary service outage would delay application processing and create a manageable backlog rather than immediately interrupt an essential service.

The scenario excludes classified information, payment-card data, and direct storage of bank account details. The exact applicant data elements, benefit programs, and applicable privacy requirements have not been validated against an actual agency mission.

## 3. FIPS 199 Impact Definitions

| Impact level | Definition |
|---|---|
| Low | A compromise could be expected to cause a limited adverse effect on organizational operations, organizational assets, or individuals. |
| Moderate | A compromise could be expected to cause a serious adverse effect on organizational operations, organizational assets, or individuals. |
| High | A compromise could be expected to cause a severe or catastrophic adverse effect on organizational operations, organizational assets, or individuals. |

Impact is evaluated separately for confidentiality, integrity, and availability. The ratings reflect the potential consequences of a compromise, not merely the sensitivity of the data or the presence of a particular technology.

## 4. Preliminary Impact Analysis

| Security objective | Proposed impact | Scenario-specific rationale |
|---|---|---|
| Confidentiality | Moderate | Unauthorized disclosure of applicant information and supporting documents could cause meaningful privacy harm to affected individuals and create serious consequences for agency operations. This rating assumes the information and circumstances could result in serious adverse effects; it requires validation against the actual information types and applicable agency requirements. |
| Integrity | Moderate | Unauthorized changes to applications or eligibility decisions could result in incorrect outcomes, require case reviews and corrections, and undermine confidence in agency processing records. The proposed rating assumes these consequences could be serious. |
| Availability | Low | Under the current scenario assumptions, a temporary outage primarily delays routine application processing and creates a manageable backlog. The impact could be higher if outages were prolonged, affected time-sensitive benefits, or prevented applicants from meeting important deadlines. |

These are scenario-based impact hypotheses, not ratings established solely by the fact that FCMS-001 processes PII.

## 5. Overall Proposed Security Category

Under FIPS 199, the system's overall security category uses the high-water-mark approach: the highest applicable impact level among confidentiality, integrity, and availability determines the overall impact level.

**Proposed security category:**

SC FCMS-001 = {(Confidentiality, MODERATE), (Integrity, MODERATE), (Availability, LOW)}

**Overall proposed impact level: MODERATE**

This is a preliminary portfolio determination based on the assumptions documented in this worksheet. It has not been approved by a system owner, authorizing official, or federal agency.

The proposed category should be reassessed if validation of the information types, mission consequences, or operational requirements changes any individual impact rating.

## 6. Assumptions and Limitations

- Applicant information is assumed to create a serious potential privacy impact if disclosed without authorization.
- Unauthorized modification of eligibility decisions is assumed to create serious consequences requiring investigation and correction.
- The system is assumed to support routine administrative processing, with a manageable backlog during a temporary outage.
- The scenario does not define application volumes, maximum tolerable downtime, recovery time objectives, or the consequences of delayed individual applications.
- The exact information types and data elements have not been mapped to the applicable NIST SP 800-60 guidance.
- Applicable agency privacy requirements, mission priorities, and organizational risk criteria have not been validated.
- No real system data, assessment evidence, or agency approval has been used.

If subsequent analysis demonstrates more severe consequences, the relevant impact rating and overall proposed category must be reassessed.

## 7. Review Questions

1. Which information types best describe the applicant information and benefits-processing records handled by FCMS-001 under NIST SP 800-60?
2. Could disclosure of the defined applicant information cause serious harm to individuals or serious adverse effects on agency operations?
3. Could unauthorized changes to eligibility decisions materially affect applicants or agency operations?
4. How long could the system be unavailable before the resulting backlog causes serious adverse effects?
5. Are there benefit types, deadlines, or applicant circumstances that could materially increase the impact?
6. Do agency requirements or documented risk criteria support the proposed impact levels?

## 8. References

- National Institute of Standards and Technology (NIST), FIPS Publication 199, *Standards for Security Categorization of Federal Information and Information Systems*: https://csrc.nist.gov/pubs/fips/199/final
- NIST SP 800-60 Volume I, Revision 1, *Guide for Mapping Types of Information and Information Systems to Security Categories*: https://csrc.nist.gov/pubs/sp/800/60/v1/r1/final
- NIST SP 800-60 Volume II, Revision 1, *Guide for Mapping Types of Information and Information Systems to Security Categories: Appendices*: https://csrc.nist.gov/pubs/sp/800/60/v2/r1/final

## 9. Simulation Disclaimer

This worksheet is an educational simulation based on a fictional system. It is not an approved federal security categorization, a completed risk assessment, or evidence of actual compliance with NIST requirements.
