# Hi, I'm Topher 👋

**Analytics Engineer & full-stack AI product builder.**

By day I work as an analytics engineer — building and maintaining data platforms with **dbt**, **Airflow** (Google Cloud Composer), and **BigQuery**, ingesting from a couple of dozen advertising-platform sources through custom API integrations and transforming it all into modelled, tested, business-ready data. By night I design and ship full-stack, AI-powered products end to end.

I came to engineering through data science and analytics, so I'm as comfortable with a forecasting model or an NLP pipeline as I am with a production data warehouse or a Flutter app talking to a Postgres backend.

```text
Data / Analytics Engineering   dbt · Airflow (Cloud Composer) · BigQuery · SQL · Python · custom REST API integrations
Product / Full-stack           Flutter/Dart · Supabase (PostgreSQL/PostgREST/RLS) · Deno edge functions · Next.js · TypeScript/React
AI / ML                        LLM app pipelines · fine-tuning (LoRA) · TensorFlow · scikit-learn · NLP · time-series forecasting
```

---

## 🌟 Featured project — History Check

**[History Check](https://historycheck.app)** — *Your campaign never forgets.*

A web-first app for tabletop-RPG Game Masters that **records a session, transcribes it, and uses AI to do the bookkeeping** — generating summaries and automatically extracting the NPCs, locations, items, monsters and organisations that came up, then tracking them across a whole campaign.

I built this solo, end to end:

- **Frontend** — Flutter web (Dart), Riverpod state management, `go_router`, responsive layout.
- **Audio capture** — in-browser recording via the MediaRecorder API (Opus), chunked and uploaded incrementally to cloud storage so a GM can close the tab mid-session and lose nothing; crash/refresh recovery reconciles local cache against what made it to storage.
- **Backend** — Supabase (PostgreSQL) as the single source of truth, accessed directly over PostgREST with **row-level security** enforcing a multi-user owner/viewer (GM/player) permission model, token-based invite links, and `SECURITY DEFINER` RPCs.
- **AI pipeline** — a fully server-side pipeline (Deno edge functions): audio → **AssemblyAI** transcription with speaker diarization → **Google Gemini** for structured (JSON-schema) summarisation and entity extraction. API keys never touch the client.
- **Production engineering** — Sentry observability, Realtime status updates, a Paddle/Stripe billing + feature-gating layer, separate staging/production Supabase + deploy pipelines, and a test suite of **1,100+ Flutter tests plus ~70 edge-function test files**.

> Stack: Flutter · Dart · Supabase · PostgreSQL · Deno · TypeScript · AssemblyAI · Google Gemini · Next.js (marketing) · Sentry · Paddle

---

## 🔭 What I'm working on

- **Analytics engineering (professional)** — production data platforms on Google Cloud: multi-source ingestion from ~two dozen ad-platform APIs, dbt transformation layers with testing, and Airflow/Cloud Composer orchestration for both dbt and business-logic pipelines. Also hands-on with agentic-AI tooling layered on top of that data.
- **[History Check](https://historycheck.app)** — see above; actively developed.
- **Smaller products & tools** — habit/activity trackers and other apps built with TypeScript/React/Vite and local-first storage.

---

## 🤖 AI / Data Science projects

| Project | What it does | Tech |
| --- | --- | --- |
| [Fine-tuning an LLM for RPG statblocks](https://tophercollins.github.io/rpg-statblock-generator.html) | LoRA fine-tune of Llama 3 to generate D&D monster statblocks; dataset + adapters published on Hugging Face | Llama 3 · Unsloth · Hugging Face |
| [Handwritten character recognition](https://tophercollins.github.io/handwritten-character-recognition.html) | CNN for automated scorecard processing, incl. artificially-constructed strikethrough characters; 99% test accuracy | TensorFlow · CNN |
| [Smoker classification](https://tophercollins.github.io/smoker-classification.html) | Ensemble stacking classifier (CatBoost/XGBoost/LightGBM/RF + NN) for a Kaggle Playground competition | scikit-learn · TensorFlow |
| [Red card / goal analysis](https://tophercollins.github.io/red-card-goal-analysis.html) | EDA + hypothesis testing across 20,000 European football matches | Pandas · Matplotlib · SciPy |
| [EIFO data extraction](https://tophercollins.github.io/eifo-data-extraction.html) | Web-scraper for country risk & cover policies, exported to Excel | BeautifulSoup · Selenium |

*Time-series (Bitcoin forecasting), NLP (medical-text classification), and transfer-learning (Food101) projects are detailed in the portfolio.*

---

## 🎲 Gaming roots

A long-time Dungeons & Dragons / tabletop-RPG nerd — which is where most of my side projects come from, including **[DnDwithToph.com](https://dndwithtoph.com)** (a Flask + SQLAlchemy platform for online D&D play) and the [Zombie Survival](https://tophercollins.github.io/zombie-survival.html) OOP game.

---

## 📫 Find me

- 🌐 **Portfolio:** [tophercollins.github.io](https://tophercollins.github.io/)
- 💼 **LinkedIn:** [christopher-collins](https://www.linkedin.com/in/christopher-collins-47419555/)
- ✍️ **Medium:** [@tophercollins](https://medium.com/@tophercollins/)
