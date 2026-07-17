SYSTEM ARCHITECTURE
Frontend UI: Custom single-page luxury hospitality landing page built with HTML5, CSS3 (Glassmorphism design patterns), and integrated with premium typography (Playfair Display & Inter), hosted on Vercel.

Orchestration & Logic: Dual-workflow automation engine powered by n8n, routing conversational states to independent functional tools.

Database Layer: Supabase (PostgreSQL) handling dynamic relational structures for bookings and support tickets with secure Row-Level Security (RLS) configurations.

Knowledge Retrieval: Semantic vector database retrieval for context-aware customer service and zero-hallucination policy enforcement.

CORE ENGINEERING HIGHLIGHTS
Stateful Context Extraction: The AI model dynamically parses unformatted user text (e.g., "from the 20th to the 29th of July") and translates it into standardized ISO dates (YYYY-MM-DD) and valid schema inputs for database ingestion.

Deterministic Fallbacks: Engineered custom database microservices that act as strict transactional guardrails, preventing the LLM from making up fake reservation logs.

Automated Escalation Matrix: Includes a human-in-the-loop support ticketing system that catches guest complaints and automatically logs open service requests directly into the centralized database backend.
