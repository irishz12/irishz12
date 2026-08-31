# Hi, I'm Rishikesh 

**GenAI / Applied AI Engineer** building retrieval, evaluation, and agentic systems in Python on AWS — focused on making AI systems *verifiably correct*, not just impressive in a demo.

 Bengaluru, India ·  B.Tech CSE (AI & ML), JAIN University — 2026

---

## Featured Projects

### [Agentic Multi-Hop RAG](https://github.com/irishz12/multihop-rag-agent)
A cost-aware RAG system benchmarked on MultiHop-RAG (Tang & Yang, COLM 2024). An agentic controller iteratively retrieves across up to 3 hops until evidence is judged sufficient, evaluated against 4 baselines — Dense, Hybrid, Hybrid+Reranker, and a learned cost-optimized Adaptive router — using an independent LLM judge and a sealed, hash-verified holdout split.
**Scored:** Evidence coverage 63.2% → 81.5% (baseline → agentic) on multi-hop questions · Adaptive RAG retains 80% answer quality at 21.8% lower cost
🔗 [Live demo](https://multi-hop-rag.vercel.app)
`Python` `Qdrant` `FastAPI` `Next.js` `scikit-learn`

### [GenAI ReleaseGate](https://github.com/irishz12/GenAI-ReleaseGate)
Statistical release-gating for production LLM prompts. Scores a candidate prompt against production on quality, safety (real AWS Bedrock Guardrails), cost, and latency, runs paired bootstrap significance tests with Holm-Bonferroni correction, and returns a declarative GO / REVIEW / HOLD / INVALID verdict — no manual override.
**Scored:** 5 of 6 real candidate prompts rejected or flagged for review before one passed both a 120-case dev set and a sealed 40-case holdout
🔗 [Live demo](https://genai-releasegate.vercel.app)
`Python` `FastAPI` `Next.js` `AWS Bedrock Guardrails`

### [Synthetic Data Validation & Optimization Platform](https://github.com/irishz12/Synthetic-Data-Validation-Optimization)
Generates synthetic tabular data (Gaussian Copula, CTGAN) and issues an ACCEPT / REGENERATE / REJECT decision across four evaluation pillars — fidelity, rare-case retention, privacy-risk, and downstream ML utility — verified against a cryptographically locked, SHA-256-hashed holdout split. 276 automated tests, 96% coverage.
**Scored:** Gaussian Copula → REGENERATE (recall ratio 0.045 vs. 0.85 required) · CTGAN → ACCEPT (composite score 0.935), on the UCI Adult dataset (48,790 rows)
`Python` `pandas` `scikit-learn` `SDV` `Pandera`

### [Machine Failure Early-Warning System](https://github.com/irishz12/machine-failure-early-warning)
A classic supervised-learning predictive-maintenance pipeline — Random Forest vs. XGBoost vs. Logistic Regression under class-imbalance-aware training (3.4% failure rate), an F2-tuned decision threshold, 5-fold stratified cross-validation, and live per-prediction SHAP explanations served through FastAPI + Streamlit.
**Scored:** PR-AUC 0.933 · 90.2% recall at a 0.6% false-positive rate on a held-out test set
`Python` `scikit-learn` `XGBoost` `SHAP` `FastAPI` `Docker`

### [Hybrid RAG for Insurance Product Q&A](https://github.com/irishz12/Benefit-Explorer)
A full-stack RAG system answering factual and comparative questions across 6 insurance products straight from PDF brochures — hybrid BGE-M3 dense + BM25 sparse retrieval (RRF), BGE cross-encoder reranking, and Qwen3 32B generation via AWS Bedrock, with a citation-verification step that checks every generated claim against retrieved source text.
**Scored:** Faithfulness 0.936 · Context Recall@4 0.837 · Answer Correctness 0.725 (RAGAS, 30-question benchmark)
`Python` `FastAPI` `Next.js` `Chroma` `AWS Bedrock`

### [Guardrailed Multi-Agent Customer Support Automation](https://github.com/irishz12/AgentFlow-Support)
A LangGraph 4-agent pipeline (Planner → Investigation → Reflection Gate → Resolution) that proposes refund/replacement/escalation decisions — every proposal is validated by deterministic Python policy checks before execution. *"LLM proposes, Python validates, Action executes."*
**Scored:** 100% issue-classification · 93.94% resolution accuracy · 96.97% final-status accuracy (33-scenario suite)
`Python` `LangGraph` `FastAPI` `Next.js` `Docker`

### [Training-Serving Feature Skew Detection Platform](https://github.com/irishz12/Skewless)
An interactive demo exposing training-serving feature skew: a LightGBM fare model scored through duplicated ("Broken") vs. shared ("Correct") feature-transformation pipelines, across 9 features and 3 injectable skew scenarios.
**Showed:** a distance-unit skew silently shifting a predicted fare from ~$20.29 (9/9 parity) to ~$29.19 (8/9 matched)
`Python` `LightGBM` `FastAPI` `React` `pytest`

### [Independent Flight Delay-Attribution Reconstruction](https://github.com/irishz12/airport-delay-propagation-analytics)
A pipeline processing 7.08M U.S. domestic flights (BTS, full-year 2024) through PostgreSQL bulk-loading and tail-number-based aircraft-rotation reconstruction, independently estimating delay propagation and benchmarking it against the BTS's official attribution.
**Found:** 95.28% valid aircraft-link rate · 0.764 buffer-adjusted correlation · downstream delay rate falls from 69.06% to 15.29% as buffer time increases
`Python` `PostgreSQL` `SQL` `Plotly Dash`

---

## Other Projects

- **[Sales Intelligence Platform](https://github.com/irishz12/Sales-Intelligence)** — ML lead-scoring classifier (Hot / Warm / Cold) with a Streamlit dashboard.
- **[Customer Churn Prediction Dashboard](https://github.com/irishz12/customer-churn-project)** — Logistic Regression churn model (ROC-AUC 0.83) with an interactive Streamlit dashboard.

---

## Tech Stack

**GenAI & LLM:** RAG · Multi-hop / agentic RAG · LangGraph · AWS Bedrock (Converse API, Bedrock Mantle, Guardrails) · Strands Agents · Local LLM serving (Ollama) · LLM evaluation (RAGAS, DeepEval, LLM-as-judge) · Statistical release gating (bootstrap CIs, Holm-Bonferroni)
**Cloud (AWS):** Bedrock · EC2 · S3 · SageMaker AI · IAM · DynamoDB
**ML & MLOps:** LightGBM · XGBoost · scikit-learn · SHAP · feature engineering · MLflow · Docker · GitHub Actions (CI/CD)
**Backend & Data:** Python · SQL · FastAPI · Next.js · Pydantic · PostgreSQL · SQLAlchemy · pandas · NumPy · FAISS · Qdrant
**Visualization:** Plotly Dash · Tableau · Power BI

---

## Reach Me

[![LinkedIn](https://img.shields.io/badge/LinkedIn-0A66C2?style=flat&logo=linkedin&logoColor=white)](https://linkedin.com/in/rishikesh-k-g-5aa1002a8)
[![Email](https://img.shields.io/badge/Email-D14836?style=flat&logo=gmail&logoColor=white)](mailto:irishz121212@gmail.com)
