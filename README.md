# Anirudh Ravipudi

**Data Engineer & AI/ML Developer** — New York City

I build systems that move, shape, and reason over data — from distributed pipelines that ingest and transform data at scale, to machine learning models that leave the notebook and run in production, to AI applications people actually use. My work spans the full stack: ingestion, feature engineering, model training and evaluation, serving infrastructure, and the REST APIs that tie it all together.

Currently a **Data Engineer at AI Cloud Solutions**, building data infrastructure for a financial services client — pipelines and models that support fraud detection, reporting, and analytics in a regulated environment. I hold a **Master's in Data Science & AI from Florida International University** (GPA 3.67).

I'm looking for full-time roles in **Data Engineering**, **Data Analytics**, and **AI/ML Engineering** across the US. I'm open to relocating anywhere, and I bring a genuine full-stack range — I'm as comfortable designing a Spark ETL job and an Airflow DAG as I am fine-tuning a transformer or shipping a FastAPI service behind it.

---

## What I Do

- **Design and build data pipelines** that hold up under real-world volume and messiness — batch and streaming, with attention to schema evolution, data quality, and cost.
- **Take ML from experiment to production** — not just training a model, but packaging, containerizing, and serving it so it's actually usable by something else.
- **Work across the modern data stack** — Spark, Airflow, Kafka, dbt, Delta Lake, Databricks, Snowflake — and across all three major clouds.
- **Apply LLMs to real business problems**, not demos: summarization, sentiment classification, and retrieval-augmented reasoning grounded in actual documents and data.
- **Care about the last mile** — an API that's documented and easy to call, a Docker image that just runs, a pipeline that fails loudly instead of silently.

Given the right opportunity, I want to keep doing exactly this at greater scale: owning data infrastructure end to end, mentoring on best practices, and pushing further into applied ML/AI systems that solve problems people actually have — not just problems that make for a good portfolio project.

---

## Projects

### [Fraud Detection Pipeline & ML System](https://github.com/anirudhcancode/fraud-detection-pipeline)
An end-to-end fraud detection system built on 284,807 real anonymized credit card transactions. I built the ETL layer in PySpark, engineering behavioral features (transaction velocity, amount deviation, time-of-day patterns) to capture the signal that raw transaction fields miss. I trained and compared Random Forest and XGBoost classifiers, tuning for the class imbalance inherent to fraud data, and landed on a model with a **0.98 ROC-AUC**. The final model is deployed behind a FastAPI service, containerized with Docker, so it can score transactions in near real time rather than sitting in a notebook. This project mirrors the kind of work I do day to day at AI Cloud Solutions — financial data at scale, where both accuracy and auditability matter.

### [LLM Financial Report Analyzer](https://github.com/anirudhcancode/llm-financial-analyzer)
An NLP pipeline purpose-built for financial text: earnings call transcripts. It uses **BART** for abstractive summarization to compress long transcripts into digestible summaries, **FinBERT** — a transformer pretrained specifically on financial language — for domain-aware sentiment classification, and **YAKE** for unsupervised keyword extraction to surface what each call was actually about. On a held-out test set, it correctly flagged Apple as the *only* negative report, at 94% confidence, which is a good proxy for how well domain-specific models outperform generic sentiment tools on financial language. The system exposes its outputs through a set of FastAPI endpoints with supporting visualizations, so the analysis is consumable rather than buried in JSON.

### [A/B Testing & Experimentation Platform](https://github.com/anirudhcancode/ab-testing-pipeline)
A full experimentation pipeline simulating a 10,000-user e-commerce checkout A/B test running over 14 days. It implements a proper statistical backbone — Z-tests for significance, confidence intervals, and lift metrics — rather than eyeballing a conversion rate difference. The pipeline detected a **26% conversion lift at p = 0.000007**, and the whole thing is wrapped in a REST API that supports on-demand simulation, so new experiments can be run and evaluated without touching the underlying code. This project reflects the kind of rigor I bring to any "does this actually work" question — the same instinct I apply when validating a pipeline or a model before it ships.

### AI Companion
A cross-platform AI assistant, live in production across iOS, Android, and web. It's built around persistent memory and a two-layer architecture — one layer handles tool-orchestrated reasoning about what context a given moment calls for, and the other maintains a continuously updated model of the person it's supporting. It's the project where I've gone deepest on applied LLM system design outside of a work context — memory architecture, retrieval, and the harder question of what a system should actually surface versus hold back. [Project overview →](https://anirudhcancode.github.io/portfolio/ai-companion-demo.html)

---

## Stack

**Data & Pipelines** — Python, SQL, PySpark, Airflow, Kafka, dbt, Delta Lake, Databricks, Snowflake
**Cloud & Infra** — AWS, Azure, GCP, Docker, Kubernetes
**ML & AI** — scikit-learn, XGBoost, HuggingFace Transformers, FastAPI, pgvector, LLM APIs
**Databases** — PostgreSQL, Snowflake, Delta Lake

---

## Certifications (in progress)

- Databricks Certified Data Engineer Associate
- Databricks Certified Data Engineer Professional

---

## Links

[Portfolio](https://anirudhcancode.github.io/portfolio) · [LinkedIn](https://linkedin.com/in/anirudhravipudi) · [Email](mailto:anirudhravipudi@outlook.com)
