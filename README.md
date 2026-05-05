[![Typing SVG](https://readme-typing-svg.herokuapp.com?size=28&color=4A90E2&center=true&vCenter=true&width=1100&pause=2000&lines=📊+ANALYTICS+ENGINEER+%7C+MARKETING+%26+REVENUE+DATA;⚙️+dbt+%7C+Snowflake+%7C+Airflow+%7C+BigQuery+%7C+Docker;🔁+END-TO-END+PIPELINES+%7C+VALIDATED+KPIs+%7C+BI+DASHBOARDS;💡+TURNING+RAW+DATA+INTO+DECISIONS)](https://github.com/ApostolicDA)

# 👋 About Me

Hi, I'm **Proud Ndlovu** — an **Analytics Engineer** specialising in marketing and revenue data pipelines, dbt modelling, and executive BI dashboards.

My background is unusual. I spent 2+ years in performance marketing analytics optimising $10K–$25K monthly ad budgets across US, UK, AU, and SA markets. That work taught me something most engineers miss: data only matters when it changes a decision. I now bring that business-first mindset to full-stack analytics engineering.

I specialise in the full pipeline lifecycle:

**Raw Data → Ingestion → Cloud Warehouse → dbt Staging → dbt Marts → Validated KPIs → Executive Dashboard**

🔹 Based in **Johannesburg, South Africa** — open to remote globally (US · UK · AU · EU)
🔹 Stack: **SQL · Python · dbt · Snowflake · BigQuery · Apache Airflow · Docker · Looker Studio · Power BI**
🔹 Recognised as **Star Performer (91%)** at Saint Louis University x Excelerate internship
🔹 Focused on **analytics engineering, data quality, and pipelines that connect directly to business decisions**

---

# 🧰 Core Skills

### Analytics Engineering and Data Pipeline

[![SQL](https://img.shields.io/badge/SQL-4479A1?style=for-the-badge&logo=mysql&logoColor=white)](https://github.com/ApostolicDA)
[![PostgreSQL](https://img.shields.io/badge/PostgreSQL-336791?style=for-the-badge&logo=postgresql&logoColor=white)](https://github.com/ApostolicDA)
[![BigQuery](https://img.shields.io/badge/BigQuery-4285F4?style=for-the-badge&logo=googlebigquery&logoColor=white)](https://github.com/ApostolicDA)
[![Snowflake](https://img.shields.io/badge/Snowflake-29B5E8?style=for-the-badge&logo=snowflake&logoColor=white)](https://github.com/ApostolicDA)
[![dbt](https://img.shields.io/badge/dbt-FF694B?style=for-the-badge&logo=dbt&logoColor=white)](https://github.com/ApostolicDA)
[![Python](https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white)](https://github.com/ApostolicDA)
[![Pandas](https://img.shields.io/badge/Pandas-150458?style=for-the-badge&logo=pandas&logoColor=white)](https://github.com/ApostolicDA)
[![Airflow](https://img.shields.io/badge/Airflow-017CEE?style=for-the-badge&logo=apacheairflow&logoColor=white)](https://github.com/ApostolicDA)
[![Docker](https://img.shields.io/badge/Docker-2496ED?style=for-the-badge&logo=docker&logoColor=white)](https://github.com/ApostolicDA)

**Capabilities**

- End-to-end pipeline design: ingestion, staging, mart layers, orchestration
- dbt modelling (staging + marts) on BigQuery and Snowflake
- Apache Airflow DAG authoring, scheduling, and failure handling
- Docker containerisation for full pipeline reproducibility
- SQL data modelling: star-schema design, CTEs, window functions
- ETL/ELT design and data quality frameworks
- Marketing analytics: ROAS, CAC, LTV, churn, cohort retention

---

### Business Intelligence and Data Visualization

[![Power BI](https://img.shields.io/badge/Power%20BI-F2C811?style=for-the-badge&logo=power-bi&logoColor=black)](https://github.com/ApostolicDA)
[![Looker Studio](https://img.shields.io/badge/Looker%20Studio-4285F4?style=for-the-badge&logo=googleanalytics&logoColor=white)](https://github.com/ApostolicDA)
[![Tableau](https://img.shields.io/badge/Tableau-E97627?style=for-the-badge&logo=tableau&logoColor=white)](https://github.com/ApostolicDA)
[![Excel](https://img.shields.io/badge/Excel-217346?style=for-the-badge&logo=microsoft-excel&logoColor=white)](https://github.com/ApostolicDA)

**Capabilities**

- Executive dashboards from dbt mart layer outputs
- KPI validation frameworks: every metric reconciled against source data
- Funnel analysis, cohort retention, and churn visualisation
- Data storytelling for technical and non-technical stakeholders

---

### DevOps and Development Tools

[![Git](https://img.shields.io/badge/Git-F05032?style=for-the-badge&logo=git&logoColor=white)](https://github.com/ApostolicDA)
[![GitHub](https://img.shields.io/badge/GitHub-181717?style=for-the-badge&logo=github&logoColor=white)](https://github.com/ApostolicDA)
[![GitHub Actions](https://img.shields.io/badge/GitHub_Actions-2088FF?style=for-the-badge&logo=githubactions&logoColor=white)](https://github.com/ApostolicDA)
[![VSCode](https://img.shields.io/badge/VSCode-007ACC?style=for-the-badge&logo=visualstudiocode&logoColor=white)](https://github.com/ApostolicDA)
[![Jupyter](https://img.shields.io/badge/Jupyter-F37726?style=for-the-badge&logo=jupyter&logoColor=white)](https://github.com/ApostolicDA)

---

# 🚀 Featured Projects

---

## ⚙️ Crypto Market Analytics Pipeline — Architectural Evolution

> One pipeline. Two generations. A deliberate engineering decision between each.

This is my most complete engineering project. It documents not just what I built, but why I rebuilt it and what I learned between versions. The domain is crypto market data. The architecture mirrors what powers data teams at scale across any domain.

---

### Version 1 — BigQuery + dbt + GitHub Actions

**Repo:** [coingecko-analytics-pipeline](https://github.com/ApostolicDA/coingecko-analytics-pipeline)
**Stack:** `Python` `BigQuery` `dbt` `Looker Studio` `GitHub Actions`

**What I built**

A fully automated analytics pipeline ingesting live data from 4 external APIs into BigQuery, transforming it through dbt staging and mart layers, and delivering a 3-page Looker Studio executive dashboard, running daily at 06:00 UTC with zero manual intervention.

```
4 External APIs (CoinGecko · Fear & Greed · ExchangeRate · Global Market)
      ↓
Python Ingestion — pulls all sources, writes to BigQuery raw layer
      ↓
BigQuery Raw Layer — full fidelity, timestamped, no transformation
      ↓
dbt Staging Layer — clean, cast, rename, document (one model per source)
      ↓
dbt Mart Layer — business logic, cross-source joins, decision-ready metrics
      ↓
dbt Test Suite — not_null, unique, accepted_values on every model
      ↓
Looker Studio Dashboard — 3 pages, live, interactive
      ↓
GitHub Actions — daily schedule, fully automated
```

**dbt model architecture**

Staging layer: one model per source, strictly limited to type casting, column renaming, and NULL handling. No business logic whatsoever.

Mart layer: all business logic lives here — cross-currency pricing, aggregations, sentiment classification, dominance signals.

| Mart Model | Purpose |
|---|---|
| mart_coin_performance | Market cap rankings, ZAR/EUR pricing, performance categorisation |
| mart_market_sentiment | BTC dominance, momentum signals, sentiment classification |
| mart_fx_crypto_correlation | BTC/ETH dominance vs Fear & Greed index, macro risk signals |

**Two real data quality issues caught during the build**

Issue 1 caught by dbt tests: BTC was returning NULL from the exchange rate API on the free tier. The not_null test flagged it immediately. Fixed at ingestion, clean data reloaded, all tests passed.

Issue 2 caught by visual validation: FX scorecards were summing rates across 10 mart rows instead of averaging, producing USD/ZAR of 163.9 instead of 16.41. Caught through human eyes on the dashboard output.

The lesson: dbt tests catch structural issues. Business logic validation requires human eyes on the output. Both layers matter. Neither replaces the other.

**Live dashboard:** [View in Looker Studio](https://lookerstudio.google.com/reporting/5b2423b8-a2c7-44b6-8aa1-62b36d16311d)

---

### Version 2 — Snowflake + dbt + Apache Airflow + Docker

**Repo:** [snowflake_crypto](https://github.com/ApostolicDA/snowflake_crypto)
**Stack:** `Python` `Snowflake` `dbt` `Apache Airflow` `Docker` `Looker Studio`

**Why I rebuilt it**

After completing Version 1, I identified three architectural limitations worth addressing:

GitHub Actions is a solid CI/CD tool but it is not a workflow orchestrator. It has no native support for task dependencies, retry logic, alerting, or observability across a DAG. For a production pipeline, that matters.

BigQuery is excellent but Snowflake's separation of compute and storage, its clone and time-travel capabilities, and its enterprise adoption made it worth learning and building on.

The pipeline had no containerisation. Moving it between environments required manual dependency management. That is a problem in any team context.

**What changed**

Migrated the full warehouse layer from BigQuery to Snowflake, rebuilding all dbt models and tests to target the new warehouse while preserving transformation logic and data quality coverage.

Replaced GitHub Actions with Apache Airflow. DAGs now handle task dependency, upstream success gating, retry logic for transient API failures, and orchestration observability.

```
[Fetch APIs] → [Load to Snowflake] → [dbt run] → [dbt test] → [Dashboard refresh]
```

Each ingestion task is independent. Downstream tasks gate on upstream success. dbt serves as both the transformation layer and the quality gate before the dashboard refreshes.

Containerised the full environment in Docker. One command bootstraps Airflow, dbt, and all ingestion dependencies across any machine.

```bash
docker-compose up
```

Added performance optimisations: incremental models where applicable to avoid full reprocessing, column pruning to reduce Snowflake scan costs, domain-separated marts to keep query surfaces narrow.

**What stayed the same**

The staging and mart layer philosophy is identical across both versions. Staging cleans and standardises. Marts contain all business logic. That separation is the right pattern regardless of which warehouse sits underneath.

The dual validation strategy is the same. Automated dbt tests plus visual reconciliation against warehouse data. Both are required.

**Architecture comparison**

| Dimension | Version 1 | Version 2 |
|---|---|---|
| Warehouse | BigQuery | Snowflake |
| Orchestration | GitHub Actions | Apache Airflow |
| Containerisation | None | Docker |
| Incremental models | No | Yes |
| Retry logic | Limited | Native Airflow |
| Environment portability | Manual setup | docker-compose up |

---

## 📊 Marketing Analytics dbt Pipeline

**Repo:** [marketing-analytics-dbt](https://github.com/ApostolicDA/marketing-analytics-dbt)
**Stack:** `BigQuery` `dbt` `Looker Studio` `GitHub`

Production-style analytics engineering pipeline tracking 2.7M+ in revenue across 5 marketing channels.

**Key work**

Built staging models (stg_customers, stg_orders, stg_order_items) feeding mart models (mart_channel_performance, mart_churn_risk, mart_cohort_retention) in dbt on BigQuery.

Search identified as the top revenue channel at 2M+ in total revenue. Cohort retention analysis surfaced a sharp first-month drop-off, directly informing early engagement strategy. High churn risk customers showed significantly higher average days since last order.

Full pipeline version-controlled on GitHub with a live Looker Studio executive dashboard.

`dbt` `BigQuery` `SQL` `Looker Studio` `Analytics Engineering` `Cohort Analysis` `Git/GitHub`

🔗 [View Project on GitHub](https://github.com/ApostolicDA/marketing-analytics-dbt)

---

## 🎓 Governed Admissions Intelligence Pipeline

**Stack:** `PostgreSQL` `Supabase` `Looker Studio` `SQL` `Python`

End-to-end governed analytics pipeline built for real stakeholder delivery. This is not a portfolio exercise — the dashboard is actively used by university leadership for admissions decision-making.

**Key work**

Cleaned and quality-assured 6,800+ admissions records in PostgreSQL, resolving epoch timestamp conversion, one-to-many deduplication with DISTINCT ON, 90%+ missing Country data, and NULL-sensitive financial aggregations.

Designed a star-schema data model with one fact table and three dimension tables. Connected PostgreSQL to Supabase to Looker Studio for a live executive dashboard tracking the full admissions funnel.

Implemented a SQL KPI validation framework reconciling every dashboard metric against source data before stakeholder delivery. 100% accuracy across all KPIs and filters.

Led a cross-timezone international team of 6 as Team Lead. Recognised as Star Performer with a 91% score in a formal 360-degree evaluation.

`SQL` `PostgreSQL` `Star Schema` `ETL` `Data Governance` `KPI Validation` `Looker Studio` `Team Lead`

🔗 [View Project on GitHub](https://github.com/ApostolicDA/Governed-Admissions-Intelligence-Pipeline)

---

## 💰 Marketing ROAS Analytics Engine

**Repo:** [roas-analytics-sql](https://github.com/ApostolicDA/roas-analytics-sql)
**Stack:** `SQL` `PostgreSQL` `Python` `Power BI`

SQL-driven analytics engine computing ROAS, CAC, LTV, churn probability, and channel profitability across 6 relational tables.

Multi-CTE pipelines with window functions and CASE-based customer segmentation. Revenue vs spend reconciliation using NULLIF logic. Channel reallocation insights projecting 20–25% ROI improvement.

`SQL` `CTEs` `Window Functions` `Marketing Analytics` `ROAS` `CAC` `LTV` `Power BI`

🔗 [View Project on GitHub](https://github.com/ApostolicDA/roas-analytics-sql)

---

## 🛡 Bank Customer Churn and Fraud Risk Analysis

**Repo:** [bank-customer-churn-analysis](https://github.com/ApostolicDA/bank-customer-churn-analysis)
**Stack:** `Python` `SQL` `Power BI`

Identified a 20.37% churn rate across 10,000 customers. Single-product customers were 4x more likely to churn. Surfaced a 10.61% fraud rate with $38,990 exposure — 10% of users drove 80% of fraud activity.

Full Python to SQL to Power BI pipeline with KPI validation at every stage.

`Python` `Pandas` `SQL` `EDA` `Churn Analysis` `Fraud Detection` `Power BI`

🔗 [View Project on GitHub](https://github.com/ApostolicDA/bank-customer-churn-analysis)

---

# 💡 What I Bring

| Capability | Business Value |
|---|---|
| **Pipeline Architecture** | Designs ingestion, staging, and mart layers that are independently evolvable and easy to debug |
| **dbt Modelling** | Delivers clean, tested, version-controlled analytical models on BigQuery and Snowflake |
| **Data Quality** | Two-layer validation: automated dbt tests plus visual reconciliation against source data |
| **Airflow Orchestration** | Production-grade DAGs with task dependency, retry logic, and observability |
| **Business Context** | 2+ years in performance marketing means pipelines are designed around decisions, not just data |
| **Stakeholder Delivery** | Proven track record of delivering dashboards that stakeholders actually trust and use |

---

# 📚 Education and Certifications

| Qualification | Institution | Year |
|---|---|---|
| Star Performer Award — Data Visualization Associate Internship | Saint Louis University x Excelerate | March 2026 |
| Microsoft Power BI Data Analyst (PL-300) | NEMISA | In Progress |
| Data Analytics Bootcamp | aLex Data | 2025 |
| Advanced Diploma in Data Science and Machine Learning | Alison | 2023–2025 |

---

⭐ **Open to remote Analytics Engineer and BI Engineer roles globally.**
Built every pipeline from scratch. Every number validated. Every model documented.

📂 [github.com/ApostolicDA](https://github.com/ApostolicDA) · 📩 fanisaproud@gmail.com · 💼 [LinkedIn](https://linkedin.com/in/proud-ndlovu-89070854) · 📍 Johannesburg, SA (UTC+2)
