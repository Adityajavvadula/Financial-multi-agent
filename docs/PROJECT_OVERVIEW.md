# Multi-Agent Financial Research System

**Batch:** CSM-B12
**Project guide:** Mr M. Anil Kumar
**Project type:** Final-year major project

## 1. Overview

The Multi-Agent Financial Research System is a proposed platform for analysing user-provided financial documents. It aims to help finance students, MBA students, analysts and researchers locate evidence, extract financial metrics, identify potential red flags, compare financial information and obtain document-grounded answers.

The system is intended to use specialised agents and retrieval-augmented generation (RAG). Important outputs should include references to the source document so that users can verify the evidence.

## 2. Planned capabilities

- Upload and process financial PDF documents.
- Extract key financial metrics and ratios.
- Identify potential financial warning signs with supporting evidence.
- Compare selected metrics across companies or reports.
- Answer multi-part questions using retrieved document passages.
- Generate an analyst-style report with source citations.

These are project objectives, not claims that the features are already implemented.

## 3. Proposed agents

| Agent | Planned responsibility |
|---|---|
| Document Agent | Parse PDFs, create chunks, generate embeddings and index document content. |
| Extraction Agent | Extract financial metrics, values and ratios with source references. |
| Red Flag Agent | Identify potential risks and unusual patterns with evidence. |
| Comparison Agent | Compare selected financial indicators across reports. |
| Research Agent | Answer questions using retrieved document evidence. |
| Report Agent | Prepare a readable report from validated outputs and citations. |

## 4. Proposed technology stack

- **Backend:** Python, FastAPI
- **PDF processing:** PyMuPDF
- **Vector search:** ChromaDB
- **Frontend:** React
- **Language-model integration:** To be finalised by the team
- **Version control:** Git and GitHub

The final stack and versions will be confirmed during implementation.

## 5. Repository structure

```text
multi-agent-financial-research-system/
├── backend/
├── frontend/
├── data/
├── docs/
│   ├── PROJECT_PLAN.md
│   ├── RESEARCH_PROTOCOL.md
│   └── MEETING_UPDATE.md
├── .env.example
├── .gitignore
├── requirements.txt
└── README.md
```

## 6. Current status

**Initial repository/documentation setup. Implementation has not yet started.**

Do not interpret the planned capabilities above as completed features. Update this section only after the team has verified actual work and evidence.

## 7. Getting started

The implementation setup instructions will be added after the backend and frontend dependencies and run commands are finalised.

## 8. Project scope and limitations

The system is intended for document-grounded financial research. It is not intended to predict stock prices or provide investment recommendations. Generated interpretations should be distinguished from facts directly stated in source documents.

## 9. Team

Add the confirmed names and roll numbers of all CSM-B12 team members here.

## 10. Guide

Mr M. Anil Kumar
