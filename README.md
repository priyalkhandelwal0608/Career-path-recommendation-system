#  Career Path & Job Recommendation System

**A Hybrid ML system that recommends personalized career paths using Semantic Search (BERT + FAISS) and Collaborative Filtering.**

---

##  Overview
This project empowers students and professionals to discover their ideal career trajectories by analyzing skills, GPA, and professional experiences. By merging **Semantic Search** (for career titles) with **Collaborative Filtering** (for user profile similarity), the system provides a dual-layer recommendation engine that is both contextually aware and data-driven.

**Why it matters:** Traditional keyword searches fail to capture the nuance of skill sets. This system enables recruiters and counselors to match candidates to roles based on deep semantic meaning and historical profile success.

---

##  Features
- **Hybrid Recommendation Engine:**
  - **Semantic Search:** Uses `Sentence-Transformers` (BERT) to convert career names into high-dimensional embeddings, with `FAISS` for lightning-fast similarity indexing.
  - **Collaborative Filtering:** Identifies similar user profiles based on numerical features (GPA, skill scores) to suggest paths taken by similar individuals.
- **Smart Input Detection:** Automatically toggles between semantic career lookup and profile-based indexing.
- **Recruiter Insights:** Integrated EDA (Exploratory Data Analysis) for visualizing talent distribution and data trends.
- **Production Ready:** Fully modular backend with a Bootstrap-powered Flask frontend, containerized with Docker.

---

## Tech Stack
- **Backend:** Python, Flask
- **Machine Learning:** Scikit-learn, SentenceTransformers (BERT)
- **Vector Database:** FAISS (Facebook AI Similarity Search)
- **Data Engineering:** Pandas, NumPy
- **Visualization:** Seaborn, Matplotlib
- **Frontend:** HTML5, CSS3 (Bootstrap 5 + Custom styles)
- **DevOps:** Docker

---

##  Project Structure
```text
CAREER_PATH_RECOMMENDATION/
│── analysis/
│   └── eda.py                     # Visualization & Data Analysis
│── app/
│   ├── __init__.py
│   ├── preprocessing.py           # Data cleaning & feature engineering
│   ├── recommender.py             # Collaborative filtering logic
│   └── semantic_search.py         # BERT embeddings + FAISS indexing
│── data/                          # Dataset folder
│── static/
│   └── style.css                  # Custom UI styling
│── templates/
│   └── index.html                 # Main Dashboard (Bootstrap)
│── api.py                         # Flask API entry point
│── Dockerfile                     # Containerization setup
│── requirements.txt               # Dependencies
└── README.md                      # Project Documentation
