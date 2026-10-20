# Control Assessment Matrix — FCMS-001

**Document Status:** Draft — Simulation  
**System ID:** FCMS-001  
**Assessment Reference:** NIST SP 800-53 Rev. 5 and SP 800-53A Rev. 5  
**Assessment Type:** Tabletop control assessment using synthetic evidence  
**Important:** No actual federal system or AWS environment has been assessed.

## 1. Purpose and Scope

This matrix documents selected security controls, the evidence needed to assess them, the proposed assessment procedures, and illustrative results for the fictional Federal Benefits Case Management System (FCMS-001).

The assessment uses the methods described in NIST SP 800-53A: examine documentation or configurations, interview responsible personnel, and test control operation where appropriate.

The controls below are a focused sample, not a complete Moderate baseline or an official assessment plan.

## 2. Assessment Method

- **Examine:** Review policies, configurations, logs, access lists, and other evidence.
- **Interview:** Ask system owners or administrators how a control is implemented and operated.
- **Test:** Perform a defined procedure to determine whether the control behaves as expected.

Evidence must support the assessment conclusion. A policy alone does not prove a technical control is operating effectively.

## 3. Control Assessment Matrix

| Control | Assessment objective | Evidence requested | Assessment procedure | Illustrative result |
|---|---|---|---|---|
| AC-2 — Account Management | Accounts are approved, managed, and removed when no longer needed | Account inventory, onboarding/offboarding procedures, recent access-change records | Examine account records and sample joiner, mover, and leaver events; interview the administrator about removal timelines | Not assessed — evidence not yet evaluated |
| AC-6 — Least Privilege | Users receive only the access needed for assigned duties | Role-permission matrix, privileged account list, access review records | Compare assigned permissions with job responsibilities; investigate unnecessary privileges | Not assessed — evidence not yet evaluated |
| IA-2 — Identification and Authentication | Users are individually identified and authenticated | Authentication configuration, MFA settings, identity integration design | Examine authentication settings and determine whether privileged and ordinary users have appropriate authentication protections | Not assessed — evidence not yet evaluated |
| AU-2 — Event Logging | Relevant security events are identified for logging | Logging requirements, event configuration, sample log records | Compare configured event types with documented requirements and confirm that relevant events are generated | Not assessed — evidence not yet evaluated |
| AU-6 — Audit Record Review, Analysis, and Reporting | Audit records are reviewed for suspicious or unauthorized activity | Review procedures, alert rules, sample review records, incident tickets | Examine evidence of reviews and follow up on a sample of alerts or anomalies | Not assessed — evidence not yet evaluated |
| CM-6 — Configuration Settings | System components use defined and approved security settings | Configuration baseline, deployment settings, exception records | Compare selected configurations with the approved baseline and investigate deviations | Not assessed — evidence not yet evaluated |
| CP-9 — System Backup | System information is backed up according to defined requirements | Backup policy, backup-job records, retention settings | Examine backup configurations and job history; determine whether backup coverage matches documented requirements | Not assessed — evidence not yet evaluated |
| IR-4 — Incident Handling | Security incidents are handled through defined procedures | Incident response plan, incident records, exercise results | Examine response procedures and a sample incident or tabletop exercise; determine whether responsibilities and escalation steps are defined | Not assessed — evidence not yet evaluated |
| RA-5 — Vulnerability Monitoring and Scanning | Vulnerabilities are identified and tracked | Scan reports, scan schedules, vulnerability tickets, remediation records | Examine a representative scan report and trace selected findings to documented remediation or risk acceptance | Not assessed — evidence not yet evaluated |
| SI-2 — Flaw Remediation | Identified system flaws are corrected within defined requirements | Patch policy, vulnerability tickets, patch records, exceptions | Sample selected flaws and trace them from identification through remediation or documented exception | Not assessed — evidence not yet evaluated |

## 4. Evidence Handling and Assessment Rules

For this simulation:

1. Evidence must be identified by a unique reference, date, source, and description.
2. Synthetic evidence must be labeled clearly and must never be presented as an actual system record.
3. Each assessment conclusion must be traceable to the relevant evidence and procedure.
4. Missing evidence must not automatically be treated as proof that a control is ineffective.
5. A control deficiency should be documented when available evidence supports a finding.
6. In a real assessment, the assessor would consider the full assessment objectives, applicable control enhancements, organizational parameters, and approved assessment plan.

## 5. Preliminary Assessment Status

No controls have been marked effective or ineffective at this stage. The matrix currently defines what evidence would be requested and how it would be evaluated.

The next exercise will introduce clearly labeled synthetic evidence for a small number of controls. The evidence will be reviewed against explicit assessment criteria to support defensible illustrative results.

## 6. References

- NIST SP 800-53 Rev. 5 — Security and Privacy Controls for Information Systems and Organizations: https://csrc.nist.gov/pubs/sp/800/53/r5/upd1/final
- NIST SP 800-53A Rev. 5 — Assessing Security and Privacy Controls in Information Systems and Organizations: https://csrc.nist.gov/pubs/sp/800/53/a/r5/final
- NIST SP 800-53B — Control Baselines for Information Systems and Organizations: https://csrc.nist.gov/pubs/sp/800/53/b/upd1/final

## 7. Simulation Disclaimer

FCMS-001 is fictional. The matrix is a learning artifact and does not establish that any real control has been implemented, tested, or found compliant.
