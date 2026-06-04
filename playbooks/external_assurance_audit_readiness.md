# Playbook: SOC 2 and PCI-DSS External Assurance Audit Coordination

## 1. Purpose
Provides a standardized framework for preparing engineering asset owners, consolidating evidence requests, and managing continuous control monitoring to fulfill annual SOC 2 Type II and PCI-DSS v4.0 compliance audits.

## 2. Pre-Audit Continuous Evidence Mapping
Rather than executing reactive evidence collection cycles, asset owners must map system evidence continuously to the unified controls structure below:

| Framework ID | Target Framework Requirement | Required Artifact / Evidence Type | Verification Frequency |
| :--- | :--- | :--- | :--- |
| **SOC2-CC6.1** | Boundary Protection / Perimeter Controls | Firewall configuration rulesets, IAM access logs, ingress network topology diagrams. | Quarterly |
| **PCI-v4-CC3** | Account Management & Account Security | Identity Provider (IdP) configurations, MFA enforcement logs, inactive account removal scripts. | Monthly |
| **NIST-PR.AC-1** | Identity Management and Access Control | Semi-annual privilege access reviews (PAR) signed off by system owners. | Bi-Annually |

## 3. Evidence Intake Triage & Execution
When external auditors issue Information Request Lists (IRLs) through the ticketing queue, the compliance specialist will execute the following:

1. **De-identification Verification:** Review the requested screenshots, system exports, or log arrays to ensure absolutely zero production patient data (PHI) is exposed within the evidence bundle.
2. **Quality Assurance Check:** Cross-reference the timestamp of the artifact with the specific audit window requested. Reject and return stale evidence back to asset owners within 48 hours.
3. **Centralized Repository Staging:** Upload verified, sanitized evidence files into the secure compliance data room, tracking completion metrics on the central dashboard.
