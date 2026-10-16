# Layer {N} — [Layer Title]

**Layer Status:** Active (In Progress)  
**Parent Roadmap:** [`ROADMAP.md`](../../ROADMAP.md)  
**Domain Glossary:** [`CONTEXT.md`](../../CONTEXT.md)  

---

## 1. 🎯 Objective & Context

[Provide a concise 2-3 paragraph description explaining what this layer accomplishes, why it exists now, and how it advances the project toward its target state.]

---

## 2. 📥 Input Requirements & Prerequisites

Before starting execution, verify that the following inputs, dependencies, and upstream artifacts are available:

- [ ] Upstream Layer results evaluated and documented in `docs/results/l{N-1}-results.md`
- [ ] Required external APIs, credentials, or third-party datasets accessible
- [ ] Architectural guidelines understood and referenced in `docs/adr/`

---

## 3. 🚀 Sequential Execution Backlog

> [!TIP]
> Execute sequentially from Step 1 to Step N. Each step contains concrete, testable tasks. When a task is completed, mark its checkbox as `[x]`.

### Step 1: [Step Title — e.g., Data Models & Schema Setup]
- [ ] **Task 1.1:** [Concrete task description, e.g., Define canonical database entities in schema]
- [ ] **Task 1.2:** [Implement data validation rules and domain constraints]
- [ ] **Task 1.3:** [Add unit tests covering valid and boundary cases]

### Step 2: [Step Title — e.g., Core Logic & Business Rules Pipeline]
- [ ] **Task 2.1:** [Implement service layer executing business rules defined in `docs/business-rules/`]
- [ ] **Task 2.2:** [Handle error conditions, edge cases, and unexpected inputs]
- [ ] **Task 2.3:** [Validate test seams using automated integration tests]

### Step 3: [Step Title — e.g., Verification & Seam Review]
- [ ] **Task 3.1:** [Run end-to-step verification suite and linters]
- [ ] **Task 3.2:** [Check if any domain terms need to be added to `CONTEXT.md`]
- [ ] **Task 3.3:** [Confirm all exit criteria are satisfied]

---

## 4. 🏁 Measurable Exit Criteria

This layer is strictly considered ready for closing when:

1. [ ] **Functional Criterion:** [e.g., Core pipeline processes all sample datasets without unhandled exceptions]
2. [ ] **Quality Criterion:** [e.g., Test suite passes with 100% green status on defined seams]
3. [ ] **Documentation Criterion:** [e.g., All non-obvious technical trade-offs recorded as ADRs in `docs/adr/`]

---

## 5. 🛑 Guardrails: What NOT To Do in This Layer

To prevent scope creep and maintain velocity, the following are explicitly **OUT OF SCOPE**:

- ❌ **Do NOT** [e.g., Build premature frontend interfaces before backend logic is verified]
- ❌ **Do NOT** [e.g., Introduce heavy cloud infrastructure before local prototype works]
- ❌ **Do NOT** [e.g., Optimize for premature scale before baseline functionality is proven]
