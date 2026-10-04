# Portfolio index

The three primary projects cover web data extraction, document processing and PDF workflows. Public portfolio code is evidence of implementation; it is not evidence of client adoption or business outcomes.

| Project | Inputs and outputs | Evidence to inspect | Important limits |
| --- | --- | --- | --- |
| [Catalog Observatory](https://github.com/keremercin/ecommerce-price-intel) | Allowed catalog HTML/JSON-LD → SQLite snapshots, CSV/JSON, API and dashboard | Collector, resume/cache/retry tests, recorded 60-product run and actual dashboard image | Public sandbox with synthetic prices; no cross-store identity resolution |
| [Legal Document Workbench](https://github.com/keremercin/legal-doc-ai-pipeline) | TXT/text PDF/images → chunks, search, extracted fields and source-labelled snippets | Ingestion/QA validation tests, actual application image, grounding diagnostic with failures | Offline lexical search misses paraphrases; source overlap does not prove answerability; provider mode needs separate evaluation |
| [PDF Layout Translator](https://github.com/keremercin/pdf-layout-translator) | PDF → translated PDF, job status and credit ledger | Real PDF pipeline fixture demo, identity/ownership tests, concurrent claim and transaction rollback tests | Fixture translation is not AI quality evidence; recovery requires stopped workers; no automatic distributed recovery |

## Supporting references

| Repository | Honest scope |
| --- | --- |
| ai-automation-toolkit | Small automation endpoints; rule-based logic and optional provider path |
| lead-support-doc-intake | Local workflow demonstration; destination labels are not external delivery |
| rag-eval-observatory | Evaluation calculations and stored run fixtures; not a live RAG quality benchmark |
| finance-loan-approval-prediction | Tabular ML baseline and inference packaging; current model-selection scores are not a separate final test |
| gym-customer-churn-prediction | Synthetic-data ML exercise; no measured retention impact |
| doctor-data-scraper / stock-data-scraper / linkedin-scraper | Archived earlier extraction examples with narrower functionality |

Forks remain attributed to their upstream projects. No customer names, usage counts or results are inferred from repository presence.

## Demonstration and verification

Start from each project's README. Inspect source-linked outputs and run the provided commands. Recorded local results apply to the documented configuration; historical CI badges do not prove that unpublished changes passed remote CI.
