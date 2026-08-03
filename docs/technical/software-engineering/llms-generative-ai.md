# LLMs & Generative AI

## Overview

Technical leadership on custom LLM and generative-AI projects spanning
RAG pipeline design, multi-LLM orchestration, prompt engineering, and
fine-tuning with proprietary datasets. Covers atomic translation-unit
management for XLIFF/TMX workflows, vector storage operations, and
compliance/governance around data ownership and per-client separation.

## Technologies & tools

- **Ollama** — self-hosted LLM runtime on Ubuntu
- **Zep** — on-premise vector store and knowledge graph
- **Qdrant** — vector storage with snapshot management
- **Cheshire Cat** — AI agent customization framework
- **n8n** — workflow automation integrated with LLM pipelines
- **TypeScript** — frontend integration layer with LLM backends
- Custom REST API orchestration for proprietary LLM engine
- **XLIFF**, **TMX**, **JSON** — translation industry document formats
  with bidirectional conversion

## Responsibilities & operational scope

- Technical lead role on custom LLM and generative-AI projects
- Prompt engineering across AI-powered systems and AI-generated task
  pipelines
- Use of proprietary datasets (translation memories in TMX/XLIFF) for
  fine-tuning
- Benchmark creation on XLIFF input/output flows
- Custom RAG pipeline design, traditional fine-tuning, and vector storage
  snapshot management (Qdrant)
- Embedding optimization and segment filtering
- Differentiation of fixed versus temporary knowledge
- Priority and weighting mechanisms to influence document selection
  within RAG
- Atomic management of Translation Units (TUs) with unique IDs:
  sentence- and paragraph-level segmentation, 100% match and fuzzy
  match handling in XLIFF files
- Multi-LLM environment orchestration
- RESTful API orchestration with proprietary routes for a custom LLM
  engine
- Bidirectional document conversion between JSON and XLIFF
- Customization of AI agents and LLM models for business tasks (e.g.
  Cheshire Cat)
- Compliance and governance: data ownership, ethical compliance, data
  separation per client and per industry sector

## Projects & evidence

### Project: Zep + Ollama Self-Hosted Knowledge Management System (Ongoing)

Leading the design and implementation of a self-hosted RAG (Retrieval-
Augmented Generation) knowledge management and helpdesk system using Zep
and Ollama on Ubuntu servers. The project integrates a complex corpus of
approximately 3,000 pages of hand-authored documentation, structured
across nine hierarchical levels with embedded hyperlinks spanning
multiple IT domains, including server architecture, cybersecurity, IT
governance, internal ticketing systems, onboarding procedures, and
internal development workflows.

Key responsibilities include configuring Zep as an on-premise vector
store and knowledge graph, orchestrating document ingestion, embedding,
and semantic search; integrating Zep with TypeScript frontends and n8n
workflows for automated query handling; managing context assembly for
LLM-driven responses; and ensuring persistence of conversations and
knowledge updates. The architecture enables secure, low-latency internal
helpdesk operations while maintaining full control over sensitive
corporate data.

The project demonstrates advanced skills in enterprise knowledge
management, vector database design, self-hosted LLM integration, and
end-to-end automation pipelines, applied to a highly complex and
manually curated knowledge base.

*Technology stack: Ubuntu, Zep, Ollama, Qdrant, TypeScript, n8n.*

### TransTools Multiple Replace - Configure Entire Document and Replace All
<!-- graphify-evidence-id: e79951e0d470 -->

- **Source**: `rimuovi_a_capo_Transtools(3).png`
- **Graph community**: 18

*Evidence text to be enriched from source document.*

*Technology stack: to be enriched from source document.*

