# Control Assessment Matrix — FCMS-001

**Document Status:** Draft — Simulation  
**System ID:** FCMS-001  
**Assessment Reference:** NIST SP 800-53 Revision 5, Release 5.2.0, and NIST SP 800-53A Revision 5, Release 5.2.0  
**Assessment Type:** Tabletop control assessment using synthetic evidence  
**Important:** No actual federal system or AWS environment has been assessed.

## 1. Purpose and Scope

This matrix documents selected security controls, the evidence needed to assess them, the proposed assessment procedures, and illustrative results for the fictional Federal Benefits Case Management System (FCMS-001).

The assessment uses methods described in NIST SP 800-53A: examine documentation or configurations, interview responsible personnel, and test control operation where appropriate.

The controls below are a focused sample, not a complete Moderate baseline or an official assessment plan.

## 2. Assessment Method

- **Examine:** Review policies, configurations, logs, access lists, and other evidence.
- **Interview:** Ask system owners or administrators how a control is implemented and operated.
- **Test:** Perform a defined procedure to determine whether the control behaves as expected.

Evidence must support the assessment conclusion. A policy alone does not prove that a technical control is operating effectively.

For this portfolio exercise, preliminary conclusions are limited to the synthetic artifacts created and reviewed. They do not establish the effectiveness of controls in a real system.

## 3. Control Assessment Matrix

| Control | Assessment objective | Evidence requested | Assessment procedure | Illustrative result |
|---|---|---|---|---|
| AC-2 — Account Management | Accounts are approved, managed, and removed when no longer needed | **EV-001:** Synthetic account inventory and account lifecycle procedure; additional deactivation records requested | Examine the synthetic inventory and procedure; identify whether a maximum deactivation timeframe is defined; request completed deactivation records to validate operation | **Preliminary potential deficiency identified.** EV-001 does not define a maximum deactivation timeframe, and completed deactivation records were not provided. Validation is required before making a formal control-effectiveness determination. See FCMS-F-001. |
| AC-6 — Least Privilege | Users receive only the access needed for assigned duties | **EV-002:** Synthetic role-permission matrix and privileged account listing; access review records | Compare assigned permissions with job responsibilities; investigate unnecessary privileges | Not assessed — evidence not yet evaluated |
| IA-2 — Identification and Authentication | Users are individually identified and authenticated | **EV-003:** Synthetic authentication configuration summary; MFA settings and identity integration design | Examine authentication settings and determine whether privileged and ordinary users have appropriate authentication protections | Not assessed — evidence not yet evaluated |
| AU-2 — Event Logging | Relevant security events are identified for logging | **EV-004:** Synthetic event-selection list and logging configuration summary; approved logging requirements and configuration evidence requested | Compare the synthetic event-selection list with documented requirements; identify event types whose inclusion or exclusion requires justification; request approved requirements and configuration evidence | **Preliminary documentation gap identified.** EV-004 does not document the basis for excluding administrative configuration changes and logging configuration or destination changes. This does not establish that required events are technically missing. Validation is required before making a formal control-effectiveness determination. See FCMS-F-002. |
| AU-6 — Audit Record Review, Analysis, and Reporting | Audit records are reviewed for suspicious or unauthorized activity | **EV-005:** Synthetic audit-log review procedure and review records; alert rules and incident tickets | Examine evidence of reviews and follow up on a sample of alerts or anomalies | Not assessed — evidence not yet evaluated |
| CM-6 — Configuration Settings | System components use defined and approved security settings | **EV-009:** Synthetic configuration baseline, configuration settings summary, and exception records | Compare selected configurations with the approved baseline and investigate deviations | Not assessed — evidence not yet evaluated |
| CP-9 — System Backup | System information is backed up according to defined requirements | **EV-006:** Synthetic backup configuration summary and backup-job history; retention settings | Examine backup configurations and job history; determine whether backup coverage matches documented requirements | Not assessed — evidence not yet evaluated |
| IR-4 — Incident Handling | Security incidents are handled through defined procedures | **EV-010:** Synthetic incident response procedures, incident records, or tabletop exercise results | Examine response procedures and a sample incident or tabletop exercise; determine whether responsibilities and escalation steps are defined | Not assessed — evidence not yet evaluated |
| RA-5 — Vulnerability Monitoring and Scanning | Vulnerabilities are identified and tracked | **EV-007:** Synthetic vulnerability scan summary and finding records; scan schedules and remediation records | Examine a representative scan report and trace selected findings to documented remediation or risk acceptance | Not assessed — evidence not yet evaluated |
| SI-2 — Flaw Remediation | Identified system flaws are corrected within defined requirements | **EV-008:** Synthetic remediation tickets and patch records; policy and exception records | Sample selected flaws and trace them from identification through remediation or documented exception | Not assessed — evidence not yet evaluated |

## 4. Evidence Handling and Assessment Rules

For this simulation:

1. Evidence must be identified by a unique reference, date, source, and description.
2. Synthetic evidence must be labeled clearly and must never be presented as an actual system record.
3. Each assessment conclusion must be traceable to the relevant evidence and procedure.
4. Missing evidence must not automatically be treated as proof that a control is ineffective.
5. A potential control deficiency must be documented when available evidence supports a specific concern, with limitations and further validation needs stated.
6. In a real assessment, the assessor would consider the full assessment objectives, applicable control enhancements, organizational parameters, and approved assessment plan.
7. A preliminary finding based on synthetic evidence is not a formal determination that a real control is ineffective.

## 5. Preliminary Assessment Status

Two controls have received a preliminary tabletop review using synthetic evidence:

- **AC-2 — Account Management:** EV-001 supports a potential deficiency because the simulated procedure does not define a maximum account-deactivation timeframe. Completed deactivation records were not provided, so operational effectiveness has not been established.
- **AU-2 — Event Logging:** EV-004 supports a potential documentation gap because the rationale for excluding certain event types is not documented. The available artifact does not establish whether those events are required or whether they are captured elsewhere.

Both issues require validation. The remaining eight controls have not been assessed, and no control has been formally determined effective or ineffective.

## 6. References

- NIST SP 800-53 Revision 5, Release 5.2.0 — *Security and Privacy Controls for Information Systems and Organizations*: https://csrc.nist.gov/pubs/sp/800/53/r5/upd1/final
- NIST SP 800-53A Revision 5, Release 5.2.0 — *Assessing Security and Privacy Controls in Information Systems and Organizations*: https://csrc.nist.gov/pubs/sp/800/53/a/r5/final
- NIST SP 800-53B, Release 5.2.0 — *Control Baselines for Information Systems and Organizations*: https://csrc.nist.gov/pubs/sp/800/53/b/upd1/final

## 7. Simulation Disclaimer

FCMS-001 is fictional. The matrix is a portfolio learning artifact and does not establish that any real control has been implemented, tested, or found compliant.
