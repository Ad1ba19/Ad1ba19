# Hi, I'm Adiba Khan 👋

**Software Engineer · Backend Engineering, Data Engineering & AI Systems**

I build data pipelines, backend services and LLM-powered tools that turn messy business data into something people can act on. Day to day I work with Python, SQL, FastAPI, PostgreSQL, Docker and the Claude API, connecting systems like Microsoft 365 and CRM platforms into automated workflows.

[![LinkedIn](https://img.shields.io/badge/LinkedIn-Adiba%20Khan-0A66C2?logo=linkedin&logoColor=white)](https://www.linkedin.com/in/adiba-khan-20ba57230/)

---

## 🔧 What I've built at work

These systems run in production for a professional-services firm. The code stays private because it handles client data, so here is what they do and how they are built.

### Meeting Intelligence Pipeline
An automated daily pipeline that prepares a briefing for every external meeting on the partners' calendars.
- Reads calendars through **Microsoft Graph**, maps every outside attendee to a company through the CRM's **GraphQL API**, and skips internal meetings.
- Enriches each company from its website, Wikipedia and search APIs, then uses **Claude** with forced tool calls to extract structured fields.
- Guards against hallucination: every extracted value must come with a verbatim quote from its source or it is dropped, followed by a chain of fallbacks (search APIs, then manual overrides).
- Stores snapshots in **PostgreSQL** and caches news signals in **Redis**, both running in **Docker Compose**.
- Serves the data to another team through a **FastAPI** service with API-key authentication and cache-aside caching.

`Python` `FastAPI` `PostgreSQL` `Redis` `Docker` `SQLAlchemy` `Alembic` `Playwright` `Claude API` `GraphQL` `Microsoft Graph`

### Conflux: internal intelligence hub
A web app where the team reads every client note, opportunity, survey and agreement in one place, and asks questions of it in plain English.
- **FastAPI** backend with a single-page frontend in plain JavaScript.
- An AI analyst built on **Claude** that calls tools for exact pipeline counts, contacts and documents instead of guessing, with streamed answers and prompt caching to keep it fast.
- Scheduled background syncs with incremental updates, plus PBKDF2 password hashing and signed session cookies.
- Deployed on **Oracle Cloud** with systemd and Caddy (automatic HTTPS).

`Python` `FastAPI` `JavaScript` `Claude API` `Server-Sent Events` `Linux` `Caddy`

### Calendar Notes Automation
An operations console that replaces manual CRM and spreadsheet updates.
- **Streamlit** front end that runs long workflows in background processes and streams their logs live.
- Syncs CRM opportunities into a shared **SharePoint** Excel workbook through the Graph workbook API.
- Creates note events next to each meeting in the partners' calendars, and produces scheduling-conflict reports.

`Python` `Streamlit` `pandas` `Microsoft Graph` `SharePoint` `MSAL`

---

## 📂 Featured projects

| Project | What it does | Highlights |
|---|---|---|
| [Customer Segmentation with RFM](https://github.com/Ad1ba19/customer-segmentation-rfm-analysis) | Segments 12,926 e-commerce customers into 9 actionable groups | Tested Python module, CLI, CI on GitHub Actions. Found that 20% of customers drive 68% of revenue |
| [Road Lane Line Detection](https://github.com/Ad1ba19/Road-Lane-Line-Detection) | Finds lane lines in dashcam video with OpenCV | Runs at ~55 fps on a CPU, holds up in shadows |

---

## 🛠️ Tech stack

**Languages**
![Python](https://img.shields.io/badge/Python-3776AB?logo=python&logoColor=white)
![SQL](https://img.shields.io/badge/SQL-4479A1?logo=postgresql&logoColor=white)
![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?logo=javascript&logoColor=black)
![Bash](https://img.shields.io/badge/Bash-4EAA25?logo=gnubash&logoColor=white)

**Backend & APIs**
![FastAPI](https://img.shields.io/badge/FastAPI-009688?logo=fastapi&logoColor=white)
![GraphQL](https://img.shields.io/badge/GraphQL-E10098?logo=graphql&logoColor=white)
![SQLAlchemy](https://img.shields.io/badge/SQLAlchemy-D71F00?logo=sqlalchemy&logoColor=white)
![Pydantic](https://img.shields.io/badge/Pydantic-E92063?logo=pydantic&logoColor=white)

**Data**
![PostgreSQL](https://img.shields.io/badge/PostgreSQL-4169E1?logo=postgresql&logoColor=white)
![Redis](https://img.shields.io/badge/Redis-DC382D?logo=redis&logoColor=white)
![pandas](https://img.shields.io/badge/pandas-150458?logo=pandas&logoColor=white)
![NumPy](https://img.shields.io/badge/NumPy-013243?logo=numpy&logoColor=white)
![Power BI](https://img.shields.io/badge/Power%20BI-F2C811?logo=powerbi&logoColor=black)

**AI & ML**
![Claude API](https://img.shields.io/badge/Claude%20API-D97757?logo=anthropic&logoColor=white)
![scikit-learn](https://img.shields.io/badge/scikit--learn-F7931E?logo=scikitlearn&logoColor=white)
![OpenCV](https://img.shields.io/badge/OpenCV-5C3EE8?logo=opencv&logoColor=white)

**DevOps & Tools**
![Docker](https://img.shields.io/badge/Docker-2496ED?logo=docker&logoColor=white)
![Linux](https://img.shields.io/badge/Linux-FCC624?logo=linux&logoColor=black)
![Git](https://img.shields.io/badge/Git-F05032?logo=git&logoColor=white)
![GitHub Actions](https://img.shields.io/badge/GitHub%20Actions-2088FF?logo=githubactions&logoColor=white)
![Oracle Cloud](https://img.shields.io/badge/Oracle%20Cloud-F80000?logo=oracle&logoColor=white)
![Streamlit](https://img.shields.io/badge/Streamlit-FF4B4B?logo=streamlit&logoColor=white)

---

## 📈 GitHub stats

![Adiba's GitHub stats](https://github-readme-stats.vercel.app/api?username=Ad1ba19&show_icons=true&count_private=true&hide_border=true&theme=transparent)

---

## 🌱 Currently

- Learning more about data orchestration (Airflow) and cloud data warehouses
- Turning internal tools into reusable, tested Python packages
- Open to Software Engineering roles in backend, data and AI systems

**Let's connect on [LinkedIn](https://www.linkedin.com/in/adiba-khan-20ba57230/).**
