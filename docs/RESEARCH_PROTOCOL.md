# Research Design and Evaluation Protocol

# 

# Project: Multi-Agent Financial Research System

# Batch: CSM-B12

# Guide: Mr M. Anil Kumar

# 

# 1\. Research Objective

# 

# The objective of this project is to develop a multi-agent AI system that analyses financial documents, extracts important financial information, identifies potential risks, compares financial performance and answers user questions with supporting document citations.

# 

# 2\. Research Questions

# 

# RQ1: How accurately can the system extract financial metrics from financial reports?

# 

# RQ2: How effectively can the system identify potential financial red flags?

# 

# RQ3: How accurately can the system answer financial questions with supporting citations?

# 

# RQ4: Does a multi-agent RAG system perform better than a general-purpose LLM without document retrieval?

# 

# 3\. Evaluation Metrics and Proposed Targets

# 

# Metric

# 

# Definition

# 

# Proposed target

# 

# Extraction Accuracy

# 

# Correctly extracted values / Total evaluated values × 100

# 

# ≥ 90%

# 

# Citation Accuracy

# 

# Supported citations / Total citations evaluated × 100

# 

# ≥ 90%

# 

# Red-Flag Precision

# 

# TP / (TP + FP)

# 

# ≥ 80%

# 

# Red-Flag Recall

# 

# TP / (TP + FN)

# 

# ≥ 75%

# 

# Retrieval Relevance

# 

# Relevant retrieved chunks / Total retrieved chunks evaluated × 100

# 

# ≥ 80%

# 

# Note: These are initial research targets and must be reviewed and approved by the project guide.

# 

# 4\. Dataset

# 

# The project will use publicly available financial reports and the FinanceBench benchmark for financial question-answering evaluation.

# 

# The evaluation documents will include annual reports and financial statements.

# 

# Reference answers and supporting evidence will be used to assess the correctness of system outputs.

# 

# 5\. Baseline Methods

# 

# The proposed system will be compared against:

# 

# Manual Reading: A person reads financial reports and answers selected questions.

# 

# General-Purpose LLM: An LLM answers questions without retrieving evidence from the uploaded documents.

# 

# Proposed Multi-Agent RAG System: Specialised agents retrieve relevant document sections, extract information and generate answers with citations.

# 

# 6\. Experimental Procedure

# 

# Collect financial reports and benchmark questions.

# 

# Extract text from the documents.

# 

# Divide documents into smaller chunks.

# 

# Generate embeddings and store them in a vector database.

# 

# Retrieve relevant document sections for each question.

# 

# Extract financial metrics and identify potential red flags.

# 

# Generate answers with source citations.

# 

# Compare the results with reference answers.

# 

# Calculate evaluation metrics.

# 

# Record observations and limitations.

# 

# 7\. Evaluation Plan

# 

# The initial pilot evaluation will use:

# 

# 50 financial question-answering examples.

# 

# 100 manually verified financial metric values.

# 

# A manually reviewed and labelled set of financial risk examples.

# 

# The final evaluation sample sizes will be decided after reviewing dataset availability and guide feedback.

# 

# 8\. Expected Outcomes

# 

# Accurate extraction of financial information.

# 

# Identification of potential financial warning signs.

# 

# Answers supported by financial document evidence.

# 

# Reduced manual research effort.

# 

# Improved transparency and traceability of financial analysis.

# 

# 9\. Current Status

# 

# Research design and evaluation metrics are being prepared. Dataset selection, baseline implementation and experimental evaluation are pending.

# 

# No experimental results or performance claims have been established yet.

