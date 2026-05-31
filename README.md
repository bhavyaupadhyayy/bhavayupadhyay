<div align="center">
  <img src="banner.svg" alt="Bhavya Upadhyay - Data Engineer & ML Practitioner" width="100%" />
</div>

<div align="center">

[![LinkedIn](https://img.shields.io/badge/LinkedIn-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/bhavyaupadhyay/)
[![Portfolio](https://img.shields.io/badge/Portfolio-1A1A1A?style=for-the-badge&logo=googlechrome&logoColor=white)](https://bhavyaupadhyay.site)
[![Email](https://img.shields.io/badge/Email-D14836?style=for-the-badge&logo=gmail&logoColor=white)](mailto:officiallybhavya@gmail.com)
[![Resume](https://img.shields.io/badge/Resume-2E9EF7?style=for-the-badge&logo=readthedocs&logoColor=white)](https://bhavyaupadhyay.site)

</div>

---

## 🧭 About

**Data Engineer & ML practitioner** building end-to-end data and ML systems: production ETL pipelines, LLM/RAG applications, and deep-learning models served behind APIs.

At **TCS (Air Canada)** I shipped AWS Lambda ETL pipelines processing **10M+ records/month**, cutting data latency by 50% and improving pipeline SLA compliance to 99.9%. Now completing my **Master of Data Science at UC Irvine** on a full merit scholarship, while working as a Data Analyst at the Graduate Division building retention models and KPI dashboards across 20+ programs.

```yaml
Role:        Data Engineer / ML Engineer  (full-time, available Jan 2027)
Strongest:   Python · SQL · AWS · Airflow · dbt · Snowflake
Building:    Kafka streaming + OpenSky live positions for Flightline
Contact:     officiallybhavya@gmail.com
```

---

## ✈️ Flightline — How It Works

My most recent build: a production flight-data pipeline. Diagram is the real architecture.

```mermaid
flowchart LR
    A["US BTS<br/>On-Time Data"] -->|Airflow DAG| C[("Snowflake<br/>Raw")]
    B["OpenSky API"] -->|OAuth2 + Kafka| C
    C -->|dbt| D["Staging"]
    D --> E["Fact + Dimension"]
    E --> F["Aggregates<br/>26/26 tests"]
    F --> G(["Streamlit<br/>Dashboard"])

    classDef src fill:#161b22,stroke:#58A6FF,color:#E6EDF3;
    classDef core fill:#0d3b5c,stroke:#29B5E8,color:#E6EDF3;
    classDef out fill:#1a3326,stroke:#3fb950,color:#E6EDF3;
    class A,B src;
    class C,D,E,F core;
    class G out;
```

> CI lints SQL with `sqlfluff` and runs `dbt build` against an ephemeral schema on every push. Idempotent partition-delete-before-COPY loads prevent drift on reruns.

---

## 🚀 Featured Projects

### ✈️ [Flightline — End-to-End Flight Data Pipeline](https://github.com/bhavyaupadhyayy/Flightline-End-to-End-Flight-Data-Pipeline)
Batch ingestion of US BTS data → **Snowflake** → **dbt** (26/26 tests) → live **Streamlit** dashboard, orchestrated with **Airflow**, with a Kafka streaming path for live flight positions.
`Airflow` · `dbt` · `Snowflake` · `Kafka` · `Docker` · `GitHub Actions`

### 🛰️ [Signal Miner — LLM Market Intelligence](https://github.com/bhavyaupadhyayy/saas-signal-miner)
LLM pipeline (LangChain prompt chaining + RAG) turning unstructured market data from 250+ sources into clean, structured records. Containerized with Docker.
`Python` · `LangChain` · `RAG` · `Supabase` · `Docker`

### 🔎 [Duplicate Detection in Job Postings](https://github.com/bhavyaupadhyayy/bayesian-duplicate-detection)
Semantic deduplication over 250K+ postings; precision lifted **68% → 92%**, ~3x faster matching via optimized ANN indexing.
`Sentence Transformers` · `Milvus` · `RAG`

### 🩺 [Skin Lesion Classification](https://github.com/bhavyaupadhyayy/skin-lesion-classification)
EfficientNet-B0 + CBAM attention on ISIC 2019 (8 classes); ablation across 4 variants, Grad-CAM interpretability, served via FastAPI.
`PyTorch` · `FastAPI` · `Grad-CAM`

---

## 🛠️ Tech Stack

**Languages**
<p>
<img src="https://img.shields.io/badge/Python-3776AB?style=flat-square&logo=python&logoColor=white" />
<img src="https://img.shields.io/badge/SQL-4479A1?style=flat-square&logo=postgresql&logoColor=white" />
<img src="https://img.shields.io/badge/R-276DC3?style=flat-square&logo=r&logoColor=white" />
<img src="https://img.shields.io/badge/Bash-4EAA25?style=flat-square&logo=gnubash&logoColor=white" />
</p>

**Data Engineering & Cloud**
<p>
<img src="https://img.shields.io/badge/AWS-232F3E?style=flat-square&logo=amazonaws&logoColor=white" />
<img src="https://img.shields.io/badge/Airflow-017CEE?style=flat-square&logo=apacheairflow&logoColor=white" />
<img src="https://img.shields.io/badge/dbt-FF694B?style=flat-square&logo=dbt&logoColor=white" />
<img src="https://img.shields.io/badge/Snowflake-29B5E8?style=flat-square&logo=snowflake&logoColor=white" />
<img src="https://img.shields.io/badge/Kafka-231F20?style=flat-square&logo=apachekafka&logoColor=white" />
<img src="https://img.shields.io/badge/Docker-2496ED?style=flat-square&logo=docker&logoColor=white" />
<img src="https://img.shields.io/badge/FastAPI-009688?style=flat-square&logo=fastapi&logoColor=white" />
<img src="https://img.shields.io/badge/Git-F05032?style=flat-square&logo=git&logoColor=white" />
</p>

**ML / AI**
<p>
<img src="https://img.shields.io/badge/PyTorch-EE4C2C?style=flat-square&logo=pytorch&logoColor=white" />
<img src="https://img.shields.io/badge/scikit--learn-F7931E?style=flat-square&logo=scikitlearn&logoColor=white" />
<img src="https://img.shields.io/badge/Hugging%20Face-FFD21E?style=flat-square&logo=huggingface&logoColor=black" />
<img src="https://img.shields.io/badge/LangChain-1C3C3C?style=flat-square&logo=langchain&logoColor=white" />
</p>

**Analytics & Viz**
<p>
<img src="https://img.shields.io/badge/Pandas-150458?style=flat-square&logo=pandas&logoColor=white" />
<img src="https://img.shields.io/badge/Tableau-E97627?style=flat-square&logo=tableau&logoColor=white" />
<img src="https://img.shields.io/badge/Streamlit-FF4B4B?style=flat-square&logo=streamlit&logoColor=white" />
</p>

---

<div align="center">
<sub>Building reliable data systems, one pipeline at a time.</sub>
</div>

<!--
ADD LATER once Flightline v2 commits fill out your graph. A stats card looks
great, but only when the numbers help you. Today your contribution count is
your weakest stat, so adding it now advertises the wrong thing:

![Stats](https://github-readme-stats.vercel.app/api?username=bhavyaupadhyayy&show_icons=true&hide_border=true&count_private=true)
-->
