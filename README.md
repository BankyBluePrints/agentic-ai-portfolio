# Agentic AI Portfolio

Architecture-focused case studies from the **Johns Hopkins University Agentic AI program (2026)**. The portfolio covers multi-agent orchestration, tool-using agents, retrieval-augmented generation (RAG), evaluation, responsible AI, and human oversight.

> **Portfolio scope:** This repository publishes original architectural writeups and learning reflections only. Course implementation code, datasets, prompts, and other non-distributable materials are not included.

## Projects

| Project | Focus | Core technologies and patterns |
| --- | --- | --- |
| [Multi-Agent Mortgage Underwriting System](projects/mortgage-underwriting/) | Coordinated specialist analysis with human review | LangGraph, hierarchical multi-agent workflow, ReAct, RAG, HITL |
| [Autonomous Financial Research Analyst](projects/financial-research-analyst/) | Tool selection and evidence-based financial research | LangGraph, LangChain, tool calling, sentiment analysis |
| [DualLens Analytics](projects/duallens-rag-evaluation/) | Multi-source RAG and systematic response evaluation | ChromaDB, embeddings, RAG, LLM-as-Judge |

## Portfolio themes

- **Orchestration:** model agent responsibilities, shared state, routing, and completion conditions explicitly.
- **Grounding:** use retrieval and external tools to support answers with relevant evidence.
- **Evaluation:** assess groundedness and relevance instead of relying only on subjective inspection.
- **Responsible AI:** include privacy, bias, auditability, and human-review controls in the design.
- **Engineering discipline:** treat failure handling, observability, and validation as part of the architecture.

## Program verification

- [Verified Great Learning e-portfolio](https://www.mygreatlearning.com/eportfolio/banketeshvar-narayan)

## Repository structure

```text
agentic-ai-portfolio/
├── README.md
└── projects/
    ├── mortgage-underwriting/
    ├── financial-research-analyst/
    └── duallens-rag-evaluation/
```

Each case study follows a consistent structure: context, objectives, architecture, workflow, responsible-AI considerations, evaluation, engineering lessons, and repository boundaries.

## Important clarification

These case studies explain educational project designs. They are not production financial, lending, compliance, or investment systems, and their outputs must not be interpreted as professional financial advice or automated approval authority.
