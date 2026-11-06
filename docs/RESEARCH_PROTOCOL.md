# Research Protocol — Working Draft

**Status:** Draft for discussion with the project guide. No experimental results or approved numeric targets are claimed.

## Working research questions

- **RQ1 — Metric extraction:** How accurately can the system extract selected financial metrics and ratios from uploaded financial reports?
- **RQ2 — Red-flag detection:** How effectively can the system identify potential financial warning signs and provide supporting evidence?
- **RQ3 — Grounded question answering:** Can the Research Agent answer multi-part questions using relevant passages and accurate source citations?
- **RQ4 — Multi-agent workflow:** Does dividing tasks among specialised agents improve completeness and traceability compared with a simpler single-step workflow?

## Proposed evaluation measures

| Area | Proposed measure | How it may be checked |
|---|---|---|
| Metric extraction | Extraction accuracy | Compare extracted values with manually verified reference values. |
| Citations | Citation accuracy | Check whether each cited page/passage supports its claim. |
| Red flags | Precision and recall | Compare detected flags with a manually reviewed labelled reference set. |
| Answer generation | Faithfulness | Check whether answer claims are supported by retrieved context. |
| Retrieval | Retrieval relevance/context precision | Review whether retrieved chunks contain evidence needed for the question. |
| System | Response time and completion rate | Record runtime and successful/failed task executions. |

## Baselines to discuss

- Manual analysis of the same financial document/questions.
- A general-purpose language model answering without retrieval.
- A retrieval-based workflow without multi-agent orchestration, if feasible.

## Dataset and benchmark

FinanceBench is a possible benchmark resource to study. The team must review its licensing, access requirements, dataset format and evaluation protocol before deciding whether and how to use it.

## Protocol decisions still required

- Which reports and questions will form the evaluation set?
- Which metrics and formulas will be used for each task?
- How many samples will be manually verified?
- What constitutes a correct citation?
- How will red-flag labels be created and reviewed?
- What baseline systems will be implemented?
- What numeric targets are realistic and approved by the guide?

## Reporting safeguards

- Separate proposed targets from measured results.
- Do not claim accuracy values until experiments have been run.
- Keep source document/page references for evaluated examples.
- Record failed cases and limitations, not only successful examples.
