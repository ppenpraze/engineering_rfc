# RFC — Migration from Monolithic Architecture to Microservices

**Title:** RFC-0001 — Migration from Monolith to Microservices  
**Author:** Netflix Platform Engineering  
**Reviewers:** SRE, Cloud Platform, Executive Engineering Leadership  
**Date:** 2009-06-01  
**Status:** Approved  

---

## 1. Purpose
This RFC proposes migrating Netflix’s core application from a single monolithic architecture to a distributed microservices-based architecture to improve scalability, availability, and development velocity.

---

## 2. Background & Problem Statement
Netflix’s existing monolithic application architecture had become a bottleneck as the company scaled rapidly. Key issues included:

- Tight coupling between components  
- Full application outages due to partial failures  
- Slow deployment cycles  
- Limited horizontal scalability  
- Increasing operational risk during peak traffic  

As Netflix transitioned from DVD rentals to streaming, these limitations posed an existential risk to the business.

---

## 3. Goals & Non-Goals

### Goals
- Improve system availability and fault isolation  
- Enable independent service scaling  
- Increase deployment velocity  
- Reduce blast radius of failures  
- Support global traffic growth  

### Non-Goals
- Immediate rewrite of all services  
- Elimination of all legacy systems  
- Changing customer-facing functionality  

---

## 4. Requirements

### Functional Requirements
- Independent service ownership  
- Service-to-service communication  
- Stateless request handling  

### Non-Functional Requirements
- High availability  
- Horizontal scalability  
- Strong observability  
- Resilience to partial failures  
- Cloud-native deployment support  

---

## 5. Options Considered

### Option A — Remain Monolithic
Pros:
- Simpler architecture  
- Lower short-term engineering cost  

Cons:
- Scaling limitations  
- High blast radius  
- Slow development cycles  

### Option B — Microservices Architecture (Proposed)
Pros:
- Fault isolation  
- Independent scaling  
- Faster deployments  
- Improved team autonomy  

Cons:
- Increased operational complexity  
- Network reliability challenges  

---

## 6. Comparative Evaluation Matrix

| Criteria | Monolith | Microservices |
|--------|----------|---------------|
| Availability | Low | High |
| Scalability | Limited | High |
| Deployment Velocity | Slow | Fast |
| Fault Isolation | Poor | Strong |
| Operational Complexity | Low | High |
| Long-Term Viability | Low | High |

---

## 7. Detailed Analysis

### 7.1 Architecture Overview
Each functional domain (recommendations, billing, streaming metadata) will be split into independently deployable services communicating over APIs.

### 7.2 Operational Considerations
- Introduce centralized monitoring  
- Build resilience tooling (later became Chaos Engineering)  
- Implement circuit breakers and retries  

---

## 8. Risks & Mitigations

### Risks
- Increased operational complexity  
- Network failures  
- Distributed debugging challenges  

### Mitigations
- Strong SRE practices  
- Chaos testing (Chaos Monkey)  
- Investment in observability  

---

## 9. Migration / Implementation Plan
- Gradual service extraction  
- Parallel running of monolith and services  
- Incremental traffic shifting  

---

## 10. Recommendation
Adopt a microservices architecture to ensure Netflix can scale reliably and innovate rapidly.

---

## 11. Appendix
- Netflix Tech Blog: “Adopting Microservices at Netflix”
