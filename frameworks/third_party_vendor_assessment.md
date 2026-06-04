# Enterprise Third-Party AI & IT Vendor Risk Assessment Framework

## 1. Purpose
This framework defines the mandatory Information Security and Compliance vetting requirements for all external IT vendors, SaaS applications, and foundational model providers procuring data processing agreements within the Ascendiun Family of Companies.

## 2. Mandatory Vendor Security Questionnaire

### Section A: Data Governance & Privacy (HIPAA Focus)
* **Q 1.1:** Will your application process, store, or transmit Protected Health Information (PHI) or Personally Identifiable Information (PII)?
* **Q 1.2:** Will your organization execute a formal Business Associate Agreement (BAA) with Blue Shield of California?
* **Q 1.3:** Do you enforce a verified Zero Data Retention (ZDR) policy for API data payloads, ensuring consumer prompt inputs are never cached or used for downstream model fine-tuning?

### Section B: External Assurance & Audits
* **Q 2.1:** Provide your most recent SOC 2 Type II audit report. Does the report contain any qualified opinions or significant exceptions within the Trust Services Criteria (Security, Confidentiality, Availability)?
* **Q 2.2:** Is your platform fully compliant with PCI-DSS v4.0 for cardholder environments (if processing premiums/billing transactions)?
* **Q 2.3:** Map your current security control environment to the NIST Cybersecurity Framework (CSF) subcategories and state your assessed maturity level.

### Section C: Artificial Intelligence Security & Trustworthiness
* **Q 3.1:** What technical mechanisms are utilized to defend your LLM endpoints against prompt injection, data poisoning, and model inversion attacks?
* **Q 3.2:** Do you provide transparent documentation detailing the data provenance and copyright statuses of the datasets used to train your core models?
* **Q 3.3:** How are algorithmic bias testing and output validation performed to prevent clinical safety hallucinations?

---

## 3. Risk Scoring & Procurement Approval Paths

| Assessment Result / Findings | Risk Tier | Required Approval Authority |
| :--- | :--- | :--- |
| Missing SOC 2 Type II **OR** Refusal to sign BAA for PHI workloads. | **Critical Risk** | **Immediate Rejection** (No Exceptions) |
| Missing automated output watermarking; signed BAA present. | **Medium Risk** | AI Governance Forum Review & Mitigation Sign-off |
| Fully certified SOC 2 Type II, signed BAA, Zero Data Retention enforced. | **Low Risk** | Standard Operational Intake Approval |
