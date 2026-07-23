# GRC & Security Audits Portfolio

A connected body of governance, risk, and compliance work built around a
single realistic (fictional) scenario — **CloudHealth Canarias S.L.**, an
80-employee healthcare company operating two clinics in Tenerife. Rather
than isolated one-off exercises, each piece builds on the same
organization, the same asset inventory, and the same risk profile —
mirroring how GRC work actually accumulates in a real role.

*Note: source documents are in Spanish (matching the original coursework
language); English translations planned.*

## Scenario: CloudHealth Canarias S.L.

A healthcare provider handling special-category health data (RGPD),
recovering from a ransomware incident 6 months prior, with known gaps in
identity management, vendor oversight, and staff security training.

## Contents

### 1. [Security Documentation Framework](./cloudhealth-canarias-framework.pdf)
Full security policy and governance framework: critical asset inventory,
threat and vulnerability analysis, applicable legal/regulatory
requirements (RGPD, LOPDGDD, ENS, ISO 27001, NIS2), a general security
policy, 5 risk-prioritized specific policies, an operational
onboarding/offboarding procedure, and a clinical staff work instruction
for handling patient records.

### 2. [TPRM Vendor Risk Assessment](./TPRM_Vendor_Risk_Assessment.pdf)
A complete third-party risk assessment for **TecnoSoluciones IT S.L.**,
CloudHealth's external IT managed services provider — a vendor with full
administrative/privileged access to all systems, including patient
health records, user accounts, and infrastructure.

**Key findings:**

| Metric | Result |
|---|---|
| Inherent Risk | **CRITICAL** (23/25) |
| Residual Risk | **HIGH** (11/30) |
| Recommendation | **MITIGATE** — update contract, require MFA, deploy monitoring |

**Direct connection:** builds on **Policy #4 (Vendor Management)** from
the Security Documentation Framework, providing the detailed risk
analysis that policy called for but didn't itself contain.

### 3. [Internal Audit Simulation](./Internal_Audit_Simulation.pdf)
A control-testing audit of 10 controls sampled across all 5 policies in
the Security Documentation Framework — each evaluated with a test
procedure, requested evidence, and a documented finding, not just a
pass/fail opinion.

**Key findings:**

| Metric | Result |
|---|---|
| Compliance Score | **9/20 (45%)** — overall rating: Insufficient |
| Conforme | 3 of 10 controls |
| Parcialmente Conforme | 3 of 10 controls |
| No Conforme | 4 of 10 controls |

**Direct connection:** 2 of the 4 failed controls tie back to earlier
findings — personal USB use (originally flagged as a HIGH vulnerability
in the framework's risk analysis) and the missing vendor security SLA
(already identified in the TPRM assessment above) — showing that
documenting a policy isn't the same as enforcing it.

### 4. Security Incident Management Plan
*(see below)*

A 7-phase incident response lifecycle (Preparation → Detection →
Analysis → Containment → Eradication/Recovery → Investigation →
Post-Incident Review), aligned with industry-standard frameworks like
NIST SP 800-61.

---

## Security Incident Management Plan

1. **Preparation & Prevention** — establish policies, tooling, and staff
   training *before* an incident occurs, so response isn't improvised
   under pressure.
2. **Detection & Notification** — identify the incident and escalate to
   the appropriate responders promptly.
3. **Preliminary Analysis** — classify and prioritize the incident,
   assess its scope and severity.
4. **Containment** — take action to prevent further spread or damage.
5. **Eradication & Recovery** — remove the root cause and restore
   affected systems to normal operation.
6. **Investigation** — forensic analysis to determine what happened and,
   where relevant, who was responsible.
7. **Post-Incident Activities** — document lessons learned, update
   policies based on findings, and produce a final incident report.

---

## Coming next in this scenario
- **NIST CSF 2.0 Maturity Mapping** — assessing CloudHealth's current
  controls against the 6 CSF functions (Govern, Identify, Protect,
  Detect, Respond, Recover), extending the framework already applied in
  the vendor risk assessment
- **Risk Register with Heat Map** — a structured 5×5 likelihood/impact
  risk register formalizing the risks identified across the framework,
  the vendor assessment, and the internal audit above

## Skills demonstrated
- ISO/IEC 27001-aligned security framework design
- RGPD/LOPDGDD/ENS/NIS2 regulatory mapping
- Third-party/vendor risk assessment (TPRM) methodology
- Inherent vs. residual risk scoring, risk treatment decision-making
- NIST CSF 2.0 function-based control evaluation
- Internal audit control testing: test procedures, evidence evaluation,
  findings documentation
- Risk-based policy prioritization and remediation roadmapping
- Operational procedure design (identity lifecycle management)
- Incident response lifecycle planning
