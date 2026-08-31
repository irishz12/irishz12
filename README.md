# Hi, I'm Rishikesh 👋

**GenAI / Applied AI Engineer** building retrieval, evaluation, and agentic systems in Python on AWS — focused on making AI systems *verifiably correct*, not just impressive in a demo.

 Currently: Data Science Intern @ Kotak Life Insurance — testing and evaluating a GenAI Sales Assistant, and building a RAG evaluation & benchmarking framework on AWS Bedrock (RAGAS, DeepEval).

📍 Bengaluru, India · 🎓 B.Tech CSE (AI & ML), JAIN University — 2026

---

##  Featured Projects

###  [Hybrid RAG for Insurance Product Q&A](https://github.com/irishz12/Benefit-Explorer)
A full-stack RAG system answering factual and comparative questions across 6 insurance products straight from PDF brochures — hybrid BGE-M3 dense + BM25 sparse retrieval (RRF), BGE cross-encoder reranking, and Qwen3 32B generation via AWS Bedrock, with a citation-verification step that checks every generated claim against retrieved source text before it's shown.
**Scored:** Faithfulness 0.936 · Context Recall@4 0.837 · Answer Correctness 0.725 (RAGAS, 30-question benchmark)
`Python` `FastAPI` `Next.js` `Chroma` `AWS Bedrock`

###  [Guardrailed Multi-Agent Customer Support Automation](https://github.com/irishz12/AgentFlow-Support)
A LangGraph 4-agent pipeline (Planner → Investigation → Reflection Gate → Resolution) that proposes refund/replacement/escalation decisions — every proposal is validated by deterministic Python policy checks before execution. *"LLM proposes, Python validates, Action executes."*
**Scored:** 100% issue-classification · 93.94% resolution accuracy · 96.97% final-status accuracy (33-scenario suite, 2.29s avg latency)
`Python` `LangGraph` `FastAPI` `Next.js` `Docker`

###  [Training-Serving Feature Skew Detection Platform](https://github.com/irishz12/Skewless)
A side-by-side demo exposing training-serving feature skew: a LightGBM fare model scored through duplicated ("Broken") vs. shared ("Correct") feature-transformation pipelines, across 9 features and 3 injectable skew scenarios.
**Showed:** a distance-unit skew silently shifting a predicted fare from ~$20.29 (9/9 parity) to ~$29.19 (8/9 matched) — despite a valid API response either way.
`Python` `LightGBM` `FastAPI` `React` `pytest`

###  [Independent Flight Delay-Attribution Reconstruction](https://github.com/irishz12/airport-delay-propagation-analytics)
A pipeline processing 7.08M U.S. domestic flights (BTS, full-year 2024) through PostgreSQL bulk-loading and tail-number-based aircraft-rotation reconstruction, independently estimating delay propagation between an aircraft's consecutive legs and benchmarking it against the BTS's official attribution.
**Found:** 95.28% valid aircraft-link rate · 0.764 buffer-adjusted correlation · downstream delay rate falls from 69.06% (0–30 min buffer) to 15.29% (120+ min)
`Python` `PostgreSQL` `SQL` `Plotly Dash`

###  [Synthetic Data Validation & Optimization Platform](https://github.com/irishz12/Synthetic-Data-Validation-Optimization)
Generates synthetic tabular data (Gaussian Copula, CTGAN) and decides ACCEPT / REGENERATE / REJECT using four deterministic evaluation pillars — fidelity, rare-case retention, privacy-risk, and downstream ML utility — verified against a cryptographically locked, SHA-256-hashed holdout split. 276 automated tests, 96% coverage.
**Showed:** Gaussian Copula → REGENERATE (recall ratio 0.045 vs. 0.85 required) · CTGAN → ACCEPT (composite score 0.935), on the UCI Adult dataset (48,790 rows).
`Python` `pandas` `scikit-learn` `SDV` `Pandera`

---

##  Tech Stack

**GenAI & LLM:** RAG · LangGraph · AWS Bedrock (Converse API, Bedrock Mantle) · Strands Agents · LLM evaluation (RAGAS, DeepEval) · Prompt optimization & token accounting
**Cloud (AWS):** Bedrock · EC2 · S3 · SageMaker AI · IAM · DynamoDB
**ML & MLOps:** LightGBM · scikit-learn · feature engineering · MLflow · Docker · GitHub Actions (CI/CD) · model monitoring
**Backend & Data:** Python · SQL · FastAPI · Pydantic · PostgreSQL · SQLAlchemy · pandas · NumPy
**Visualization:** Plotly Dash · Tableau · Power BI

---

## 📫 Reach Me

[![LinkedIn](https://img.shields.io/badge/LinkedIn-0A66C2?style=flat&logo=linkedin&logoColor=white)](https://linkedin.com/in/rishikesh-k-g-5aa1002a8)
[![Email](https://img.shields.io/badge/Email-D14836?style=flat&logo=gmail&logoColor=white)](mailto:irishz121212@gmail.com)
