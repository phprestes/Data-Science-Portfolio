# 🤖 Machine Learning & Data Science Portfolio

Welcome to my machine learning and data science repository! This portfolio aggregates the projects where the core of the work is data — modeling it, moving it, or reasoning about it. It spans undergraduate research, course projects, hackathons, and personal tools built while pursuing my **B.S. in Computer Science** at the **University of São Paulo (USP) - ICMC**.

The portfolio is organized by area rather than by date. Each project includes a brief description, core techniques, technology stack, and an interactive repository card.

> For the full academic record organized by semester and course, see [Undergraduate Projects Portfolio](https://github.com/phprestes/Undergraduate-ICMC-USP).

---

## 📌 Quick Navigation
- [Graph Machine Learning & Deep Learning](#-graph-machine-learning--deep-learning)
- [Natural Language Processing & Embeddings](#-natural-language-processing--embeddings)
- [Evolutionary Computation & Optimization](#-evolutionary-computation--optimization)
- [Network Science & Graph Analysis](#-network-science--graph-analysis)
- [Statistics, Simulation & Probability](#-statistics-simulation--probability)
- [Data Engineering & Pipelines](#-data-engineering--pipelines)
- [LLM & AI Applications](#-llm--ai-applications)
- [Numerical & Mathematical Foundations](#-numerical--mathematical-foundations)

---

## 🔹 Graph Machine Learning & Deep Learning

## 🧠 Undergraduate Research (Iniciação Científica)
* **Project Name:** CNES — Network Structure and Medical Resource Acquisition
* **Description:** A full data and modeling pipeline over the microdata of **CNES** (Brazil's National Registry of Health Establishments, DATASUS), predicting medical equipment acquisition between annual snapshots. The study compares three representations of the *same* label — no structure (tabular baselines), relational structure (a heterogeneous GNN over the registry schema), and geographic structure — so the numbers are directly comparable. The unit of analysis is the **transition** `t → t+1` rather than the row, because a CNES snapshot is current-state, not an event log, making its date column right-censored. Ten annual snapshots (2017–2026) yield nine transitions across a four-layer medallion architecture, with an isolated second pipeline for a 440 GB / 2× RTX A6000 cluster. Every run emits a reproducible artifact package — weights, provenance manifest, node/item index, and per-example scores — so metrics can be recomputed and audited without a GPU or the raw data. Advised by **Alexandre C. B. Delbem** and **Eric K. Tokuda**.
* **Techniques:** Graph Neural Networks (heterogeneous, temporal), Relational Deep Learning (RelBench), Link Prediction, Tabular Gradient Boosting Baselines, Medallion Data Architecture (raw → intermediate → primary → feature), Temporal Splitting & Leakage Control, Ranking Metrics (Average Precision, AUC via Mann-Whitney, MAP@k), Seed-Variance Estimation, Memory-Bounded Execution (cgroups), Checkpointed & Resumable Training, Reproducible Artifact Packaging, Schema-as-Documentation (single source of truth parsed at import).
* **Stack:** `Python 3.12`, `PyTorch`, `PyTorch Geometric`, `RelBench`, `scikit-learn`, `DuckDB`, `Parquet`, `PyArrow`, `SciPy`, `Jupyter Notebook`, `pytest`, `uv`, `Make`, `CUDA`
* **Repository:**

  <a href="https://github.com/phprestes/DATASUS-Resource-Prediction-GNN">
    <img src="https://gh-card.dev/repos/phprestes/DATASUS-Resource-Prediction-GNN.svg" alt="Repo Card" />
  </a>

---

## 🔹 Natural Language Processing & Embeddings

## 📚 Evolutionary Systems Applied to Robotics
* **Project Name:** Genetic Embeddings
* **Description:** An investigation into applying Evolutionary/Genetic Algorithms to Natural Language Processing — first predicting the next word in a sentence, then evolving text embeddings from scratch and benchmarking them against Word2Vec. The study concludes that GAs mainly capture syntactic patterns and degrade geometrically as vocabulary size grows.
* **Techniques:** Genetic Algorithms (Selection, Crossover, Mutation), Fitness Function Design, Word Embeddings, Word2Vec Comparison, Vector Space Geometry Analysis, Natural Language Processing, Convergence & Efficiency Analysis.
* **Stack:** `Python`, `Jupyter Notebook`, `Gensim`, `NumPy`
* **Repository:**

  <a href="https://github.com/phprestes/Genetic-Embeddings">
    <img src="https://gh-card.dev/repos/phprestes/Genetic-Embeddings.svg" alt="Repo Card" />
  </a>

---

## 🔹 Evolutionary Computation & Optimization

## 📚 Evolutionary Systems Applied to Robotics
* **Project Name:** N-SAT Genetic Solver
* **Description:** A genetic-algorithm approach to the Boolean Satisfiability Problem (SAT) — the first problem proven NP-complete. Candidate assignments are encoded as chromosomes and scored by how many clauses they satisfy, evolved through single-point crossover against the best individual and a 5% per-gene mutation rate, with live plotting of the fitness evolution.
* **Techniques:** Genetic Algorithms, Chromosome Encoding, Fitness Evaluation, Single-Point Crossover, Mutation Rates, Metaheuristic Search, NP-Complete Problems, Boolean Satisfiability, Real-Time Data Plotting.
* **Stack:** `C`, `C++`, `Python`, `Tkinter`, `GNUplot`, `Shell/Bash Script`
* **Repository:**

  <a href="https://github.com/phprestes/N-SAT-Genetic">
    <img src="https://gh-card.dev/repos/phprestes/N-SAT-Genetic.svg" alt="Repo Card" />
  </a>

---

## 🔹 Network Science & Graph Analysis

## 📚 Complex Networks
* **Project Name:** Complex Networks Problem Sets (SME0130)
* **Description:** Jupyter Notebook solutions to the course's problem sets, analyzing real-world network datasets (*lesmis*, *powergrid*, *euroroad*, *usairport*, *hamsterster*, *jazz*) through topological measures, centrality metrics, community detection, network classification, and epidemic dynamics.
* **Techniques:** Degree Distribution & Moments, Shannon Entropy of Degree Distribution, Transitivity & Clustering Coefficients, Centrality Measures (Eigenvector, Betweenness, Closeness, k-core), Pearson & Spearman Correlations, Community Detection, Supervised Network Classification, Epidemic Spreading Models.
* **Stack:** `Python`, `Jupyter Notebook`, `NetworkX`, `graph-tool`, `NumPy`, `SciPy`, `pandas`, `scikit-learn`, `Matplotlib`, `seaborn`, `EoN`
* **Repository:**

  <a href="https://github.com/phprestes/Redes-Complexas">
    <img src="https://gh-card.dev/repos/phprestes/Redes-Complexas.svg" alt="Repo Card" />
  </a>

---

## 🔹 Statistics, Simulation & Probability

## 📚 Statistics
* **Project Name:** Statistical Simulation Projects (SME0123)
* **Description:** Two computational simulation projects tackling probability problems: an M/M/r/4 finite-capacity queue analyzed as a Markov chain with two competing server-allocation strategies, and the classical geometric-probability question of whether a tetrahedron formed by four random points on a sphere contains its center.
* **Techniques:** Monte Carlo Simulation, Markov Chains & Queueing Theory, Hypothesis Testing, Chi-Squared Uniformity Test, Confidence Intervals, Random Point Generation on Spheres, 3D Interactive Visualization.
* **Stack:** `Python`, `Jupyter Notebook`, `NumPy`, `SciPy`, `Plotly`
* **Repository:**

  <a href="https://github.com/phprestes/Estatistica">
    <img src="https://gh-card.dev/repos/phprestes/Estatistica.svg" alt="Repo Card" />
  </a>

---

## 🔹 Data Engineering & Pipelines

## 📚 Advanced Algorithms and Applications
* **Project Name:** PT-Wikipedia Graph Builder
* **Description:** A data pipeline that processes official Portuguese Wikipedia dumps into a Neo4j graph of article-to-article links, using SQLite as an on-disk intermediate cache for memory-efficient ID-to-title resolution. Built as the outreach demo for **ICMC de Portas Abertas**, teaching high-school students how the Wikipedia Game reduces to a shortest-path problem on graphs.
* **Techniques:** Large Dump Processing (`mwsql`), Graph Databases & Modeling, Shortest Path Algorithms, Batch Ingestion & Throughput Tuning, Checkpointing/Resumable Pipelines, Disk-Based Caching, Memory-Constrained ETL.
* **Stack:** `Python`, `Neo4j`, `SQLite`, `mwsql`
* **Repository:**

  <a href="https://github.com/phprestes/Wikipedia-Graph">
    <img src="https://gh-card.dev/repos/phprestes/Wikipedia-Graph.svg" alt="Repo Card" />
  </a>

## 💡 Personal Project
* **Project Name:** ICMC Grad Maker — Course Schedule Data Pipeline
* **Description:** A platform that helps ICMC-USP students assemble their semester timetable without schedule conflicts. The data side is a two-source extraction pipeline with intelligent orchestration: a Selenium scraper reads the official JúpiterWeb portal when the semester's class offerings are published, and an LLM-based parser falls back to the preliminary PDFs when they are not, with a merge step consolidating either path into a single clean `courses.json` consumed by a React SPA.
* **Techniques:** Web Scraping & Browser Automation, PDF Text Extraction, LLM-Assisted Structured Extraction, Pipeline Orchestration with Source Fallback, Data Consolidation & Normalization, Schedule Conflict Detection, Static Data Consumption (no runtime API calls).
* **Stack:** `Python`, `Selenium`, `BeautifulSoup`, `pdfplumber`, `google-genai` (Gemini), `pandas`, `uv`, `JavaScript`, `React`, `Vite`
* **Repository:**

  <a href="https://github.com/phprestes/ICMC-Grad-Maker">
    <img src="https://gh-card.dev/repos/phprestes/ICMC-Grad-Maker.svg" alt="Repo Card" />
  </a>

## 📚 Docker Course (Asimov Academy)
* **Project Name:** Docker Datalake Extractor
* **Description:** A Docker study project that simulates data extraction for a datalake: a Python application queries the public DummyJSON API on a schedule and saves products and carts as timestamped JSON files, with cron running inside the container.
* **Techniques:** Containerization (Multi-Stage Dockerfile), Docker Volumes, Scheduled Execution (cron), Rotating Logs, HTTP API Consumption, Command-Line Argument Parsing.
* **Stack:** `Python`, `Docker`, `Cron`, `Requests`, `Shell/Bash Script`
* **Repository:**

  <a href="https://github.com/phprestes/Docker-Datalake-Extractor">
    <img src="https://gh-card.dev/repos/phprestes/Docker-Datalake-Extractor.svg" alt="Repo Card" />
  </a>

## 📚 SAMPA Course — MLOps Foundations
* **Project Name:** SAMPA — ML Systems Engineering Exercises
* **Description:** The theoretical foundation for MLOps systems: ten exercises from the SAMPA course on engineering Machine Learning systems (based on *Machine Learning in Production: From Models to Products* and the Carnegie Mellon course of the same name), evolving a single case-study system from objectives to performance modeling.
* **Techniques:** Objectives & Requirements Specification, Failure Modes, Fault Tree Analysis (FTA), Measurement & Model Quality, Validation Automation, System Architecture (Edge Computing / TinyML), C4 Diagrams, ML Pipelines (Training, Deployment, Data Ingestion), Monitoring, Performance Modeling.
* **Stack:** `Markdown`, `C4 Model`
* **Repository:**

  <a href="https://github.com/phprestes/Curso-SAMPA">
    <img src="https://gh-card.dev/repos/phprestes/Curso-SAMPA.svg" alt="Repo Card" />
  </a>

---

## 🔹 LLM & AI Applications

## 🏆 Hackathon — Tractian @ SECOMP UFSCar XII
* **Project Name:** Manutec — Voice-Driven Maintenance Assistant
* **Description:** A maintenance-management application built for the Tractian hackathon. Field technicians upload a voice recording of their instructions; the system transcribes it and turns free-form speech (or typed text) into an actionable task checklist through the GPT API. It also suggests and tracks which tools are in use, by whom, and when.
* **Techniques:** Speech-to-Text Transcription, LLM Prompt Design for Structured Output, Audio Preprocessing & Format Handling, Task Extraction from Unstructured Text, Tool Recommendation, Desktop GUI Development.
* **Stack:** `Python`, `OpenAI GPT API`, `Pydub`, `ffmpeg`, `Tkinter`, `PIL`
* **Repository:**

  <a href="https://github.com/phprestes/Hackaton-Manutec">
    <img src="https://gh-card.dev/repos/phprestes/Hackaton-Manutec.svg" alt="Repo Card" />
  </a>

## 🏆 Hackathon — BTG @ SEMCOMP
* **Project Name:** FinSense — WhatsApp Finance Agent (BTG Hackathon)
* **Description:** A LangChain-based financial agent that simulates and extends BTG Pactual's WhatsApp assistant (Finanças+), adding card management, savings goals ("caixinhas"), category budgets, spend alerts and expense charts, delivered over WhatsApp via the Twilio API. Built as a collaborator for the BTG hackathon at SEMCOMP.
* **Techniques:** LangChain Agent / Tool-Calling, WhatsApp Integration (Twilio API), Webhook Tunneling (Ngrok), Structured Output Validation (Pydantic), Budget & Spend Alerting, Data Visualization (Matplotlib).
* **Stack:** `Python`, `LangChain`, `Twilio API`, `Pydantic`, `Matplotlib`, `Ngrok`
* **Repository:**

  <a href="https://github.com/bielpieroli/HACKATHON_BTG_SEMCOMP">
    <img src="https://gh-card.dev/repos/bielpieroli/HACKATHON_BTG_SEMCOMP.svg" alt="Repo Card" />
  </a>

---

## 🔹 Numerical & Mathematical Foundations

## 📚 Linear Algebra and Applications
* **Project Name:** Linear Algebra Exercises & Applied Projects (SME0142)
* **Description:** A notebook collection working through the course's exercise sets plus a practical assignment and a final project, connecting linear algebra theory to computational applications — the algebra that underpins dimensionality reduction, least-squares fitting, and the linear layers of neural networks.
* **Techniques:** Vector Spaces & Linear Transformations, Matrix Factorizations, Eigenvalues & Eigenvectors, Orthogonality & Projections, Least Squares, Numerical Linear Algebra.
* **Stack:** `Python`, `Jupyter Notebook`, `NumPy`, `Matplotlib`
* **Repository:**

  <a href="https://github.com/phprestes/Algebra-Linear">
    <img src="https://gh-card.dev/repos/phprestes/Algebra-Linear.svg" alt="Repo Card" />
  </a>

## 📚 Numerical Calculus
* **Project Name:** Numerical Methods Notebooks (SME104)
* **Description:** A series of Jupyter Notebooks implementing and explaining classical numerical methods, pairing theoretical derivations with executable code and visualizations for each topic — including the floating-point error analysis and iterative solvers that sit underneath every numerical optimizer.
* **Techniques:** Numeric Base Conversion, Floating-Point Arithmetic (Rounding & Truncation Errors), Root Finding (Bisection, Newton-Raphson, Secant), Direct Solvers for Linear Systems (Gaussian Elimination, LU Factorization), Nonlinear Systems (Newton's Method).
* **Stack:** `Python`, `Jupyter Notebook`, `NumPy`, `Matplotlib`
* **Repository:**

  <a href="https://github.com/phprestes/Calculo-Numerico">
    <img src="https://gh-card.dev/repos/phprestes/Calculo-Numerico.svg" alt="Repo Card" />
  </a>
