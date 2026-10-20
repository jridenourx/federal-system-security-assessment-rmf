# Security Findings Register — FCMS-001

**Document Status:** Draft — Simulation  
**System ID:** FCMS-001  
**Assessment Type:** Tabletop assessment using synthetic evidence  
**Finding Count:** 1 preliminary finding

## 1. Purpose

This register documents potential security control deficiencies identified during the fictional FCMS-001 assessment. Each finding links the observed condition to its supporting evidence, potential risk, and recommended corrective action.

All findings are illustrative. They are not findings from a real federal agency, AWS environment, or production security assessment.

## 2. Findings Summary

| Finding ID | Control | Finding title | Preliminary severity | Status |
|---|---|---|---|---|
| FCMS-F-001 | AC-2 — Account Management | Account deactivation timeframe is not defined | Moderate — preliminary | Open; validation required |

The severity is an initial scenario judgment, not a calculated or approved risk rating. It must be reassessed using the agency's risk criteria, actual exposure, and potential impact.

## 3. FCMS-F-001 — Account Deactivation Timeframe Is Not Defined

**Related control:** AC-2 — Account Management  
**Evidence reference:** EV-001  
**Status:** Open; validation required  
**Preliminary severity:** Moderate — provisional

### Condition

The synthetic account deactivation procedure assigns responsibility for disabling accounts but does not define a maximum timeframe for removing access after an employee leaves the program or no longer requires access. The scenario also lacks completed deactivation records demonstrating how the procedure operates.

### Criteria

Account management processes should define how accounts are managed throughout their lifecycle, including when access is no longer required. The applicable AC-2 requirements and organizational parameters must be confirmed against the selected control baseline and agency policy.

### Cause

The fictional procedure does not specify an approved deactivation service level or documented exception process.

This is the apparent cause within the scenario; it has not been independently verified.

### Potential risk and impact

If access is not removed promptly when it is no longer required, a former employee or other unauthorized user could retain an opportunity to access applicant records or perform unauthorized actions.

The actual likelihood and impact cannot be established from the available synthetic evidence.

### Recommendation

Define and approve a risk-based account deactivation timeframe. Establish an exception and escalation process, and retain records showing when access-removal requests are received, when accounts are disabled, and whether required timeframes are met.

### Evidence supporting the finding

- **EV-001:** Synthetic account inventory and account lifecycle procedure.
- The procedure assigns responsibility for deactivation but does not specify a required timeframe.
- No completed deactivation records are available in the scenario.

### Additional validation required

1. Confirm the applicable AC-2 requirements and organizational policy.
2. Obtain sample deactivation tickets and corresponding disablement timestamps.
3. Determine whether a timeframe exists in another approved policy or procedure.
4. Evaluate whether the observed condition represents a control deficiency under the applicable assessment criteria.
5. Reassess severity using documented risk-rating criteria.

## 4. Proposed Remediation Tracking

The following is a proposed action, not evidence that remediation has occurred.

| Action ID | Corrective action | Proposed owner | Target date | Status |
|---|---|---|---|---|
| FCMS-A-001 | Define the account deactivation timeframe, document escalation procedures, and retain completion evidence | System owner and identity/access administrator | To be assigned | Proposed |

The target date should be assigned by the responsible owner based on the approved remediation process and risk priority. No completion date is assumed.

## 4.1 FCMS-F-002 — Logging Event Selection Requires Validation

**Related control:** AU-2 — Event Logging  
**Evidence reference:** EV-004  
**Status:** Open; validation required  
**Preliminary severity:** Undetermined

### Condition

The synthetic draft event list does not include administrative configuration changes or changes to logging settings and destinations. The available documentation does not establish whether these events are required, intentionally excluded, or captured through other mechanisms.

### Criteria

The applicable AU-2 requirements, organizational logging policy, and approved system event-selection rationale should establish which events must be logged. The exact applicable control requirements and organizational parameters must be confirmed against the selected baseline.

### Cause

The fictional scenario lacks a documented, approved rationale for selecting and excluding security-relevant event categories.

This is the apparent cause within the scenario, not an independently verified root cause.

### Potential risk and impact

If required administrative or logging-configuration changes are not recorded, investigators may have difficulty determining who changed security settings, what changed, and when the change occurred.

The actual likelihood and impact cannot be determined from the synthetic evidence.

### Recommendation

Document and approve the event-selection rationale. Confirm which administrative and logging-configuration events are required, then examine relevant configuration exports and sample records to determine whether the required events are generated and captured.

### Evidence supporting the finding

- **EV-004:** Synthetic event list and logging configuration summary.
- Administrative configuration changes and logging-configuration changes are absent from the draft list.
- No actual technical configuration or log records are available.

### Additional validation required

1. Obtain the approved logging policy and event-selection rationale.
2. Determine whether the missing event categories are required.
3. Review relevant configuration settings and sample event records.
4. Confirm whether other logging mechanisms capture the events.
5. Assign a severity only after the condition and associated risk are sufficiently established.

### Proposed corrective action

If validation confirms a gap, update the logging requirements, configure the applicable event sources, and retain evidence demonstrating that required events are generated and delivered to the intended destination.

## 5. Findings Summary

| Finding ID | Control | Finding title | Preliminary severity | Status |
|---|---|---|---|---|
| FCMS-F-001 | AC-2 — Account Management | Account deactivation timeframe is not defined | Moderate — provisional | Open; validation required |
| FCMS-F-002 | AU-2 — Event Logging | Logging event selection requires validation | Undetermined | Open; validation required |

## 6. Closure Criteria

The finding may be considered for closure when:

- An approved account deactivation timeframe and exception process are documented.
- The responsible team demonstrates the process using appropriate records.
- A sample of account removal events is evaluated against the approved timeframe.
- The designated reviewer confirms that the corrective action adequately addresses the finding.

A documented procedure alone may not be sufficient to demonstrate that the control operates effectively.

## 7. Simulation Disclaimer

FCMS-001, finding FCMS-F-001, and all supporting evidence are fictional. This register is a portfolio learning artifact and does not represent an actual security incident, confirmed vulnerability, or formal federal assessment finding.
