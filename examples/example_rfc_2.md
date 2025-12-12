# RFC — Standardized Container Orchestration Platform

**Title:** RFC-0042 — Standardized Container Orchestration Platform  
**Author:** Google Infrastructure Engineering  
**Reviewers:** SRE, Platform, Product Infrastructure Leadership  
**Date:** 2014-03-01  
**Status:** Approved  

---

## 1. Purpose
This RFC proposes externalizing and standardizing Google’s internal container orchestration concepts (Borg) into a unified, extensible platform suitable for broad adoption: Kubernetes.

---

## 2. Background & Problem Statement
Google had successfully operated Borg internally for over a decade. However:

- Borg was tightly coupled to Google’s internal systems  
- External teams lacked access to similar orchestration capabilities  
- Industry lacked a standard container orchestration platform  
- Portability across environments was limited  

Google recognized the need for a portable, open orchestration system.

---

## 3. Goals & Non-Goals

### Goals
- Standardize container orchestration  
- Enable portability across environments  
- Reduce vendor lock-in  
- Share operational best practices  

### Non-Goals
- Open-source Borg directly  
- Replace all internal orchestration immediately  

---

## 4. Requirements

### Functional Requirements
- Declarative workload management  
- Service discovery and scheduling  
- Self-healing workloads  

### Non-Functional Requirements
- Scalability to tens of thousands of nodes  
- Strong reliability guarantees  
- Extensibility via APIs  
- Cloud-provider neutrality  

---

## 5. Options Considered

### Option A — Continue with Borg Internally Only
Pros:
- Mature, proven system  

Cons:
- No external adoption  
- Limited ecosystem growth  

### Option B — Create a New Open Platform (Kubernetes)
Pros:
- Industry standardization  
- Community-driven innovation  
- Ecosystem growth  

Cons:
- Engineering investment  
- Governance overhead  

---

## 6. Comparative Evaluation Matrix

| Criteria | Borg | Kubernetes |
|--------|------|------------|
| Portability | Low | High |
| Ecosystem | Closed | Open |
| Extensibility | Limited | High |
| Community Adoption | None | High |
| Long-Term Viability | Internal | Industry-wide |

---

## 7. Detailed Analysis

### 7.1 Architecture Overview
Kubernetes abstracts workloads using Pods, Services, and Controllers, inspired by Borg but redesigned for extensibility and portability.

### 7.2 Operational Considerations
- Control plane redundancy  
- Declarative state reconciliation  
- API-driven automation  

---

## 8. Risks & Mitigations

### Risks
- Fragmentation  
- Community governance challenges  

### Mitigations
- CNCF governance model  
- Strong API contracts  
- Backward compatibility guarantees  

---

## 9. Migration / Implementation Plan
- Gradual external release  
- Internal dogfooding  
- Incremental feature parity with Borg  

---

## 10. Recommendation
Proceed with Kubernetes as an open, extensible container orchestration platform to standardize container operations across the industry.

---

## 11. Appendix
- Google Borg Paper  
- Kubernetes Design Docs  
- CNCF Charter  
