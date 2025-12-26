# 🔧 Addendum: Architecture & Use-Case Customization  
## Automated Newsletter & Stock Sentiment Analysis (DSSA)

---

## A. Target Architecture Diagrams

> **Note:** Diagrams are written in **Mermaid** and can be rendered in Notion, GitHub, Obsidian, or any Markdown-compatible viewer that supports Mermaid.

---

## A.1 High-Level System Architecture

```mermaid
flowchart LR
    NewsAPI[News & Media APIs]
    MarketAPI[Market Data APIs]
    Comments[User Comments<br/>(Stockbit, Forums)]
    
    n8n[n8n Workflow Orchestrator]
    
    Proc[Processing Services<br/>(FastAPI)]
    RAG[RAG & AI Services]
    Sentiment[Sentiment Analysis Service]
    
    DB[(Supabase / PostgreSQL)]
    VectorDB[(Vector Database)]
    
    Email[Email Delivery]
    WA[WhatsApp Delivery]
    Dashboard[Management Dashboard]

    NewsAPI --> n8n
    MarketAPI --> n8n
    Comments --> n8n

    n8n --> Proc
    Proc --> RAG
    Proc --> Sentiment

    RAG --> VectorDB
    Proc --> DB
    Sentiment --> DB

    DB --> Dashboard
    Proc --> Email
    Proc --> WA
