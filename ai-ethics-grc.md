# AI Ethics & GRC Compliance Checklist

This governance, risk, and compliance (GRC) framework ensures all organizational artificial intelligence models are deployed safely, ethically, and legally.

## 1. Governance & Oversight
* **Human-in-the-Loop:** Establish a clear protocol where high-risk automated decisions must be reviewed by a qualified team member.
* **Accountability Mapping:** Assign a specific compliance officer or team leader responsible for monitoring the AI model's real-world impact.

## 2. Risk Management & Fairness
* **Bias Auditing:** Scan all historical training data sets for embedded biases before the model training phase begins.
* **Data Privacy Protection:** Verify that all data ingested by the model strictly complies with standard organizational and legal privacy regulations.
* **No PII Exposure:** Ensure no unauthorized personally identifiable information (PII) is accessible or exposed by the system.

## 3. Compliance & Transparency
* **Audit Trails:** Maintain automated logs detailing how the AI model reaches its outputs for future regulatory audits.
* **User Appeal Process:** Provide a transparent, accessible mechanism for users or clients to appeal an automated system decision.
## 5. High-Risk Sector Compliance Standard Operating Procedures (SOPs)

### Control 5.1: Financial Sector Credit & Lending Bias Defenses
AI systems used for credit underwriting, mortgage approvals, or interest-rate calculations face strict liability under the Equal Credit Opportunity Act (ECOA).
*   **Proxy Variable Scrubbing:** The system must actively scrub "proxy variables." Even if a model does not explicitly look at race or gender, it cannot use variables that closely correlate with them (e.g., zip codes, historical neighborhood data, or certain shopping habits).
*   **Adverse Action Transparency:** If a financial LLM or model denies a loan application, it must generate a human-readable "Adverse Action Notice" detailing the exact top three financial reasons for the denial (e.g., debt-to-income ratio). A vague algorithmic score is legally unacceptable.

### Control 5.2: Healthcare Diagnostic & Resource Allocation Defenses
AI models used to prioritize patient care, predict health risks, or allocate hospital resources must prevent systemic health disparities.
*   **Clinical Metric Normalization:** Models must not use financial cost metrics as a proxy for health needs. (Historically, routing more resources to patients who spend more money on healthcare inadvertently discriminates against lower-income demographics).
*   **Demographic Performance Parity:** The model's diagnostic accuracy (False Positive and False Negative rates) must be statistically equal across all age, race, and gender cohorts. If a diagnostic tool is 95% accurate for one group but only 60% accurate for another, it must be pulled from clinical use immediately.
