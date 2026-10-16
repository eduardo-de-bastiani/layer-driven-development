# Business Rules — [Domain / Feature Area]

**Domain Area:** [e.g., Clinical Analysis & Risk Stratification / Financial Portfolio Rebalancing]  
**Status:** Active  
**Last Updated:** [YYYY-MM-DD]  
**Related Layer:** Layer {N} — [Layer Title]  

---

## 1. 🎯 Business Intent & Vision

[Explain the business or domain purpose behind these rules. What problem do they solve for end-users, and what guarantees must the system provide?]

---

## 2. 🧩 Domain Entities & Ubiquitous Vocabulary

Define the core domain terms as mapped in [`CONTEXT.md`](../../CONTEXT.md):

- **[Entity 1]:** [Canonical definition and key attributes]
- **[Entity 2]:** [Canonical definition and relationship to Entity 1]

---

## 3. ⚖️ Deterministic Business Rules

Use structured conditional expressions (**WHEN / MUST / THEN**) to specify unambiguous system behavior:

| Rule ID | Trigger / Condition (WHEN) | System Obligation (MUST) | Expected Outcome (THEN) |
| :--- | :--- | :--- | :--- |
| **BR-001** | When [input condition occurs] | The engine MUST [validate or transform] | Output [result state or flag] |
| **BR-002** | When [boundary threshold exceeded] | The system MUST NOT [forbidden action] | Raise [specific domain error or alert] |
| **BR-003** | When [contextual modifier present] | The engine MUST adjust [parameter] | Compute [adjusted target value] |

---

## 4. 🛡️ Invariants & System Guardrails

Non-negotiable constraints that must hold true across all states:

1. **Invariant 1:** [e.g., An unverified external value must never be marked as clinically verified]
2. **Invariant 2:** [e.g., Financial transactions must always balance to zero across double-entry ledgers]
3. **Invariant 3:** [e.g., Sensitive personal data must be pseudonymized before logging or persistence]

---

## 5. ⚠️ Edge Cases & Boundary Conditions

| Scenario | Input Condition | Expected System Behavior |
| :--- | :--- | :--- |
| **Missing Data** | Required field null or empty | Fallback to safe default or reject with actionable error |
| **Extreme Range** | Numerical value outside physiological/realistic limit | Flag as outlier anomaly and request human review |
| **Concurrent Change**| Conflict between local state and upstream API | Apply optimistic concurrency rule with conflict resolution |

---

## 6. 🧪 Traceability to Seams & Verification

- **Automated Tests:** [`tests/rules/`](../../tests/)
- **Target Implementation Seam:** [`src/domain/`](../../src/)
