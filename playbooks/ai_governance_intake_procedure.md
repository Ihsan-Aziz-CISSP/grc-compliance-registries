# Playbook: Artificial Intelligence (AI) Use Case Governance & Intake

## 1. Purpose
This playbook defines the operational workflow for triaging, assessing, and approving or rejecting net-new AI Agent and Large Language Model (LLM) use cases submitted by business units across the Ascendiun Family of Companies.

## 2. Intake and Triage Workflow
All AI requests arriving via the ticketing system or dedicated email intake must be cataloged and categorized within 24 hours based on the following risk tiering matrix:

### Use Case Risk Tiering
* **Tier 1: Prohibited Risk** (Immediate Rejection)
  * Real-time biometric tracking without explicit statutory exemptions.
  * Cognitive behavioral manipulation scripts.
* **Tier 2: High Risk** (Requires Comprehensive Assessment)
  * Clinical decision support tools mapping to patient diagnostics.
  * Automated resume screening or HR talent management models.
* **Tier 3: Limited / Specific Risk** (Requires Transparency Controls)
  * Customer-facing chatbots providing administrative or benefit navigation support.
  * Synthetic text/image generation platforms.

## 3. Control Assessment Checklists
For Tier 2 and Tier 3 systems, the analyst must verify the following controls before scheduling the project for the AI Governance Forum:

1. **Data Provenance:** Document data sources. Verify that no Protected Health Information (PHI) or personally identifiable information (PII) is transmitted to public model endpoints.
2. **Vendor Assessment:** Confirm whether the third-party provider provides a signed Business Associate Agreement (BAA) and enforces a Zero Data Retention (ZDR) policy.
3. **Technical Controls:** Enforce digital watermarking on outputs and verify that strict input sanitization/LLM firewalls are planned to prevent prompt injection.

## 4. Escalation and Consequence Management
If a business unit deploys an unapproved "Shadow AI" system outside this workflow:
1. Issue an immediate system isolation/API token revocation request to NetSec.
2. Log the event in the root cause analysis queue.
3. Schedule a mandatory AI Acceptable Use awareness briefing for the department head.
