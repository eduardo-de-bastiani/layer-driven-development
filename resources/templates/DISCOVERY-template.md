# Discovery — [Topic / Investigation Title]

**Topic:** [e.g., LLM Extraction Benchmark / Market Evaluation / API Protocol Comparison]  
**Date:** [YYYY-MM-DD]  
**Related Layer:** Layer {N} — [Layer Title]  
**Status:** Complete  

---

## 1. 🎯 Purpose & Scope

[Explain what question or unknown this discovery document investigates. Why was research or benchmarking needed? What decisions will this inform?]

---

## 2. 🧪 Methodology & Setup

Describe how the investigation or benchmark was conducted:

- **Tools / Models Tested:** [e.g., Gemini 2.5 Flash, GPT-4o, Claude 3.5 Sonnet]
- **Sample Dataset / Workload:** [e.g., 50 anonymized medical lab report PDFs]
- **Evaluation Metrics:** [e.g., Extraction accuracy %, token cost, latency (ms), schema adherence]

---

## 3. 📊 Findings & Comparative Analysis

| Subject / Option | Metric 1 (e.g., Accuracy) | Metric 2 (e.g., Latency) | Metric 3 (e.g., Cost / 1k reqs) | Key Trade-off |
| :--- | :--- | :--- | :--- | :--- |
| **Option A** | [Result] | [Result] | [Result] | [Trade-off description] |
| **Option B** | [Result] | [Result] | [Result] | [Trade-off description] |
| **Option C** | [Result] | [Result] | [Result] | [Trade-off description] |

### Qualitative Observations
- [Observation 1 regarding developer experience, API reliability, or prompt sensitivity]
- [Observation 2]

---

## 4. 💡 Synthesis & Architectural Recommendations

Based on the empirical findings:

1. **Recommended Path:** [Clear statement of recommended technical or product direction]
2. **Impact on Layer Scope:** [How this impacts current or future layer steps]
3. **Trigger for ADR:** [Does this require a formal ADR in `docs/adr/`? If yes, specify]

---

## 5. 🔗 References & Primary Sources

- [Source 1 / Official Documentation link]
- [Source 2 / Academic Paper or Guideline link]
- Related Layer Backlog: [`docs/layers/l{N}-<name>.md`](../layers/l{N}-<name>.md)
