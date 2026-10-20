# Plan of Action and Milestones (POA&M) — FCMS-001

**Document Status:** Draft — Simulation  
**System ID:** FCMS-001  
**Assessment Reference:** FCMS-F-001, FCMS-F-002  
**POA&M Status:** Proposed remediation plan  
**Classification:** Fictional educational portfolio artifact

## 1. Purpose

This document tracks proposed corrective actions for potential security control deficiencies identified during the fictional FCMS-001 security assessment.

A Plan of Action and Milestones (POA&M) documents identified weaknesses, planned corrective actions, responsible parties, milestones, and progress toward resolution.

This document represents a proposed remediation plan for a simulated system. It is not an approved agency POA&M, and no remediation activities have been performed against a real system.

## 2. POA&M Summary

| POA&M ID | Finding ID | Control | Weakness | Preliminary severity | Status |
|---|---|---|---|---|---|
| FCMS-POAM-001 | FCMS-F-001 | AC-2 — Account Management | Account deactivation timeframe is not defined | Moderate — provisional | Open — proposed |
| FCMS-POAM-002 | FCMS-F-002 | AU-2 — Event Logging | Logging event selection requires validation | Undetermined | Open — proposed |

Severity assignments remain subject to validation. FCMS-POAM-001 has a provisional scenario rating. FCMS-POAM-002 remains unrated until the applicable logging requirements and potential deficiency are established.

## 3. FCMS-POAM-001 — Account Management

**Related finding:** FCMS-F-001  
**Control:** AC-2 — Account Management  
**Evidence reference:** EV-001  
**Status:** Open — proposed  
**Preliminary severity:** Moderate — provisional

### 3.1 Weakness

The fictional account deactivation procedure assigns responsibility for disabling accounts but does not specify a maximum timeframe for removing access when an employee leaves the program or no longer requires access.

The scenario also lacks completed deactivation records demonstrating how the process operates.

### 3.2 Risk Statement

If access is not removed promptly when personnel no longer require it, unnecessary access to applicant records or administrative functions could persist. This could increase the opportunity for unauthorized access or changes to benefits case information.

The actual likelihood and impact remain undetermined because no real account activity or completed deactivation records have been examined.

### 3.3 Corrective Action

Define and approve a risk-based account deactivation timeframe. Document escalation and exception procedures, and retain records showing when access-removal requests are received, when accounts are disabled, and whether applicable timeframes are met.

### 3.4 Milestones

| Milestone | Planned activity | Expected evidence | Responsible role | Status |
|---|---|---|---|---|
| M1 | Review applicable account management requirements and existing procedures | Requirements review and documented gap analysis | System owner / security lead | Proposed |
| M2 | Define and approve the deactivation timeframe and exception process | Approved account management procedure | System owner / identity and access administrator | Proposed |
| M3 | Implement the approved process and establish recordkeeping | Updated procedure, workflow documentation, and sample deactivation records | Identity and access administrator | Proposed |
| M4 | Evaluate a sample of account removal events against the approved requirements | Assessment workpaper with evidence references and results | Security assessor / control owner | Proposed |
| M5 | Review results and determine whether the finding can be closed | Closure review and documented approval | Authorized reviewer | Proposed |

### 3.5 Closure Criteria

The finding may be considered for closure when:

- The deactivation timeframe and exception process are approved and documented.
- The responsible team demonstrates that the process has been implemented.
- A sample of account removal events is evaluated against the approved timeframe.
- Any identified exceptions or failures are assessed and addressed.
- The designated reviewer determines that the corrective action adequately addresses the finding.

A documented procedure alone may not be sufficient to demonstrate effective operation.

## 4. FCMS-POAM-002 — Event Logging

**Related finding:** FCMS-F-002  
**Control:** AU-2 — Event Logging  
**Evidence reference:** EV-004  
**Status:** Open — proposed  
**Preliminary severity:** Undetermined

### 4.1 Weakness

The fictional system's draft event list does not establish whether administrative configuration changes and changes to logging settings or destinations must be recorded.

The available documentation does not establish whether these events are required, intentionally excluded, or captured through other mechanisms.

### 4.2 Risk Statement

If required administrative or logging-configuration changes are not recorded, investigators may have difficulty determining who changed security settings, what changed, and when the change occurred.

The actual likelihood and impact cannot be determined from the synthetic evidence. The existence of a confirmed technical logging deficiency has not been established.

### 4.3 Corrective Action

Validate the applicable logging requirements and document the event-selection rationale. Determine whether administrative and logging-configuration events must be captured.

If a control gap is confirmed, update the logging requirements and configurations as necessary, then verify that required events are generated and delivered to the intended logging destination.

If the existing configuration already satisfies the applicable requirements, document the rationale and reassess whether the finding remains warranted.

### 4.4 Milestones

| Milestone | Planned activity | Expected evidence | Responsible role | Status |
|---|---|---|---|---|
| M1 | Review logging policy and applicable event-selection requirements | Requirements review and gap analysis | System owner / security lead | Proposed |
| M2 | Determine whether the identified event categories must be captured | Documented assessment decision and approved event-selection rationale | System owner / security lead | Proposed |
| M3 | If required, implement approved logging changes | Configuration records and change documentation | Cloud / application administrator | Conditional |
| M4 | Evaluate sample events and confirm expected logging behavior | Assessment workpaper, configuration evidence, and sample event records | Security assessor / control owner | Proposed |
| M5 | Review results and determine closure eligibility | Closure review and documented approval | Authorized reviewer | Proposed |

### 4.5 Closure Criteria

The finding may be considered for closure when:

- Applicable logging requirements and the event-selection rationale are documented.
- The assessment determines whether the identified event categories are required.
- Any confirmed deficiencies are corrected.
- Appropriate configuration records and sample events demonstrate that required events are generated and captured.
- The designated reviewer determines that the evidence supports closure.

If the assessment determines that the existing configuration satisfies the applicable requirements, the decision must be documented and the finding formally reassessed.

## 5. Schedule and Tracking

No milestone dates or completion claims have been assigned because FCMS-001 is a simulated system without an actual system owner or remediation team.

In a real engagement, responsible owners would assign milestone dates based on risk, applicable requirements, available resources, and the organization's approved remediation process.

| Tracking field | FCMS-POAM-001 | FCMS-POAM-002 |
|---|---|---|
| Remediation owner | To be assigned | To be assigned |
| Planned completion date | To be assigned | To be assigned |
| Actual completion date | Not applicable — simulation | Not applicable — simulation |
| Risk acceptance | Not determined | Not determined |
| Closure status | Open — proposed | Open — proposed |
| Last status update | Initial draft | Initial draft |

## 6. Relationship to Assessment Evidence

The remediation entries trace back to the following artifacts:

| Artifact | Purpose |
|---|---|
| EV-001 | Synthetic account inventory and account lifecycle procedure |
| FCMS-F-001 | Preliminary account management finding |
| FCMS-POAM-001 | Proposed account management corrective action |
| EV-004 | Synthetic event list and logging configuration summary |
| FCMS-F-002 | Preliminary event logging finding |
| FCMS-POAM-002 | Proposed logging validation and corrective action |

This traceability links evidence, potential weaknesses, corrective actions, and closure criteria. It does not establish that either control has been found ineffective in a real environment.

## 7. References

- NIST SP 800-53 Revision 5 — Security and Privacy Controls for Information Systems and Organizations: https://csrc.nist.gov/pubs/sp/800/53/r5/upd1/final
- NIST SP 800-53A Revision 5 — Assessing Security and Privacy Controls in Information Systems and Organizations: https://csrc.nist.gov/pubs/sp/800/53/a/r5/final

## 8. Simulation Disclaimer

FCMS-001, FCMS-F-001, FCMS-F-002, FCMS-POAM-001, FCMS-POAM-002, and all associated evidence are fictional.

This document is an educational portfolio artifact. It does not represent an actual federal agency finding, approved remediation deadline, completed corrective action, or formal authorization decision.
