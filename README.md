# 🦠 COVID-19 Operational Tracking & Predictive Modeling Engine

![Python Version](https://img.shields.io/badge/Python-3.10-blue?style=for-the-badge&logo=python&logoColor=white)
![Framework](https://img.shields.io/badge/SDK-Streamlit-FF4B4B?style=for-the-badge&logo=streamlit&logoColor=white)
![Deployment](https://img.shields.io/badge/Container-Docker-2496ED?style=for-the-badge&logo=docker&logoColor=white)
![Project Status](https://img.shields.io/badge/Project-Completed-success?style=for-the-badge)

An interactive, containerized data science framework dedicated to tracking, analyzing, and forecasting global epidemiological trends. This system integrates raw health data streams, advanced exploratory data analysis (EDA), and machine learning time-series modeling to map transmission velocity and predict future caseload curves.

🚀 **Live Active Dashboard Application:** [Interact with the Live Demo on Hugging Face Spaces](https://huggingface.co/spaces/anuragN2107/covid19-trend-forecaster)

---

## 💼 The Strategic Analytics Challenge
During large-scale public health and epidemiological events, healthcare systems, policymakers, and logistics managers require rapid, automated analytics to project future resource demands. Traditional static reporting tools fall short because:
1. **Changing Trajectories:** Pandemic curves shift dynamically due to localized containment strategies, breaking standard linear algorithms.
2. **Resource Allocation Gaps:** Logistics operators require short-term, out-of-sample forward projections to optimize ICU bed capacity, medical supply chains, and staffing levels.

**The Solution:** This end-to-end analytical application isolates historical time-series profiles across 180+ countries. It implements an automated, Bayesian-based **Prophet Additive Regression Model** to capture non-linear trend components alongside weekly seasonality, outputting a reliable 30-day forward prediction window.

---

## 📌 Project Objectives
* **Trend Analysis:** Map global and regional transmission velocities to identify peak infection windows and recovery rate shifts.
* **Feature Engineering:** Structuring time-series indexes to capture rolling averages and smooth out statistical reporting noise.
* **Predictive Modeling:** Deploy robust time-series forecasting models to predict caseloads, aiding proactive clinical resource allocation and policy planning.

---

## 📊 Core Analytical Workflow

### 1. Data Pipeline & Preprocessing
* Raw epidemiological data streams are cleaned and structured, systematically accounting for missing regional reporting intervals and reporting anomalies.
* Chronological time-series indexes are established to calculate rolling averages and eliminate weekday reporting variance.

### 2. Exploratory Data Analysis (EDA)
* Identified peak transmission windows, mutation impact phases, and historical correlation milestones between structural virus vectors.
* Generated interactive visual graphs displaying explicit relationships across active, recovered, confirmed, and mortality metrics.

### 3. Predictive Forecasting Layer
* Configured time-series algorithms explicitly optimized for non-stationary, volatile health data streams.
* Evaluated uncertainty distributions using 95% confidence intervals to maintain risk bounds for short-to-mid-term epidemiological predictions.

---

## 🛠️ Technology Stack & Tools

* **Core Language Engine:** Python 🐍 (v3.10 optimized)
* **Core Modeling Mathematics:** `prophet` (Additive non-linear time-series regression framework)
* **Mathematical Backend Engine:** `cmdstanpy` (Fast Python interface to the Stan C++ backend for Bayesian inference)
* **Data Pipelines & Manipulation:** `pandas`, `numpy` (Resampling, chronological indexing, and data cleaning)
* **Visualization System Layer:** `matplotlib`, `seaborn` (Dynamic real-time generation of trend plots and visual matrices)
* **Application Framework SDK:** `Streamlit` (Web dashboard frontend rendering and interactive state management)
* **Infrastructure Containerization:** `Docker` (Virtualized isolation for environmental reproducibility)
* **Cloud Platform Hosting:** `Hugging Face Spaces` (Isolated, serverless deployment container)

---

## 📋 System Requirements & Dependencies

The application runs inside an isolated **Python 3.10** base environment to match compliance parameters required by the Stan compilation binaries.

### `requirements.txt`
```text
prophet==1.1.6
pandas==2.2.3
matplotlib==3.10.0
seaborn==0.13.2
