---
name: "📘 RFC — Engineering & Architecture Decision Proposal"
about: "Use this template to propose architectural decisions, framework choices, infrastructure changes, or major engineering implementations."
title: "RFC: <Concise Title>"
labels: ["rfc", "architecture", "proposal"]
assignees: ""
---

# 📘 RFC — Engineering & Architecture Decision Proposal

**Title:** <Concise RFC Title>  
**Author:** <Name / Team>  
**Reviewers:** <Architecture Leads / SRE / Directors / MDs>  
**Date:** <YYYY-MM-DD>  
**Status:** Draft / In Review / Approved / Rejected / Superseded  

---

## 1. Purpose
A short summary describing:
- What decision is being proposed  
- What problem or opportunity it addresses  
- Expected outcome of the decision  

> _Example:_ This RFC proposes adopting <Technology/Architecture> to improve <performance/reliability/maintainability> for <system/team>.

---

## 2. Background & Problem Statement
Provide context:
- Why this RFC exists  
- Current limitations, pain points, failures, or risks  
- Why this problem is worth solving now  

---

## 3. Goals & Non-Goals

### 🎯 Goals
What this RFC intends to achieve.

-  
-  
-  

### 🚫 Non-Goals
What is *not* in scope for this RFC.

-  
-  
-  

---

## 4. Requirements

### Functional Requirements
-  
-  
-  

### Non-Functional Requirements
- Performance  
- Scalability  
- Reliability (SLIs/SLOs)  
- Security  
- Compliance  
- Observability  
- Maintainability  
- Cost boundaries  

---

## 5. Options Considered

### Option A — <Option Name> (Proposed / Preferred)
Description:  
Pros:  
Cons:  

### Option B — <Alternative Option>  
Description:  
Pros:  
Cons:  

### Option C — <Alternative Option>  
Description:  
Pros:  
Cons:  

---

## 6. Comparative Evaluation Matrix

| Criteria | Option A | Option B | Option C |
|---------|----------|----------|----------|
| Reliability / SLO Alignment | | | |
| Performance / Latency | | | |
| Scalability | | | |
| Operational Complexity | | | |
| Cost | | | |
| Security / Compliance | | | |
| Developer Productivity | | | |
| Maintainability / Support | | | |
| Vendor Lock-In Risk | | | |
| Alignment With Existing Standards | | | |
| Long-Term Viability | | | |

---

## 7. Detailed Analysis

### 7.1 Architecture Overview
Provide diagrams or high-level design details.  
(You may embed Mermaid diagrams or attach images.)

### 7.2 Operational Considerations
- Deployment model  
- Rollback strategy  
- Scaling  
- Failure modes  
- Disaster recovery  
- Observability (logs, metrics, traces)  

### 7.3 Security Considerations
- Authentication  
- Authorization  
- Encryption  
- Secret management  

### 7.4 Performance Considerations
- Throughput expectations  
- Latency patterns  
- Benchmarks (if available)  

### 7.5 Team Impact
- Training or upskilling  
- Ownership  
- Support burden  

---

## 8. Risks & Mitigations

### Risks
-  
-  
-  

### Mitigations
-  
-  
-  

---

## 9. Migration / Implementation Plan
Describe how the chosen solution would be introduced.

- Milestones  
- Rollout phases  
- Dependencies  
- Testing approach  
- Backward/forward compatibility  
- Rollback procedures  

---

## 10. Cost Analysis (If Applicable)
- Licensing  
- Cloud compute/storage/network cost  
- Maintenance cost  
- Opportunity cost  

---

## 11. Recommendation
State which option you recommend and why.

> _Example:_ Option A is recommended due to reliability, maintainability, and alignment with architectural principles.

---

## 12. Open Questions
List anything requiring further investigation or executive input.

-  
-  
-  

---

## 13. Appendix (Optional)
You may include:
- Benchmark results  
- Prototype findings  
- Additional diagrams  
- References  
- Glossary of terms  
