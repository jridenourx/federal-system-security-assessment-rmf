# EV-004 — Event Logging Evidence

**Classification:** SIMULATED EVIDENCE — NOT FROM A REAL SYSTEM  
**System:** FCMS-001 — Federal Benefits Case Management System  
**Control:** NIST SP 800-53 Rev. 5, AU-2 — Event Logging  
**Evidence Type:** Synthetic logging requirements and configuration review  
**Scenario Date:** October 20, 2026

## 1. Assessment Objective

Determine whether the fictional system has identified the security-relevant events that should be logged and documented requirements for generating those records.

AU-2 concerns the identification of events to be logged. The assessment must also consider applicable organizational requirements and related audit controls.

## 2. Scenario Background

For this tabletop exercise, the assessor reviews a fictional logging configuration summary and a draft list of security events.

The scenario assumes that FCMS-001 uses an application, a relational database, object storage, and identity and access services. The specific AWS services and actual configurations have not been established.

All evidence below is synthetic and created solely for this exercise.

## 3. Synthetic Evidence A — Draft Event List

The fictional system documentation identifies the following candidate events:

| Event category | Example event | Included in draft list? |
|---|---|---|
| Authentication | Successful and failed sign-in attempts | Yes |
| Account management | Account creation, disabling, and privilege changes | Yes |
| Authorization | Denied access to restricted application functions | Yes |
| Benefits records | Changes to application status and eligibility decisions | Yes |
| Administrative activity | Changes to security-related configuration | No |
| Audit configuration | Changes to logging settings or log destinations | No |

This table represents a draft list, not proof that any event is actually generated or recorded.

## 4. Synthetic Evidence B — Logging Configuration Summary

The fictional configuration summary states:

- Application authentication events are intended to be logged.
- Changes to benefits application records are intended to be logged.
- The scenario provides no documented decision explaining which administrative configuration changes must be logged.
- The scenario provides no documented decision about recording changes to logging settings or log destinations.
- No actual configuration exports, event records, or log-delivery tests are available.

These are assumptions established for the exercise, not observations from an actual AWS environment.

## 5. Evidence Review

**Evidence reviewed:** Synthetic draft event list and synthetic logging configuration summary.

**Observations:**

1. The draft list identifies several security-relevant event categories.
2. Administrative configuration changes and changes to logging settings are not included in the draft list.
3. The available documentation does not explain whether these omissions are intentional or justified.
4. No technical evidence demonstrates that the listed events are generated, retained, or delivered to a central logging destination.

**Assessment limitation:** A missing event category in a draft list does not, by itself, establish that the event is not logged in practice. The assessor needs the approved logging requirements and relevant technical evidence.

## 6. Preliminary Assessment Conclusion

**Status: Potential control gap identified — validation required.**

The available synthetic documentation does not establish that the system has fully identified and justified the security-relevant events that should be logged.

The assessor should obtain an approved event-selection rationale and determine whether administrative configuration changes and logging-configuration changes are required by applicable organizational policy and the system's risk profile.

No definitive conclusion about control effectiveness is assigned at this stage.

## 7. Additional Evidence Requested

- Approved event-logging requirements and event-selection rationale.
- Relevant application and cloud-service logging configuration exports.
- Sample records for selected security-relevant events.
- Documentation identifying log destinations, access restrictions, and retention requirements.
- Evidence that selected events are generated and delivered as intended.

## 8. Recommended Next Action

Document and approve the event-selection rationale, including whether administrative configuration changes and logging-configuration changes must be captured.

If technical evidence later demonstrates that required events are not generated or recorded, document the confirmed condition, assess the associated risk, and recommend a corrective action.

## 9. Simulation Disclaimer

FCMS-001, all event categories, and all configuration details in this artifact are fictional. No actual AWS configuration, application log, security event, or production system was examined.
