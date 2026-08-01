<!--
**gladytdavianus/gladytdavianus** is a ✨ _special_ ✨ repository because its `README.md` (this file) appears on your GitHub profile.
-->
<!-- Banner / Header -->
<p align="center">
  <img src="https://capsule-render.vercel.app/api?type=waving&color=0:0f2027,100:2c5364&height=200&section=header&text=Hi,%20I'm%20Davi%20👋&fontSize=40&fontColor=ffffff" />
</p>

<h3 align="center">Instrument & Control Engineer → Data Engineer</h3>
<p align="center">
  10 years building reliable industrial control systems, now applying that same discipline to data pipelines.
</p>

---

### About Me

- Instrument & Control Engineer since 2016. SCADA, sensor calibration, process reliability.
- Transitioning into Data Engineering, applying that same discipline for reliability and monitoring to data pipelines
- Building end-to-end pipelines with Python, PySpark, Airflow, PostgreSQL, and Docker
- Linux user, daily-driving Neovim, tmux, and zsh in a terminal-first workflow

---

### Featured Projects

**[crypto-market-pipeline](https://github.com/gladytdavianus/crypto-market-pipeline)**

End-to-end cryptocurrency market data pipeline — CoinGecko API → PySpark (transformation + 3-layer quality gate) → PostgreSQL (staging + upsert pattern) → orchestrated by two independent Airflow DAGs (daily incremental + manual backfill), fully containerized with Docker and backed by CI/CD via GitHub Actions.

- Idempotent loading (staging + `ON CONFLICT DO UPDATE`) — safe to retry, no duplicates
- Data quality validated before it reaches the database, not after
- Two isolated PostgreSQL instances (application data vs. Airflow metadata)
- SQL monitoring views for price anomalies, missing-date detection, and pipeline health
- CI (lint + type check) and CD (Docker image → GHCR) fully automated

**[crypto-market-elt](https://github.com/gladytdavianus/crypto-market-elt)**

Companion project to `crypto-market-pipeline`, same CoinGecko data source, opposite philosophy — CoinGecko API → raw JSON landing in BigQuery → dbt (staging + marts models) → orchestrated by two independent Airflow DAGs, fully containerized with Docker.

- Raw API responses land untouched as native BigQuery `JSON` columns; all parsing and typing happens in dbt, not Python
- dbt test suite (`unique`, `not_null`, `relationships`, plus a `dbt_utils` multi-column uniqueness check) runs against live BigQuery data on every push
- Runs entirely on BigQuery Sandbox (free tier), no billing account required
- A direct architectural comparison: ETL in the companion project vs. ELT here

---

### Tech Stack

<p>
  <img src="https://img.shields.io/badge/Python-3776AB?logo=python&logoColor=white" />
  <img src="https://img.shields.io/badge/Apache%20Spark-E25A1C?logo=apachespark&logoColor=white" />
  <img src="https://img.shields.io/badge/Apache%20Airflow-017CEE?logo=apacheairflow&logoColor=white" />
  <img src="https://img.shields.io/badge/PostgreSQL-4169E1?logo=postgresql&logoColor=white" />
  <img src="https://img.shields.io/badge/Docker-2496ED?logo=docker&logoColor=white" />
  <img src="https://img.shields.io/badge/Poetry-60A5FA?logo=poetry&logoColor=white" />
  <img src="https://img.shields.io/badge/Git-F05032?logo=git&logoColor=white" />
  <img src="https://img.shields.io/badge/dbt-FF694B?logo=dbt&logoColor=white" />
  <img src="https://img.shields.io/badge/Google%20BigQuery-4285F4?logo=googlebigquery&logoColor=white" />
  <img src="https://img.shields.io/badge/Linux-FCC624?logo=linux&logoColor=black" />
  <img src="https://img.shields.io/badge/Neovim-57A143?logo=neovim&logoColor=white" />
</p>

---

### Contact

<p align="center">
  <a href="https://gt-davianus.vercel.app">
    <img src="https://img.shields.io/badge/Portfolio-000000?logo=vercel&logoColor=white" />
  </a>
  <a href="https://www.linkedin.com/in/glady-t-davianus-4554a797/">
    <img src="https://img.shields.io/badge/LinkedIn-0A66C2?logo=linkedin&logoColor=white" />
  </a>
  <a href="mailto:gladytdavianus@gmail.com">
    <img src="https://img.shields.io/badge/Email-D14836?logo=gmail&logoColor=white" />
  </a>
</p>

---

<p align="center">
  <img src="https://readme-typing-svg.herokuapp.com?font=Fira+Code&size=20&pause=1000&color=2C5364&center=true&vCenter=true&width=650&lines=10+years+in+Instrumentation+%26+Control;Now+building+data+pipelines+that+don't+break;Reliability-minded+by+background%2C+by+choice" />
</p>

<!-- Footer -->
<p align="center">
  <img src="https://capsule-render.vercel.app/api?type=waving&color=0:0f2027,100:2c5364&height=120&section=footer"/>
</p>
