# 🏛 RFC Governance Workflow

This document defines the formal workflow for submitting, reviewing, and approving RFCs.

---

# 1. Roles

### **Author**
Creates the RFC, owns the proposal.

### **Tech Lead / Application Owner**
Final decision-maker.  
Ensures solution is technically appropriate.

### **SRE Reviewer**
Ensures:
- Reliability  
- Operational safety  
- Observability compliance  

### **Architecture Reviewer**
Ensures:
- Long-term maintainability  
- Standards alignment  
- Scalability and future-proofing  

### **Director / MD**
- Ensures business alignment  
- Provides directional input  
- Does **not** choose frameworks or low-level implementation details  

---

# 2. Approval Requirements

Approval varies by impact:

| Impact | Required Approvals |
|--------|---------------------|
| Local code-level change | Tech Lead |
| Application-level architecture change | Tech Lead + SRE |
| Platform or infra-level change | Tech Lead + SRE + Architecture |
| Cross-team or strategic change | Tech Lead + Architecture + Director |

---

# 3. Workflow Steps

### **Step 1 — Create RFC**
Author creates an RFC using GitHub template.

### **Step 2 — Assign Reviewers**
- Tech Lead  
- Relevant SRE  
- Architecture  
- (Optional) Security  

### **Step 3 — Discussion**
Async comments, sync review meetings if necessary.

### **Step 4 — Revisions**
Author updates RFC until reviewers are satisfied.

### **Step 5 — Approval**
Reviewers comment:  

### **Step 6 — Final Decision**
Tech Lead marks RFC as:
- **Approved**
- **Rejected**
- **Superseded**

### **Step 7 — Merge**
Move RFC to `/docs/rfc/RFC-xxxx-title.md` for permanent record.

### **Step 8 — Implementation**
Subsequent issues/PRs must reference the RFC ID.

---

# 4. Decision Principles

All decisions must consider:

- Reliability impact  
- Operational load  
- Long-term maintenance  
- Security and compliance  
- Cost efficiency  
- Developer productivity  
- Alignment with architectural strategy  

---

# 5. When RFCs Are NOT Required

- Cosmetic code refactors  
- Documentation updates  
- Bug fixes  
- Non-breaking config changes  
- Updates that affect only a single developer and do not impact others  

---

# 6. Superseding an RFC

When a new RFC replaces an old one:
- Link to the old RFC  
- Mark old RFC as **Superseded**  
- Explain rationale for the change  

---

# 7. Escalation Path

If reviewers cannot agree:

1. Tech Lead resolves the decision  
2. If still blocked → escalate to Architecture Lead  
3. If still unresolved → Director/MD decides based on business priorities  

