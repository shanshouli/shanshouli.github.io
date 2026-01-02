---
name: ESG Reporting & AI Analytics Platform
tools: [Next.js, React, TypeScript, FastAPI, RAG, PostgreSQL]
image: https://images.unsplash.com/photo-1454165804606-c3d57bc86b40?w=800
description: Full-stack ESG reporting platform with ETL + RAG workflows for document ingestion, analytics, chat, and report generation.
---

# ESG Reporting & AI Analytics Platform

**Duration:** 2024  
**Tech Stack:** Next.js, React, TypeScript, FastAPI, Python, Supabase (PostgreSQL/Storage/Auth), OpenAI, FAISS, sentence-transformers, pandas, Docker

## Overview

Built a full-stack ESG reporting platform that ingests multi-format documents, runs ETL + RAG workflows, and delivers analytics, chat, and report generation for ESG compliance.

## Architecture & Services

- **Frontend Dashboard:** Next.js analytics, document management, and chat UI
- **Backend API:** Flask upload/ETL orchestration, analytics endpoints, report generation, JWT auth
- **RAG Service:** Flask microservice for semantic chunking, entity/relationship extraction, graph analytics, and LLM querying
- **Data Platform:** Supabase Storage + Postgres for documents, metadata, and graph persistence

## Key Achievements

- Delivered multi-format ingestion (PDF/DOCX/Excel/CSV) with semantic chunking, table extraction, and OCR fallback
- Implemented hybrid RAG pipeline with query intent classification, graph retrieval, and streaming responses
- Added automatic SIA chart generation (bar/pie/scatter/metric cards) embedded in reports with minimal pipeline changes
- Exposed report generation with progress tracking and cancellation endpoints

## Technical Implementation

- **Parsing:** PyMuPDF with pdfminer/PyPDF2 fallback, Camelot table extraction, image extraction
- **NLP:** Language detection, multilingual embeddings, semantic chunking, entity/relationship extraction
- **Retrieval:** FAISS vector search + NetworkX graph analysis + tabular analytics
- **Storage/Auth:** Supabase Postgres + Storage, JWT-protected APIs

## DevOps & Deployment

- Dockerized frontend, backend, and RAG services with environment-driven configuration
- Health checks and reproducible local setup scripts

## Technical Highlights

- Automated report generation flow with GRI support
- Tabular analytics pipeline for Excel/CSV with structured storage and query endpoints
- Streaming chat interface for ESG Q&A grounded in ingested documents

## Impact

Enabled teams to transform raw ESG documents into searchable knowledge graphs and report-ready insights, speeding up ESG reporting workflows.
