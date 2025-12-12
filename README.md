# 📘 RFC Process — Engineering & Architecture Decision Framework

This repository uses a lightweight, GitHub-based RFC (Request for Comments) process to propose, review, and approve significant engineering or architectural decisions.

The goal is to ensure:
- Consistent and transparent technical decision-making  
- Alignment across teams  
- Clear documentation of trade-offs, rationale, and outcomes  
- Strong engineering governance for long-term maintainability  
- Efficient collaboration between Engineering, SRE, Architecture, and Leadership  

---

# 🧭 When Should You Create an RFC?

Create an RFC when proposing changes that affect:

### **Architecture**
- Framework selection  
- Major refactors  
- Introduction of new services  
- Changes in communication patterns (REST → gRPC, etc.)  
- Data model redesigns  

### **Infrastructure / Platform**
- Kubernetes changes  
- New CI/CD workflow  
- Observability tooling  
- Cloud architecture changes  
- Service discovery & networking patterns  

### **Standards / Practices**
- New coding standards  
- API conventions  
- Logging or tracing standards  
- Security and compliance posture  

### **Anything With Long-Term Impact**
If a change will be around for 3+ months, it needs an RFC.

---

# 📝 RFC Types

### **1. Full RFC**
Used for major decisions involving:
- Architectural redesign  
- New frameworks or infrastructure  
- Multi-team impact  
- Significant operational changes  

> Use `.github/ISSUE_TEMPLATE/rfc.md`

### **2. RFC-Lite**
Used for:
- Localized changes  
- Small design decisions  
- Minor tools or library selections  
- Low-risk, low-impact items  

> Use `.github/ISSUE_TEMPLATE/rfc-lite.md`

---

# 🔄 RFC Life Cycle

1. **Draft**  
   - Author creates RFC issue using GitHub template.  
   - RFC is assigned reviewers.

2. **Discussion**  
   - Inline comments, design review meetings, async feedback.  

3. **Revision**  
   - Changes incorporated based on feedback.  

4. **Approval**  
   - Required approvers comment: `Approved`  
   - At minimum:  
     - Application Owner / Tech Lead  
     - SRE reviewer (if operational impact)  
     - Architecture Lead (if platform impact)  

5. **Final Decision**  
   - Mark RFC as **Approved** or **Rejected**  
   - Merge into `/docs/rfc/` directory as a permanent record.

6. **Implementation**  
   - A follow-up issue or PR links back to the RFC.

7. **Superseded / Deprecated (Optional)**  
   - Older RFCs may be superseded by newer ones.

---

# 🏛 Governance Model

### **Decision Owner**
- The **Application Owner / Tech Lead** has final decision-making authority.  
- Directors/MDs provide oversight but do not select technologies.  

### **Reviewers**
- SRE: operational risk, reliability, deployability  
- Architecture: alignment with standards, long-term viability  
- Security: if sensitive data or authentication flows change  

### **Approvals Required**
- 1 Tech Lead / Application Owner  
- 1 SRE Reviewer (if relevant)  
- 1 Architecture Reviewer (if relevant)

Techology Leadership may request changes or escalate concerns but does not approve day-to-day engineering decisions.

# 🧩 Benefits of GitHub-Based RFCs

- Version-controlled  
- Transparent and auditable  
- Easy for async reviews  
- Links directly to PRs and code  
- Avoids Confluence sprawl  
- Encourages high-quality technical decision-making  

---

# 🙋 Need Help?

For guidance or questions, tag:
- `@application-owner`
- `@sre-team`
- `@architecture-review`

Or check existing RFCs under `/docs/rfc/`.

