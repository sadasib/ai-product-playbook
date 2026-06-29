# AI Risk Register Template

## Purpose

AI systems introduce risks that extend beyond traditional software, including hallucinations, policy violations, unsafe outputs, model drift, and customer trust concerns.

This register helps teams identify, assess, assign ownership, and monitor AI-specific risks throughout the product lifecycle.

---

# Risk Assessment Scale

| Severity | Definition                                             |
| -------- | ------------------------------------------------------ |
| Low      | Minimal customer or business impact                    |
| Medium   | Noticeable impact requiring mitigation                 |
| High     | Significant customer, operational, or financial impact |
| Critical | Immediate blocker to launch                            |

---

# Risk Register

| ID    | Risk                              | Category   | Severity | Likelihood | Owner    | Mitigation                               | Status |
| ----- | --------------------------------- | ---------- | -------- | ---------- | -------- | ---------------------------------------- | ------ |
| R-001 | Hallucinated responses            | AI Quality | High     | Medium     | AI PM    | Human evaluation, grounding improvements | Open   |
| R-002 | Incorrect policy guidance         | Compliance | High     | Medium     | Product  | Policy validation and automated testing  | Open   |
| R-003 | Prompt injection attacks          | Security   | Critical | Low        | Security | Prompt hardening and input validation    | Open   |
| R-004 | Exposure of sensitive information | Privacy    | Critical | Low        | Security | PII filtering and access controls        | Open   |
| R-005 | Poor escalation decisions         | Operations | High     | Medium     | Product  | Escalation evaluation and monitoring     | Open   |

---

# Risk Categories

## AI Quality

Examples:

* Hallucinations
* Low accuracy
* Missing context
* Inconsistent responses

---

## Responsible AI

Examples:

* Harmful content
* Bias
* Fairness issues
* Lack of transparency

---

## Privacy & Security

Examples:

* PII exposure
* Prompt injection
* Data leakage
* Unauthorized access

---

## Operational

Examples:

* Monitoring gaps
* Missing alerts
* Failed rollback
* Support readiness

---

## Business

Examples:

* Low adoption
* High operational cost
* Poor customer satisfaction
* Limited ROI

---

# Mitigation Planning

For every High or Critical risk, document:

* Root cause
* Mitigation strategy
* Risk owner
* Target completion date
* Residual risk after mitigation

---

# Review Cadence

| Phase               | Frequency           |
| ------------------- | ------------------- |
| Development         | Weekly              |
| Beta                | Twice per week      |
| Production          | Monthly             |
| Major model updates | Before each release |

---

# Launch Rule

A launch should not proceed while any Critical risk remains open unless an executive exception has been formally approved and documented.
