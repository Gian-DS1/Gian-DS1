<div align="center">

<a href="https://github.com/Gian-DS1">
  <picture>
    <source media="(prefers-color-scheme: dark)" srcset="assets/banner-dark.v9.svg">
    <source media="(prefers-color-scheme: light)" srcset="assets/banner-light.v9.svg">
    <img src="assets/banner-light.v9.svg" width="960" alt="Giancarlos Estévez — Data Engineer. Animated portrait, Python and SQL silhouettes, and profile in a city-pop terminal.">
  </picture>
</a>

<br>

<img src="https://readme-typing-svg.demolab.com?font=JetBrains+Mono&amp;weight=700&amp;size=26&amp;duration=2600&amp;pause=900&amp;color=F78CA0&amp;center=true&amp;vCenter=true&amp;width=900&amp;lines=Giancarlos+Est%C3%A9vez+%E2%80%94+Data+Engineer%3BPython+%C2%B7+SQL+%C2%B7+Airflow+%C2%B7+dbt%3BPoint-in-time+correct+data+pipelines%3BMSc+Data+Science+%26+Business+Analytics" alt="Giancarlos Estévez — Data Engineer · Python · SQL · Airflow · dbt · point-in-time correct pipelines">

<br>

<img src="https://img.shields.io/badge/status-open_to_remote_roles-f78ca0?style=flat-square&amp;logoColor=1a1a2e" alt="Open to remote roles">

</div>

---

## `$ whoami`

<p align="center">
  <img src="assets/whoami-citypop.svg" width="960" alt="Giancarlos Estévez, Data Engineer in Santo Domingo, Dominican Republic. Python, SQL, Airflow, dbt, Snowflake, Docker and CI.">
</p>

**Data engineer** · Santo Domingo, Dominican Republic · open to remote roles

I build data pipelines that hold up outside a notebook: real sources, point-in-time
correctness, tests and CI. MSc in Data Science & Business Analytics, currently studying
Software Engineering to pair the data side with solid engineering practice.


---

## `$ cat tech-stack.yaml`

<table>
  <thead>
    <tr><th colspan="2" align="left"><code>Gian-DS1:~$ cat tech-stack.yaml</code></th></tr>
  </thead>
  <tbody>
    <tr>
      <td width="50%" valign="top"><code>├─ ◈ data_foundations:</code><br><br>
        <img src="https://skillicons.dev/icons?i=python,postgres" alt="Python and PostgreSQL"><br><br>
        <img src="https://img.shields.io/badge/pandas-c7a4f5?style=flat-square&amp;logo=pandas&amp;logoColor=1a1a2e" alt="pandas">
        <img src="https://img.shields.io/badge/Parquet-76d8d2?style=flat-square&amp;logo=apacheparquet&amp;logoColor=1a1a2e" alt="Parquet"><br>
        <sub><code>Python · SQL · pandas · Parquet</code></sub>
      </td>
      <td width="50%" valign="top"><code>├─ ⇄ pipelines_warehouse:</code><br><br>
        <img src="https://img.shields.io/badge/Airflow-f78ca0?style=for-the-badge&amp;logo=apacheairflow&amp;logoColor=1a1a2e" alt="Airflow"><br>
        <img src="https://img.shields.io/badge/dbt-c7a4f5?style=for-the-badge&amp;logo=dbt&amp;logoColor=1a1a2e" alt="dbt"><br>
        <img src="https://img.shields.io/badge/Snowflake-76d8d2?style=for-the-badge&amp;logo=snowflake&amp;logoColor=1a1a2e" alt="Snowflake"><br>
        <sub><code>Airflow · dbt · Snowflake</code></sub>
      </td>
    </tr>
    <tr>
      <td valign="top"><code>├─ ✦ machine_learning:</code><br><br>
        <img src="https://img.shields.io/badge/scikit--learn-f3d29b?style=for-the-badge&amp;logo=scikitlearn&amp;logoColor=1a1a2e" alt="scikit-learn"><br>
        <sub><code>scikit-learn · SHAP · FinBERT</code></sub>
      </td>
      <td valign="top"><code>├─ ▣ api_engineering:</code><br><br>
        <img src="https://skillicons.dev/icons?i=fastapi,nodejs,express" alt="FastAPI, Node.js and Express"><br>
        <sub><code>FastAPI · Node.js · Express · WebSocket</code></sub>
      </td>
    </tr>
    <tr>
      <td valign="top"><code>├─ ⚙ delivery_quality:</code><br><br>
        <img src="https://skillicons.dev/icons?i=docker,githubactions" alt="Docker and GitHub Actions"><br><br>
        <img src="https://img.shields.io/badge/pytest-76d8d2?style=flat-square&amp;logo=pytest&amp;logoColor=1a1a2e" alt="pytest">
        <img src="https://img.shields.io/badge/Vitest-c7a4f5?style=flat-square&amp;logo=vitest&amp;logoColor=1a1a2e" alt="Vitest">
        <img src="https://img.shields.io/badge/Playwright-f78ca0?style=flat-square" alt="Playwright"><br>
        <sub><code>Docker · GitHub Actions · pytest · Vitest · Playwright</code></sub>
      </td>
      <td valign="top"><code>╰─ ⌁ also_worked_with:</code><br><br>
        <img src="https://skillicons.dev/icons?i=aws,react" alt="AWS and React"><br><br>
        <img src="https://img.shields.io/badge/Databricks-f78ca0?style=flat-square&amp;logo=databricks&amp;logoColor=1a1a2e" alt="Databricks">
        <img src="https://img.shields.io/badge/Power_BI-f3d29b?style=flat-square" alt="Power BI">
        <img src="https://img.shields.io/badge/Streamlit-c7a4f5?style=flat-square&amp;logo=streamlit&amp;logoColor=1a1a2e" alt="Streamlit"><br>
        <sub><code>AWS · Databricks · Power BI · Streamlit · React</code></sub>
      </td>
    </tr>
  </tbody>
  <tfoot><tr><td colspan="2"><code>focus: data engineering · status: open to remote roles</code></td></tr></tfoot>
</table>

---

## `$ ls projects/`

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

---

## `$ python scripts/radar.py`

<p align="center">
  <picture>
    <source media="(prefers-color-scheme: dark)" srcset="assets/radar-dark.svg">
    <source media="(prefers-color-scheme: light)" srcset="assets/radar-light.svg">
    <img src="assets/radar-light.svg" width="390" alt="Coverage across four featured projects: data pipelines 50%, machine learning 25%, web apps 75%, finance 50%, orchestration 25%, agent tooling 25%.">
  </picture>
  <picture>
    <source media="(prefers-color-scheme: dark)" srcset="assets/radar-langs-dark.svg">
    <source media="(prefers-color-scheme: light)" srcset="assets/radar-langs-light.svg">
    <img src="assets/radar-langs-light.svg" width="370" alt="Public repository language mix: JavaScript, Python, TypeScript, PLpgSQL, PowerShell and Swift, scaled by relative byte count.">
  </picture>
</p>

<p align="center"><sub>Project coverage: share of the four featured projects in each category. Language mix: public repository bytes, square-root scaled relative to the largest language. Snapshot: 2026-10-01.</sub></p>

---

## `$ git log --stats`

<div align="center">

<picture>
  <source media="(prefers-color-scheme: dark)" srcset="./profile/stats-dark.svg">
  <img height="160" alt="Giancarlos Estevez's GitHub stats: commits, pull requests, issues and stars" src="./profile/stats-light.svg">
</picture>
<picture>
  <source media="(prefers-color-scheme: dark)" srcset="./profile/langs-dark.svg">
  <img height="160" alt="Most used languages on Giancarlos Estevez's GitHub" src="./profile/langs-light.svg">
</picture>


</div>

---

## `$ cat background.md`

- **MSc in Data Science & Business Analytics** — IMF Smart Education / UCAV, co-developed with Indra–Minsait
- Currently studying **Software Engineering**
- ~6 years in **customer service across regulated health and finance sectors** — real domain knowledge and the habit of absorbing complex business rules fast
- Spanish (native) · English (C1)
- Certifications: AWS Academy (ML & Cloud Foundations) · IBM Data Science · Google Cybersecurity


---

## `$ connect --socials`

<div align="center">

<a href="https://www.linkedin.com/in/gestevez-ds/">
  <img src="https://img.shields.io/badge/LinkedIn-c7a4f5?style=for-the-badge&amp;logo=linkedin&amp;logoColor=1a1a2e" alt="Connect with Giancarlos Estévez on LinkedIn">
</a>&nbsp;&nbsp;
<a href="https://github.com/Gian-DS1">
  <img src="https://img.shields.io/badge/GitHub-f78ca0?style=for-the-badge&amp;logo=github&amp;logoColor=1a1a2e" alt="Giancarlos Estévez on GitHub">
</a>

<br><br>

<sub>Santo Domingo, Dominican Republic · @Gian-DS1 · always learning</sub><br>
<sub>City-pop design and SVG generators adapted from <a href="https://github.com/macu-dev/macu-dev">macu-dev/macu-dev</a>.</sub>

</div>
