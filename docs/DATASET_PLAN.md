# Financial Dataset Collection and Evaluation Protocol
**Project:** Multi-Agent Financial Research System (CSM-B12)  
**Assigned Member:** Kusumuru Teja (teja007ai-ops)  
**Guide:** Mr. M. Anil Kumar  

## 1. Objective
To establish a rigorous, mathematically verifiable ground-truth dataset for evaluating the multi-agent system's retrieval and extraction accuracy. This fulfills Module M1 (Research Design & Evaluation Protocol) by defining benchmark data, numeric targets, and baseline comparisons.

## 2. Primary Dataset: FinanceBench
We will utilize the **FinanceBench** dataset (arXiv:2311.11944) as our primary benchmark for financial question answering. 
* **Repository:** `patronus-ai/financebench`
* **Data Structure:** 10,000+ QA pairs sourced from public SEC filings (10-K, 10-Q, 8-K).
* **Target Question Categories:** The dataset covers exact numeric extraction (e.g., "What is the FY23 Net Income?"), ratio calculations (e.g., Operating Margin), and relational mapping (e.g., subsidiary risk exposure).

## 3. Secondary Data: SEC EDGAR Ingestion (M2 Preparation)
To evaluate the Document Agent's ingestion pipeline, we will download 5 primary 10-K filings from a single sector (e.g., Technology - AAPL, MSFT) directly from the SEC EDGAR database. 
* **Validation Layer:** Extracted values from the PDFs must be cross-checked against native **XBRL** data via the `Arelle` library to prove extraction accuracy without LLM hallucination.

## 4. Evaluation Metrics & Numeric Targets (RAGAS Framework)
To transition from a subjective summarizer to a verifiable research tool, the dataset will be used to calculate the following metrics using the `explodinggradients/ragas` framework:
1. **Citation Faithfulness:** Measures if the final generated answer is entirely supported by the retrieved context (Target: > 90%).
2. **Context Precision:** Measures the signal-to-noise ratio of the retrieved chunks (Target: > 85%).
3. **Extraction Accuracy:** Exact match of floating-point numbers and units against the XBRL ground truth (Target: > 95%).
4. **Red-Flag Recall:** Ability of the system to identify all labeled risk factors within a document (Target: > 85%).

## 5. Baselines for Comparison
Our system's performance on this dataset will be benchmarked against three baselines:
* **Baseline 1:** Manual reading time for junior analysts.
* **Baseline 2:** A general-purpose LLM (e.g., Llama-3.3-70B) attempting to answer the questions without RAG retrieval.
* **Baseline 3:** Standard flat-vector RAG (1,000-character chunks) to demonstrate how table-splitting degrades financial extraction.

## 6. Execution Steps
1. Clone `patronus-ai/financebench` and extract a 50-question pilot test set.
2. Download one sample 10-K filing and its associated 8-K restatements.
3. Map the FinanceBench question types to the specific agents (Extraction, Red-Flag, Comparison) responsible for processing them.