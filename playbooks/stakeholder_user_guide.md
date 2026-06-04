# 👥 Stakeholder How-To Guide: Working with Our GRC Repository

Welcome! This repository is the central hub for security, compliance, and risk management across the Ascendiun Family of Companies. 

Because we manage compliance as a team, this guide explains exactly how **you** should use this page based on your specific job role. Find your role below for simple, step-by-step instructions.

---

## 1. For Business Leaders & Project Requesters
*Your goal: Launch new tools and AI features quickly and safely.*

### When to use this page:
Before you buy new software, build an AI agent, or start a project that handles customer data.

### Your Step-by-Step Instructions:
1. **Check the Rules First:** Go to the `/frameworks` folder and open `third_party_vendor_assessment.md`. Review Section A and Section C to see what security questions your vendor must pass.
2. **Review the AI Risk Log:** Go to the `/registries` folder and click on `ai_agents_risk_matrix.csv`. Look at the "Mitigation" column to see what security safeguards your team needs to build into your AI project.
3. **Submit a Request:** When you open a project ticket in our service desk, link to the specific Risk IDs (e.g., `AGENT-001`) to show the security team you have already reviewed the required guardrails.

---

## 2. For Software Engineers & Cloud Architects
*Your goal: Build stable systems without being slowed down by paperwork.*

### When to use this page:
During system design phases and before releasing code to production.

### Your Step-by-Step Instructions:
1. **Read the Security Standards:** Go to the `/playbooks` folder and review the `ai_governance_intake_procedure.md`. Ensure your application architecture matches the required risk tiering.
2. **Propose Changes via Pull Request (PR):** If you mitigate a risk or identify a new one, don't write an email. Open a Pull Request to update the status column in our `.csv` logs from `Open` to `Resolved`.
3. **Let Automation Check Your Work:** When you submit a PR, our automated pipeline (`csv-validator.yml`) will instantly scan your formatting. If you make a typo, the system will tell you exactly where to fix it before a human review even happens.

---

## 3. For Legal, Privacy, & Procurement Officers
*Your goal: Keep the company safe from lawsuits, data leaks, and fines.*

### When to use this page:
During contract negotiations with IT suppliers or when reviewing privacy guardrails.

### Your Step-by-Step Instructions:
1. **Evaluate IT Vendors:** Go to the `/frameworks` folder and use the `third_party_vendor_assessment.md` questionnaire during your vendor calls. 
2. **Enforce the Risk Matrix:** Scroll to Section 3 of the vendor framework to determine the approval path. If a healthcare vendor refuses to sign a Business Associate Agreement (BAA), use this page as your official policy ground to reject the vendor.
3. **Verify Compliance Mapping:** Go to the `/registries` folder and look at `healthcare_ai_compliance.csv` to ensure all data processing aligns legally with HIPAA requirements.

---

## 4. For External Auditors (SOC 2, PCI-DSS, Regulatory)
*Your goal: Verify that our company actively follows its security policies.*

### When to use this page:
During seasonal or annual audit windows.

### Your Step-by-Step Instructions:
1. **Review the History Book:** Do not ask for manual spreadsheets. Click on any file in the `/registries` folder and select the **History** button in the top right corner. You can view an unalterable, time-stamped trail of every compliance update made over the past year.
2. **Inspect Pre-Audit Playbooks:** Open `/playbooks/external_assurance_audit_readiness.md` to see exactly how our internal teams scrub and sanitize data before it reaches an audit bundle, ensuring absolute data privacy.
3. **Verify Continuous Monitoring:** Review the `/metrics/queue_and_incident_metrics.csv` to see live evidence of how our organization tracks compliance gaps, system targets, and corrective action timelines.
