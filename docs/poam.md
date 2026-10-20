# Plan of Action and Milestones (POA&M) — FCMS-001

**Document Status:** Draft — Simulation  
**System ID:** FCMS-001  
**Assessment Reference:** FCMS-F-001, FCMS-F-002  
**Assessment Framework:** NIST SP 800-53 Revision 5, Release 5.2.0, and NIST SP 800-53A Revision 5, Release 5.2.0

## 1. Purpose

This Plan of Action and Milestones (POA&M) documents proposed corrective actions for potential control deficiencies identified during the fictional FCMS-001 security assessment.

The plan connects each finding to its supporting synthetic evidence, proposed remediation activities, milestones, closure criteria, and validation requirements.

All actions and dates are proposed for the simulation. No actual federal agency, production system, or operational remediation activity is represented.

## 2. POA&M Summary

| POA&M ID | Finding ID | Control | Finding title | Preliminary severity | Status |
|---|---|---|---|---|---|
| FCMS-POAM-001 | FCMS-F-001 | AC-2 — Account Management | Account deactivation timeframe is not defined | Moderate — provisional | Open — proposed |
| FCMS-POAM-002 | FCMS-F-002 | AU-2 — Event Logging | Logging event selection requires validation | Undetermined | Open — proposed |

Severity ratings and remediation priorities have not been formally approved. The status of each item must be reassessed if validation changes the underlying finding.

## 3. FCMS-POAM-001 — Account Management

**Related finding:** FCMS-F-001  
**Control:** AC-2 — Account Management  
**Evidence:** EV-001  
**Preliminary severity:** Moderate — provisional  
**Status:** Open — proposed

### 3.1 Condition

The synthetic account lifecycle procedure assigns responsibility for disabling accounts but does not define a maximum timeframe for removing access when an employee leaves the program or no longer requires access. Completed deactivation records are not available in the scenario.

### 3.2 Potential Risk

If access is not removed promptly when it is no longer required, unnecessary access to applicant records or administrative functions could persist.

The actual likelihood and impact have not been established. The preliminary severity is a scenario judgment and requires validation against documented risk-rating criteria.

### 3.3 Proposed Corrective Action

Define and approve a risk-based account deactivation timeframe. Establish escalation and exception procedures, and retain records showing when access-removal requests are received and when accounts are disabled.

Validate the approved procedure against the applicable account-management requirements and determine whether the process operates as intended.

### 3.4 Proposed Milestones

| Milestone | Activity | Expected evidence | Status |
|---|---|---|---|
| M1 | Review applicable account-management requirements and organizational policy | Documented requirements and proposed timeframe | Planned |
| M2 | Approve the account deactivation procedure, including escalation and exceptions | Approved procedure and designated responsibilities | Planned |
| M3 | Implement the procedure and retain access-removal records | Implementation evidence and completed request records | Planned |
| M4 | Evaluate a sample of account-removal events against the approved timeframe | Sample results, timestamps, and exception documentation | Planned |
| M5 | Conduct closure review | Documented reviewer decision and closure rationale | Planned |

### 3.5 Proposed Closure Criteria

The finding may be considered for closure when:

- An approved account deactivation timeframe and exception process are documented.
- The responsible team demonstrates that the process has been implemented.
- A sample of account-removal events is evaluated against the approved timeframe.
- Identified exceptions are assessed and addressed.
- A designated reviewer determines that the available evidence supports closure.

A documented procedure alone may not be sufficient to establish that the control operates effectively.

### 3.6 Ownership and Schedule

**Proposed owner:** System owner or designated identity and access management lead.  
**Target dates:** To be determined after requirements, responsibilities, and implementation constraints are established.  
**Risk acceptance:** Not determined.

These are proposed roles and planning assumptions, not actual assignments.

## 4. FCMS-POAM-002 — Event Logging

**Related finding:** FCMS-F-002  
**Control:** AU-2 — Event Logging  
**Evidence:** EV-004  
**Preliminary severity:** Undetermined  
**Status:** Open — proposed

### 4.1 Condition

The synthetic event-selection list does not include administrative configuration changes or changes to logging settings and destinations. The available documentation does not establish whether these events are required, intentionally excluded, or captured through other mechanisms.

### 4.2 Potential Risk

If required administrative or logging-configuration changes are not recorded, investigators may have difficulty determining who changed security settings, what changed, and when the change occurred.

The actual likelihood and impact cannot be determined from the synthetic evidence.

### 4.3 Proposed Corrective Action

Validate the applicable logging requirements and document an approved event-selection rationale.

If validation confirms that required events are not being generated or recorded, update the relevant logging requirements and configurations, then verify that the required events are generated and delivered to the intended destination.

If the existing configuration already satisfies applicable requirements, document the supporting rationale and reassess whether the finding remains warranted.

### 4.4 Proposed Milestones

| Milestone | Activity | Expected evidence | Status |
|---|---|---|---|
| M1 | Review applicable logging requirements and organizational policy | Approved requirements or documented policy basis | Planned |
| M2 | Determine which event categories must be captured and document the rationale | Approved event-selection decision | Planned |
| M3 | If a gap is confirmed, implement the required logging changes | Updated configuration and change records | Conditional |
| M4 | Validate the relevant events and their delivery to the intended destination | Configuration evidence and sample event records | Planned |
| M5 | Conduct closure review or reassess the finding if no deficiency is confirmed | Documented reviewer decision and rationale | Planned |

### 4.5 Proposed Closure Criteria

The finding may be considered for closure when:

- Applicable logging requirements and the event-selection rationale are documented.
- The assessment determines whether administrative and logging-configuration changes must be captured.
- Any confirmed deficiencies are corrected.
- Relevant configuration records and sample events demonstrate that required events are generated and captured.
- A designated reviewer determines that the evidence supports closure.

If validation determines that the existing configuration satisfies the applicable requirements, the assessor should document the rationale and determine whether the finding should be withdrawn or otherwise resolved.

### 4.6 Ownership and Schedule

**Proposed owner:** System owner or designated security logging lead.  
**Target dates:** To be determined after the requirements and any confirmed gaps are established.  
**Risk acceptance:** Not determined.

These are proposed roles and planning assumptions, not actual assignments.

## 5. Traceability

| Evidence | Finding | POA&M | Relationship |
|---|---|---|---|
| EV-001 | FCMS-F-001 | FCMS-POAM-001 | Synthetic account lifecycle procedure lacks a defined maximum deactivation timeframe |
| EV-004 | FCMS-F-002 | FCMS-POAM-002 | Synthetic event-selection documentation lacks a documented rationale for excluding certain event categories |

This traceability supports review of the relationship between the observed scenario condition, the potential risk, and the proposed corrective action.

## 6. Tracking and Review Requirements

For an actual system, the POA&M would be maintained with approved owners, target completion dates, risk priorities, status updates, dependencies, and supporting implementation evidence.

For this simulation, those operational details remain unassigned. No action should be represented as completed until the corresponding evidence exists and has been reviewed.

Changes to a finding's condition, severity, or validation status should be reflected consistently in the findings register, assessment report, and POA&M.

## 7. References

- [NIST SP 800-53 Revision 5, Release 5.2.0 — Security and Privacy Controls for Information Systems and Organizations](https://csrc.nist.gov/pubs/sp/800/53/r5/upd1/final)
- [NIST SP 800-53A Revision 5, Release 5.2.0 — Assessing Security and Privacy Controls in Information Systems and Organizations](https://csrc.nist.gov/pubs/sp/800/53/a/r5/final)
- [NIST SP 800-53B, Release 5.2.0 — Control Baselines for Information Systems and Organizations](https://csrc.nist.gov/pubs/sp/800/53/b/upd1/final)

## 8. Simulation Disclaimer

FCMS-001, FCMS-F-001, FCMS-F-002, FCMS-POAM-001, FCMS-POAM-002, and all associated evidence are fictional.

This document is an educational portfolio artifact. It does not represent an actual federal agency finding, approved remediation deadline, completed corrective action, or formal authorization decision.
