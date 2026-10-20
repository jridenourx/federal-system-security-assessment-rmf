# EV-001 — Account Management Evidence

**Classification:** SIMULATED EVIDENCE — NOT FROM A REAL SYSTEM  
**System:** FCMS-001 — Federal Benefits Case Management System  
**Control:** NIST SP 800-53 Rev. 5, AC-2 — Account Management  
**Evidence Type:** Synthetic account inventory and lifecycle review  
**Scenario Date:** October 20, 2026  
**Prepared For:** Educational security control assessment

## 1. Objective

Assess whether FCMS-001 maintains an account inventory and has a defined process for removing access when personnel no longer require it.

## 2. Scenario Background

For this fictional exercise, the assessor receives a synthetic account inventory and a short description of the account deactivation process.

The scenario does not represent an actual AWS account, federal agency, identity provider, or production environment.

## 3. Synthetic Evidence A — Account Inventory

| Account ID | Assigned role | Account status | Last review |
|---|---|---|---|
| FCMS-USER-014 | Benefits Caseworker | Active | September 30, 2026 |
| FCMS-USER-027 | Benefits Supervisor | Active | September 30, 2026 |
| FCMS-ADMIN-003 | System Administrator | Active | September 30, 2026 |
| FCMS-USER-041 | Benefits Caseworker | Active | September 30, 2026 |

These records are illustrative examples created for this exercise. They are not extracted from a real system.

## 4. Synthetic Evidence B — Account Deactivation Procedure

The fictional procedure states:

- A supervisor submits an account removal request when an employee leaves the program or changes duties.
- An administrator is responsible for disabling the account.
- The procedure does not specify a maximum time for disabling access after notification.
- The scenario includes no completed deactivation tickets or records demonstrating how quickly access was removed.

## 5. Evidence Review

**Evidence reviewed:** Synthetic account inventory and synthetic account deactivation procedure.

**Observations:**

1. The inventory identifies account IDs, assigned roles, status, and a review date.
2. The procedure assigns responsibility for submitting requests and disabling accounts.
3. The procedure does not define a required deactivation timeframe.
4. No completed deactivation records are available to demonstrate that the process operates as described.

**Limitations:** The evidence does not establish whether any unauthorized or unnecessary account remains active. It also does not demonstrate actual system behavior.

## 6. Preliminary Assessment Conclusion

**Status: Potential control gap identified — validation required.**

The missing deactivation timeframe may make it difficult to determine whether access is removed promptly when no longer needed. The lack of completed deactivation records also limits the assessor's ability to evaluate whether the process operates effectively.

The available synthetic evidence is insufficient to conclude that AC-2 is fully effective or definitively ineffective. Additional evidence and defined assessment criteria are required.

## 7. Additional Evidence Requested

- The approved account management policy and applicable deactivation timeframe.
- Sample completed account removal requests and corresponding disablement timestamps.
- Evidence of periodic account reviews and follow-up on identified discrepancies.
- Confirmation of how emergency access removal is handled.

## 8. Recommended Corrective Action

Define and approve an account deactivation timeframe based on organizational requirements and risk. Retain account removal records that demonstrate when requests were received, when access was disabled, and how exceptions were handled.

## 9. Simulation Disclaimer

All accounts, roles, dates, procedures, and observations in this artifact are fictional. This artifact does not demonstrate actual control testing or an assessment of a real system.
