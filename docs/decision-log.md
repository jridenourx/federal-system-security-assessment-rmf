# FCMS-001 — Decision Log

**Document status:** Working draft  
**Version:** 1.0  
**System ID:** FCMS-001

## Purpose

This log records significant project decisions, their rationale, and assumptions that require validation as the simulated Federal Case Management System assessment progresses.

| ID | Decision | Rationale | Status |
|---|---|---|---|
| D-001 | Use a fictional federal case management system as the assessment subject. | Provides a consistent scenario for demonstrating RMF and security assessment methods without representing an actual federal system. | Established |
| D-002 | Use AWS as the proposed hosting environment. | Creates a relevant cloud security scenario with external dependencies and shared-responsibility considerations. | Established as a scenario assumption |
| D-003 | Treat case-related PII as a primary information type. | Makes confidentiality and privacy considerations relevant to system scoping and security categorization. | Provisional; exact data elements remain undefined |
| D-004 | Use moderate impact as the initial FIPS 199 hypothesis for confidentiality, integrity, and availability. | Provides a starting hypothesis for analysis without predetermining the final categorization. | Pending impact analysis |
| D-005 | Define a provisional authorization boundary around the application, database, document storage, and system-specific security components. | Establishes an initial assessment scope while recognizing external dependencies and shared responsibilities. | Provisional; requires refinement |
| D-006 | Treat underlying AWS infrastructure and separately managed agency services as external dependencies. | Avoids assuming the system owner directly implements every supporting control. Responsibility and inheritance must be validated. | Provisional |
| D-007 | Treat intended security capabilities as design requirements rather than verified controls. | Prevents the project from claiming implementation or effectiveness without supporting assessment evidence. | Established |
| D-008 | Label all scenario evidence and assessment results as simulated or synthetic. | Maintains transparency about the educational nature of the portfolio. | Established |

## Change History

| Version | Change |
|---|---|
| 1.0 | Initial decision log created during Phase 1 system definition and scope. |

## Review Notes

Decisions marked provisional may change when additional information becomes available. Changes to the system boundary, information types, or impact categorization must be reflected in the relevant project documents.
