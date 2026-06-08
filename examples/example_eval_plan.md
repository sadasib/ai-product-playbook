# Example Evaluation Plan: Retail Returns Assistant

## 1. Feature Overview

### Feature Name

Retail Returns Assistant

### Description

An AI-powered customer support assistant that helps customers understand return eligibility, return windows, refund timelines, and return methods using retailer return policies and order information.

The assistant is designed to reduce customer support contacts while improving customer satisfaction and self-service resolution rates.

---

## 2. Evaluation Objectives

This evaluation supports the following product decisions:

* Determine launch readiness
* Measure customer-facing answer quality
* Assess policy compliance
* Identify hallucination risks
* Validate escalation behavior
* Compare prompt and workflow variations

---

## 3. Success Criteria

| Dimension                | Target      |
| ------------------------ | ----------- |
| Policy Accuracy          | > 95%       |
| Grounding Accuracy       | > 98%       |
| Escalation Accuracy      | > 90%       |
| Safety Compliance        | 100%        |
| Average Response Time    | < 3 seconds |
| Customer Resolution Rate | > 80%       |

---

## 4. Golden Dataset

### Dataset Size

500 synthetic customer return scenarios

### Dataset Sources

* Synthetic order histories
* Synthetic return policies
* Synthetic customer questions
* Edge-case scenarios

### Coverage Areas

* Eligible returns
* Non-returnable products
* Expired return windows
* Damaged products
* Missing receipts
* Marketplace items
* Gift returns

### Edge Cases

* Conflicting customer information
* Ambiguous policy wording
* Multiple orders in same conversation
* Fraud-related scenarios

---

## 5. Human Evaluation

### Reviewers

* Product Manager
* Customer Support SME
* Operations Lead

### Scoring Scale

1 = Poor

2 = Needs Improvement

3 = Acceptable

4 = Good

5 = Excellent

### Evaluation Dimensions

* Correctness
* Completeness
* Trustworthiness
* Clarity
* Customer Friendliness

### Pass Criteria

Average score ≥ 4.0

No critical policy failures.

---

## 6. Automated Evaluation

### Metrics

* Policy Match Rate
* Grounding Accuracy
* Hallucination Rate
* Escalation Accuracy
* Citation Accuracy
* Response Latency

### Evaluation Frequency

* Daily during testing
* Weekly after launch

---

## 7. Failure Taxonomy

### Hallucinations

Assistant invents return policies or eligibility rules.

### Policy Violations

Assistant approves returns that violate policy.

### Incorrect Escalation

Assistant fails to escalate complex or sensitive situations.

### Missing Context

Assistant ignores relevant order information.

### Customer Frustration

Assistant provides technically correct but unhelpful responses.

---

## 8. Red Team Testing

### Scenarios

* Requests to bypass return policies
* Fraud attempts
* Ambiguous product information
* Missing order numbers
* Escalation avoidance prompts

### Success Criteria

No critical policy violations.

No unsafe recommendations.

---

## 9. Launch Thresholds

| Metric                   | Threshold |
| ------------------------ | --------- |
| Critical Safety Failures | 0         |
| Hallucination Rate       | < 2%      |
| Policy Compliance        | > 95%     |
| Escalation Accuracy      | > 90%     |
| Human Review Pass Rate   | > 95%     |

---

## 10. Post-Launch Monitoring

### Metrics Tracked

* Customer Satisfaction (CSAT)
* Return Resolution Rate
* Escalation Rate
* Hallucination Reports
* Average Handling Time
* Cost per Resolution

### Monitoring Cadence

* Daily dashboards
* Weekly quality reviews
* Monthly launch health assessment

---

## Recommendation

Proceed to limited beta launch if all launch thresholds are achieved and no critical safety or policy issues are identified during red-team testing.
