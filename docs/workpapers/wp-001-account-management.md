# Control Assessment Workpaper — WP-001

**System:** FCMS-001 — Federal Benefits Case Management System  
**Workpaper ID:** WP-001  
**Control:** AC-2 — Account Management  
**Evidence Reference:** EV-001  
**Related Finding:** FCMS-F-001  
**Assessment Type:** Tabletop assessment using synthetic evidence  
**Status:** Draft — Simulation

## 1. Assessment Objective

Evaluate whether the available scenario evidence supports the conclusion that the fictional FCMS-001 account management process defines responsibility and requirements for disabling accounts when access is no longer needed.

This workpaper documents an illustrative assessment procedure and its reasoning. It does not represent testing performed against a real system.

## 2. Assessment Criteria

The assessment considers the applicable AC-2 requirements and relevant organizational account management procedures.

The specific control requirements, organization-defined parameters, and assessment objectives must be confirmed against the selected baseline and applicable policy before a formal assessment conclusion is reached.

For this exercise, the key questions are:

- Is responsibility for account deactivation defined?
- Is a required timeframe for deactivation documented?
- Is there evidence that account removal events are processed according to the applicable requirements?

## 3. Evidence Reviewed

| Evidence ID | Description | Evidence limitation |
|---|---|---|
| EV-001 | Synthetic account inventory | Illustrative records only; no real accounts were examined |
| EV-001 | Synthetic account deactivation procedure | Does not specify a required deactivation timeframe |
| EV-001 | Scenario description of available records | No completed deactivation tickets or disablement timestamps are available |

## 4. Assessment Procedure

1. Examine the synthetic account inventory for account identifiers, roles, status, and review dates.
2. Examine the synthetic deactivation procedure to identify responsibilities and required actions.
3. Determine whether the procedure defines a timeframe for disabling access when it is no longer required.
4. Identify evidence needed to determine whether actual deactivation events meet applicable requirements.
5. Document observations, limitations, and the basis for any preliminary conclusion.

## 5. Assessment Results

| Assessment question | Result | Basis |
|---|---|---|
| Is responsibility for deactivation defined? | Supported by scenario evidence | The synthetic procedure assigns responsibility for submitting requests and disabling accounts |
| Is a required deactivation timeframe documented? | Not demonstrated | The synthetic procedure does not specify a maximum timeframe |
| Is effective operation demonstrated? | Insufficient evidence | No completed deactivation records or timestamps are available |

These results describe the synthetic evidence only. They do not establish the operating effectiveness of a real control.

## 6. Observation and Analysis

The scenario documentation assigns responsibility for disabling accounts but does not define a maximum deactivation timeframe.

Without an approved timeframe, the assessor cannot determine whether a particular deactivation delay would violate the applicable organizational requirement. The absence of completed deactivation records also prevents evaluation of whether the process operates as intended.

The documentation gap therefore warrants further validation. The assessor should not infer that unauthorized accounts exist or that access removal has failed without supporting evidence.

## 7. Preliminary Conclusion

**Conclusion: Potential control deficiency requiring validation.**

The available synthetic evidence does not demonstrate that the account management process defines an approved deactivation timeframe or that account removal events meet an established requirement.

This is a preliminary scenario conclusion, not a formal determination that AC-2 is ineffective.

## 8. Recommended Follow-up

Request the following:

- The approved account management policy and applicable deactivation timeframe.
- Completed account removal requests and corresponding disablement timestamps.
- Evidence of periodic account reviews and resolution of identified discrepancies.
- Documentation of exception handling and urgent access-removal procedures.

Evaluate the additional evidence against the confirmed control requirements before finalizing the finding and its severity.

## 9. Traceability

| Artifact | Relationship |
|---|---|
| EV-001 | Synthetic evidence reviewed |
| FCMS-F-001 | Related preliminary finding |
| FCMS-POAM-001 | Proposed remediation plan |

## 10. Simulation Disclaimer

FCMS-001, EV-001, and all observations in this workpaper are fictional. No real accounts, identity provider, AWS environment, or production evidence were examined. This workpaper does not represent a formal federal control assessment.
