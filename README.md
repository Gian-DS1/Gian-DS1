# Giancarlos Estévez

**Data engineer** · Santo Domingo, Dominican Republic · open to remote roles

I build data pipelines that hold up outside a notebook: real sources, point-in-time
correctness, tests and CI. MSc in Data Science & Business Analytics, currently studying
Software Engineering to pair the data side with solid engineering practice.

[LinkedIn](https://www.linkedin.com/in/gestevez-ds/)

## Projects

### [Stock Screener ML](https://github.com/Gian-DS1/stock-screener-ml)

Equity screener for the S&P 500 + NASDAQ 100 built on a strict *point-in-time* pipeline:
fundamentals enter by their real SEC filing date, macro series by their ALFRED vintage,
and 8-K sentiment only from the next business day — so the backtest can't learn from the
future. Trained on 298k rows (515 tickers, 34 features), with SHAP explanations per
signal, a rule-based exit engine and graduated drift monitoring.

`Python` · `scikit-learn` · `SEC EDGAR` · `FRED` · `FinBERT` · `FastAPI` · `React` · `pytest` · `GitHub Actions`

### [FinTrack](https://github.com/Gian-DS1/fintrack) · [live app](https://fintrack-rd.vercel.app)

Personal-finance PWA: zero-based budgeting, credit-card cycles, debts and savings goals.
Multi-currency, bilingual (es/en), installable, and backed by Postgres row-level security
so each user only ever reaches their own rows.

`React 19` · `Vite` · `Supabase (Postgres + RLS)` · `Tailwind` · `Vitest` · `Playwright`

### [Zomato Data Pipeline](https://github.com/Gian-DS1/zomato-data-engineering-pipeline)

End-to-end batch pipeline on a modern data stack: ingestion into Snowflake, dbt staging
and mart models, Airflow orchestration, and an analytics layer with LLM review enrichment
and natural-language querying over the warehouse.

`Airflow` · `dbt` · `Snowflake` · `Python` · `Streamlit`

### [LIENZO](https://github.com/Gian-DS1/lienzo)

Desktop canvas for running several AI coding agents in parallel — each one in its own real
terminal, on an infinite board, driven by text or voice. macOS, Windows and Linux, with no
build step.

`Node.js` · `Express` · `WebSocket` · `xterm.js` · `node-pty`

## Toolbox

**Core** — Python · SQL · pandas · scikit-learn · Airflow · dbt · Snowflake · Parquet · FastAPI · Docker · GitHub Actions · pytest

**Also worked with** — AWS · Databricks · Power BI · Streamlit · React

## Background

- **MSc in Data Science & Business Analytics** — IMF Smart Education / UCAV, co-developed with Indra–Minsait
- Currently studying **Software Engineering**
- ~6 years in **customer service across regulated health and finance sectors** — real domain knowledge and the habit of absorbing complex business rules fast
- Spanish (native) · English (C1)
- Certifications: AWS Academy (ML & Cloud Foundations) · IBM Data Science · Google Cybersecurity · Alura LATAM (Data Science & AI Agents)

## How I build

I use AI-assisted development and I'm open about it. What I keep for myself are the
decisions — architecture, data integrity, trade-offs — and I don't ship anything I can't
explain, defend or extend on my own.
