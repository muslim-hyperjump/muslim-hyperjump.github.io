# System Architecture — DSS Automated Newsletter

## 1) High-Level Overview
This system processes curated article sources into structured
newsletter components through an automated pipeline consisting of:

- ingestion
- classification
- summarization
- formatting
- delivery

---

## 2) Architecture Diagram
(Describe or link draw.io / excalidraw)

Components include:
- Source ingestion layer
- Storage (Supabase / DB)
- LLM summarization engine
- Formatting + output renderer
- Distribution workflow (n8n)

---

## 3) Data Flow
1) Article collected
2) Metadata normalized
3) Company / sector relevance detection
4) LLM structured summary generation
5) Duplicate detection
6) Output stored
7) Channel-formatted rendering

---

## 4) LLM Prompting Strategy
- company-scoped summarization
- structured JSON response enforcement
- key takeaway formatting rules
- collapse-safe rendering for WhatsApp

---

## 5) Operational Considerations
- retry strategy
- failure logs
- output validation
- manual override option

---

## 6) Known Issues & Risks
- occasional markdown collapse cases
- inconsistent bullet rendering
- multilingual sentence mixing

Mitigations documented in runbook.
