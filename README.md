# Agentic AI Portfolio

Project writeups from the **Johns Hopkins University Agentic AI** program (2026). These describe systems I designed and built during the program — architecture, approach, and key learnings.

> **Note:** This repository contains descriptions and architectural writeups only. The implementation code is not published, as the program used non-distributable course materials. The designs and learnings below are my own.

🔗 **Verified portfolio:** [mygreatlearning.com/eportfolio/banketeshvar-narayan](https://www.mygreatlearning.com/eportfolio/banketeshvar-narayan)

---

## 1. Multi-Agent Mortgage Underwriting System

An AI-driven underwriting system using a **hierarchical multi-agent architecture** to accelerate and standardize loan decisions.

- **Architecture:** A Supervisor Agent coordinating four specialist agents — Credit Analyst, Income Analyst, Property Analyst, and Compliance Officer — each following the ReAct (Reasoning + Acting) pattern.
- **Capabilities:** RAG-based policy retrieval for compliance checking, PII redaction, bias detection, audit trails, and Human-in-the-Loop review for edge cases.
- **Stack:** LangGraph, RAG, ChromaDB, Multi-Agent Systems, HITL.
- **Key learning:** How state machines manage complex shared state across multiple agents, and how to translate a business process that traditionally takes 3–5 days into a consistent, auditable, automated agentic workflow.

## 2. Autonomous Financial Research Analyst

A smart financial agent that analyzes AI companies for investors — pulling real-time stock prices, checking multi-year performance trends, scanning news for sentiment, and mining analyst reports via RAG to produce sourced Buy/Hold/Sell recommendations.

- **Architecture:** A LangGraph state machine with an Agent Node, Tool Node, and conditional routing that autonomously orchestrates four tools without explicit step-by-step user instruction.
- **Stack:** LangGraph, LangChain, tool calling, sentiment analysis, prompt engineering.
- **Key learning:** The four core agent design principles — proactiveness, autonomy, reactivity, and actuators — and how behavioral constraints and goal definitions shape agent reliability. This shifted my thinking from "prompting an LLM" to "designing an agent with a charter."

## 3. DualLens Analytics — RAG Evaluation Pipeline

A RAG system that integrates quantitative financial data with qualitative insights from organizations' AI initiatives, giving investors a combined performance-and-readiness view.

- **Architecture:** End-to-end pipeline — real-time data ingestion, PDF chunking, embeddings stored in ChromaDB, and synthesis into investment recommendations, with quality measured via LLM-as-Judge (groundedness and relevance).
- **Stack:** RAG, ChromaDB, embeddings, OpenAI, evaluation metrics.
- **Key learning:** How multi-source data integration produces richer, more defensible decisions than any single source, and how to evaluate RAG quality systematically rather than by intuition.

---

*These projects reflect hands-on work in agentic system design, multi-agent orchestration, and RAG — the same principles I apply to AI-enabled engineering at enterprise scale.*
