# Deep Patel

Python backend engineer. I build production RAG systems with FastAPI, LangChain, and PostgreSQL.

2.5 years shipping LLM-powered features at Blockspark — multi-agent chatbots, semantic search, document Q&A. Currently open to **remote Python backend / GenAI engineering roles**.

📬 **[your.email@example.com](mailto:your.email@example.com)** · [LinkedIn](https://www.linkedin.com/in/deeppatel2/) · [GitHub](https://github.com/PatelDeep223)

---

## What I'm good at

Designing FastAPI services that hold up under real traffic. RAG pipelines where the retrieval actually works — not just cosine similarity and hope. Wiring caching, query rewriting, and evaluation harnesses around LLMs so they ship as products instead of demos. The boring infrastructure underneath all of it: Postgres schema design, async Python, Docker, observability.

**Stack:** Python · FastAPI · LangChain · LangGraph · PostgreSQL · Redis · FAISS · Docker · AWS

---

## Featured project

### FinBot — Financial Document Q&A

**[Live demo](https://YOUR-DEMO-URL.com)** · **[Source](https://github.com/PatelDeep223/finbot-financial-rag)**

A RAG system for financial documents, where a wrong answer is worse than no answer. I built the architecture around that constraint:

- **Semantic cache** using embedding similarity. Cache hits return in ~50ms vs 2–4s for full retrieval. *(Add real cache hit rate + similarity threshold here.)*
- **Query rewriting** before retrieval. Resolves ambiguous follow-ups ("what about last quarter?") against conversation context, which fixed most of the retrieval failures I was seeing in testing.
- **Citation enforcement + confidence scoring.** Every answer surfaces the source chunks it used. Low-confidence responses are flagged instead of hidden behind fluent prose.
- Async FastAPI, Redis, FAISS, Docker Compose with Nginx in front.

**Stack:** FastAPI · LangChain · OpenAI · FAISS · Redis · PostgreSQL

---

## Other projects

**[Appointment Scheduling Agent](https://github.com/PatelDeep223/appointment-scheduling-agent)**
Medical scheduling agent with RAG-backed FAQ and Calendly integration. Handles booking, rescheduling, and clinic-specific Q&A in a single conversation flow.

**Multi-Agent RAG Chatbot** *(private — Blockspark)*
Support, sales, and billing agents coordinated via LangGraph supervisor. Beyond the standard tutorial pattern: per-agent retrieval indexes, fallback handoff, and shared conversation memory across agents.

**CharConnect** *(private — Blockspark)*
Embeddable chat widget shipped as an npm package. Three-tier response strategy — Dialogflow for known intents, RAG for documented questions, OpenAI fallback for the rest.

**SNG India CRM** *(private — Blockspark)*
Lead management system with SPANCO pipeline and 4-tier RBAC. FastAPI + PostgreSQL + React.

---

## Selected work at Blockspark

Backend engineer, 2.5 years. Some specifics:

- Cut p95 latency on our highest-traffic chatbot endpoint from **~1.2s to ~720ms** by introducing Redis caching for repeated retrieval queries. *(Replace with your real numbers.)*
- Owned the RAG pipeline for [product name] from prototype to production — chunking strategy, embedding model selection, retrieval evaluation, prompt iteration.
- Built and maintained the FastAPI services behind [N internal/external products].

---

## Now

Building [whatever you're actively shipping right now — one line]. Writing about RAG evaluation and production LLM patterns at [your blog if you have one, or remove this section].

---

## Get in touch

The fastest way to reach me is email: **your.email@example.com**

I'm currently open to remote Python backend and GenAI engineering roles. Happy to talk about RAG architecture, evaluation harnesses, semantic caching, or anything else in this stack.
