# YouTube Analytics Data Platform 🎬📊

An end-to-end **data engineering project** that simulates the scale of YouTube Analytics using **batch + streaming pipelines, data modeling, and ML**.

---

## 🚀 Architecture

```mermaid
flowchart TD
    A[YouTube API / Kafka Events] -->|Ingest| B[Raw Data Lake]
    B -->|Batch PySpark ETL| C[Staging Layer]
    C -->|Transform| D[Curated Layer]
    D -->|Modeling| E[Analytics Layer - Star Schema]
    E -->|Serve| F[ML Model: Trending Predictor]
    E -->|Query| G[Streamlit Dashboard]

```
