---
name: Robust Data Processor - Multi-Tenant Log Ingestion System
tools: [Go, AWS Lambda, SQS, DynamoDB, API Gateway, Terraform]
image: https://images.unsplash.com/photo-1558494949-ef010cbdcc31?w=800
description: Serverless, multi-tenant log ingestion pipeline in Go with async processing, strict isolation, and resilience testing.
---

# Robust Data Processor - Multi-Tenant Log Ingestion System

**Duration:** 2025 Nov
**Tech Stack:** Go, AWS Lambda, SQS, DynamoDB, API Gateway, Terraform, CloudWatch

## Overview

Built a serverless, multi-tenant log ingestion system on AWS. It normalizes JSON/text logs into a unified internal message, enqueues them for async processing, and stores results with strict tenant isolation.

## Key Achievements

- Delivered a single `/ingest` endpoint with immediate `202 Accepted` for non-blocking ingestion
- Ensured tenant isolation using DynamoDB partition keys (no cross-tenant queries)
- Implemented idempotent writes with conditional checks to avoid duplicates on retries
- Added DLQ-based failure handling and retry policy for resiliency
- Integrated PII redaction and crash simulation for chaos testing

## Architecture & Data Flow

- **API Gateway → Ingest Lambda (Go):** Validates content type, extracts tenant ID, normalizes payload, enqueues to SQS
- **SQS → Worker Lambda (Go):** Processes messages asynchronously and applies redaction
- **DynamoDB:** Stores log records per tenant with strict key partitioning

## Technical Highlights

- Unified JSON and text ingestion into a single internal message schema
- Configured SQS visibility timeout and max receive count for safe retry behavior
- Used CloudWatch metrics/logs for observability and incident triage

## Impact

Enabled high-throughput log ingestion (1,000+ RPM) with strong isolation guarantees and graceful failure recovery, reducing operational risk for multi-tenant workloads.
