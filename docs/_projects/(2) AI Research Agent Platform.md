---
name: AI Research Agent Platform
tools: [FastAPI, Next.js, LangGraph, Redis, PostgreSQL, pgvector, MCP, GitHub Actions]
image: https://images.unsplash.com/photo-1677442136019-21780ecad995?w=800
description: Full-stack AI agent platform with async document processing, multi-modal input support (text, voice, image), and tool-calling agent architecture via LangGraph with MCP protocol, achieving p95 latency under 2s and 85% test coverage.
---

# AI Research Agent Platform

**Duration:** Feb 2026 – Feb 2026  
**Tech Stack:** FastAPI, Next.js, LangGraph, Redis, PostgreSQL, pgvector, MCP Protocol, GitHub Actions  
**GitHub:** [github.com/shanshouli/AI-Research-Agent-Platform](https://github.com/shanshouli/AI-Research-Agent-Platform)

## Overview

Engineered a full-stack AI agent platform that combines async document processing, multi-modal input handling, and an intelligent tool-calling agent architecture to deliver a powerful research assistant with enterprise-grade reliability and performance.

## Architecture & Core Systems

### 🤖 Tool-Calling Agent (LangGraph + MCP)
- **Agent Orchestration:** Architected tool-calling agent via LangGraph with structured state management and dynamic tool routing
- **MCP Protocol Integration:** Decoupled retrieval, web search, and code execution into independently testable services using Model Context Protocol
- **Retry & Fallback Logic:** Implemented structured retry and fallback mechanisms, reducing agent error rate by **35%**
- **Modular Tool Services:** Each tool (retrieval, search, code execution) operates as an independent service with its own test suite

### 📄 Async Document Processing Pipeline
- **Redis Task Queue:** Asynchronous job scheduling for document ingestion and processing
- **PostgreSQL + pgvector:** Vector storage and similarity search for semantic document retrieval
- **Multi-Modal Input:** Support for text, voice, and image inputs with unified processing pipeline
- **Performance:** Achieved **p95 latency under 2 seconds** across all input modalities

### 🌐 Full-Stack Architecture
- **Backend:** FastAPI with async request handling and structured API design
- **Frontend:** Next.js with responsive UI for research workflows
- **Data Layer:** PostgreSQL for relational data, pgvector for embeddings, Redis for caching and task queues

## Key Achievements

### 📈 Performance & Reliability
- **p95 latency < 2s** for end-to-end request processing including multi-modal inputs
- **35% reduction in agent error rate** through structured retry and fallback logic
- **85% test coverage** across unit, integration, and end-to-end tests

### 🧪 Testing & CI/CD
- Comprehensive test suite with **85% coverage** spanning unit, integration, and e2e tests
- **GitHub Actions CI/CD** pipeline with automated testing and security scanning
- Independent service testing enabled by MCP protocol decoupling
