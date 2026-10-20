# FCMS-001 — Decision Log

**Document status:** Working draft  
**Version:** 1.2  
**System ID:** FCMS-001

## Purpose

This log records significant project decisions, their rationale, and assumptions that require validation as the simulated Federal Benefits Case Management System assessment progresses.

## Decisions

| ID | Decision | Rationale | Status |
|---|---|---|---|
| D-001 | Use a fictional federal benefits case management system as the assessment subject. | Provides a consistent scenario for demonstrating RMF and security assessment methods without representing an actual federal system. | Established |
| D-002 | Use AWS as the proposed hosting environment. | Creates a cloud security scenario involving provider dependencies and shared-responsibility considerations. | Established as a scenario assumption |
| D-003 | Include applicant PII, benefit application information, supporting documents, and eligibility decisions as information types. | Supports meaningful analysis of confidentiality, integrity, privacy, and mission availability. | Provisional; exact data elements remain undefined |
| D-004 | Exclude classified information, payment-card data, and direct storage of bank account details from the initial scenario. | Keeps the project focused on a manageable benefits-processing system without introducing unrelated requirements. | Established for the current simulation |
| D-005 | Use Moderate as the preliminary impact hypothesis for confidentiality and integrity, and Low for availability. | Reflects the current scenario assumptions documented in `docs/security-categorization.md`. Confidentiality and integrity are assumed to have the potential for serious adverse effects, while a temporary availability disruption is assumed to cause processing delays and a manageable backlog. | Provisional; requires validation |
| D-011 | Model FCMS-001 as a routine administrative benefits-processing service rather than a mission-critical service. | Establishes a realistic operational context in which outages cause processing delays and backlogs. The actual availability impact remains subject to validation of potential consequences, including prolonged outages and time-sensitive benefits. | Established for the simulation |
| D-006 | Define a provisional authorization boundary around the application, database, document storage, and system-specific security components. | Establishes an initial assessment scope while recognizing external dependencies and shared responsibilities. | Provisional; requires refinement |
| D-007 | Treat underlying AWS infrastructure and separately managed agency services as external dependencies. | Avoids assuming the system owner implements every supporting control. Responsibility and inheritance must be validated. | Provisional |
| D-008 | Treat intended security capabilities as design requirements rather than verified controls. | Prevents claims about implementation or effectiveness without supporting assessment evidence. | Established |
| D-009 | Label all scenario evidence and assessment results as simulated or synthetic. | Maintains transparency about the educational nature of the portfolio. | Established |
| D-010 | Prioritize a focused assessment of system scope, security categorization, control selection, evidence-based testing, and remediation. | Concentrates effort on transferable skills relevant to entry-level GRC, security assurance, and IT risk roles. | Established |

## Change History

| Version | Change |
|---|---|
| 1.0 | Initial decision log created during system definition and scope. |
| 1.1 | Refined the system mission to federal benefits processing and documented the associated information types and scope assumptions. |
| 1.2 | Aligned D-005 and the review notes with the preliminary confidentiality Moderate, integrity Moderate, and availability Low categorization hypothesis. |

## Review Notes

Decisions marked provisional may change when additional information becomes available.

Changes to the system mission, information types, authorization boundary, or impact categorization must be reflected in the relevant project documents.

The preliminary impact hypothesis is Moderate for confidentiality and integrity and Low for availability. It is not a final FIPS 199 determination. Each security objective requires a documented impact rationale before the system categorization is finalized.
