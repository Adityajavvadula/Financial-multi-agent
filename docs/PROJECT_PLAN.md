# Project Plan

## Project

Multi-Agent Financial Research System — CSM-B12
Guide: Mr M. Anil Kumar

## Goal

Develop a document-grounded system that helps users analyse financial reports through specialised agents. The system should retain source references for important extracted values and generated claims.

## Planned agent responsibilities

1. **Document Agent:** PDF parsing, text extraction, chunking, embeddings and indexing.
2. **Extraction Agent:** financial metrics, values and ratios.
3. **Red Flag Agent:** potential risks and anomalies with supporting evidence.
4. **Comparison Agent:** comparison of selected indicators across companies/reports.
5. **Research Agent:** multi-part question answering using retrieved passages.
6. **Report Agent:** analyst-style report generation with citations.

## Module roadmap

| Module | Focus | Indicative project weeks |
|---|---|---|
| M0 | Foundations: financial statements, ReAct agents and RAG basics | Foundation |
| M1 | Research design and evaluation protocol | 1–2 |
| M2 | Document ingestion from financial filings | 2–3 |
| M3 | Chunking, embeddings and indexing | 3–4 |
| M4 | Financial metric extraction | 4–5 |
| M5 | Red-flag detection | 5–6 |
| M6 | Peer comparison | 6–7 |
| M7 | Source-grounded research answers | 7–8 |
| M8 | Multi-agent orchestration | 7–9 |
| M9 | Full-stack platform | 3–10 |
| M10 | Report generation, manuscript and release | 9–12 |

Use the coordinator's latest schedule for official deadlines and progress reporting.

## Proposed development sequence

1. Confirm research questions, scope and evaluation protocol with the guide.
2. Select sample financial documents and define expected outputs.
3. Implement and test PDF ingestion.
4. Compare chunking and retrieval approaches.
5. Implement each agent with clear input/output schemas.
6. Add orchestration and error handling.
7. Integrate the frontend and backend.
8. Evaluate accuracy, faithfulness, citation quality and response time.
9. Generate reports and prepare project documentation.

## Current status

Initial planning/documentation only. The team has not yet confirmed implementation work for this repository. Update this section after checking with all team members.
