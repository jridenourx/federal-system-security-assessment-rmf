# FCMS-001 — Security Categorization Worksheet

**Document status:** Draft  
**Version:** 1.0  
**System ID:** FCMS-001  
**Methodology:** FIPS 199  
**Assessment type:** Portfolio simulation

## 1. Purpose

This worksheet evaluates the potential impact of unauthorized disclosure, modification, or disruption of information processed by the Federal Benefits Case Management System (FCMS-001).

The proposed impact ratings are based on the fictional system's defined mission, information types, and expected operational consequences. They are preliminary and require further review before being treated as final.

## 2. System and Information Summary

FCMS-001 is a fictional AWS-hosted federal application used to process administrative benefit applications.

The system stores applicant personally identifiable information (PII), application details, supporting documents, eligibility decisions, and case history.

The system supports routine administrative benefits processing. A service outage is expected to delay application processing and create a backlog, rather than immediately interrupt an essential service.

The scenario excludes classified information, payment-card data, and direct storage of bank account details.

## 3. FIPS 199 Impact Definitions

| Impact level | Definition |
|---|---|
| Low | The compromise could cause a limited adverse effect on organizational operations, assets, or individuals. |
| Moderate | The compromise could cause a serious adverse effect on organizational operations, assets, or individuals. |
| High | The compromise could cause a severe or catastrophic adverse effect on organizational operations, assets, or individuals. |

## 4. Preliminary Impact Analysis

| Security objective | Proposed impact | Scenario-specific rationale |
|---|---|---|
| Confidentiality | Moderate | Unauthorized disclosure of applicant information and supporting documents could cause meaningful privacy harm to affected individuals and create serious consequences for agency operations. |
| Integrity | Moderate | Unauthorized changes to applications or eligibility decisions could result in incorrect outcomes, require case reviews and corrections, and undermine confidence in the agency's processing records. |
| Availability | Low | Under the current scenario assumptions, an outage primarily delays routine application processing and creates a manageable backlog. The impact could increase if outages become prolonged or affect time-sensitive benefits. |

## 5. Overall Proposed Security Category

Under the FIPS 199 high-water-mark approach, the system's overall security category uses the highest applicable impact level among confidentiality, integrity, and availability.

**Proposed categorization:**

SC FCMS-001 = {(Confidentiality, MODERATE), (Integrity, MODERATE), (Availability, LOW)}

**Overall impact level: MODERATE**

This is a preliminary portfolio determination based on the stated scenario assumptions. It is not an approved government categorization.

## 6. Assumptions and Limitations

- Applicant information is assumed to create a serious potential privacy impact if disclosed without authorization.
- Unauthorized modification of eligibility decisions is assumed to create serious consequences requiring investigation and correction.
- The system is assumed to support routine administrative processing, with a manageable backlog during a temporary outage.
- The scenario does not yet define the volume of applications, maximum tolerable downtime, recovery time objectives, or the consequences of delayed individual applications.
- The exact applicant data elements and applicable privacy requirements have not been validated against an actual agency mission.
- No real system data, assessment evidence, or agency approval has been used.

If subsequent analysis demonstrates more severe consequences, the relevant impact rating must be revised.

## 7. Review Questions

1. Could disclosure of the defined applicant information cause serious harm to individuals?
2. Could unauthorized changes to eligibility decisions materially affect applicants or agency operations?
3. How long could the system be unavailable before the resulting backlog causes serious adverse effects?
4. Are any benefit types, deadlines, or applicant circumstances that could materially increase the impact excluded from the current scenario?

## 8. Reference

National Institute of Standards and Technology (NIST), FIPS Publication 199, *Standards for Security Categorization of Federal Information and Information Systems*.

Official publication: https://csrc.nist.gov/pubs/fips/199/final
