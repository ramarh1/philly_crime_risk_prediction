# Predicting Crime Risk Using 311 Requests and Historical Data

**Author:** Ramar Huntley

**Project Type:** Data Analysis / Predictive Modeling

**Tools:** Python, Pandas, Scikit-learn, Jupyter, (optional: Power BI / Tableau)

** If you found this project interesting, feel free to star the repo! **

---

## Project Overview

This project explores whether **311 service requests** (non-emergency city service data) can help predict **crime risk patterns** across Philadelphia neighborhoods.

By combining **public safety data** with  **operational service data** , this analysis aims to uncover relationships between environmental conditions and crime activity.

The final output is a predictive model that estimates  **crime risk by location and time window** , supporting more informed resource allocation and planning decisions.

---

## Objective

The main goal of this project is to:

* Predict the **likelihood of crime incidents**
* Identify **high-risk areas and time periods**
* Determine whether **311 activity improves prediction accuracy**

---

## Data Sources

### 1. Crime Incidents Data

* Source: OpenDataPhilly
* Description: Records of reported crimes including:
  * Crime type
  * Date and time
  * Location (neighborhood / district)

---

### 2. 311 Service Requests Data

* Source: OpenDataPhilly
* Description: Requests submitted by residents, such as:
  * Graffiti removal
  * Abandoned vehicles
  * Sanitation issues

---

## Methodology

### 1. Data Preparation

* Combined multi-year datasets (2018–2024)
* Handled missing values and inconsistent formats
* Standardized time and location fields

---

### 2. Data Aggregation

Both datasets were aggregated to a shared level:

* **Geography:** Neighborhood / district / ZIP
* **Time:** Daily (or hourly, depending on implementation)

This ensured compatibility and prevented duplication during merging.

---

### 3. Feature Engineering

Key features included:

* Time-based features (hour, day, weekend)
* Crime history (rolling averages, past trends)
* 311 activity (request volume, request types)
* Lag features (previous time windows)

---

### 4. Modeling

Models evaluated:

* Logistic Regression (baseline)
* Random Forest
* Gradient Boosting (optional)

Approach:

* Time-based train/test split
* Evaluation using accuracy, precision/recall, and ROC-AUC

---

## Key Insights

* Certain neighborhoods show consistent **high-risk time windows**
* 311 request volume can act as a **leading indicator** for certain crime types
* Environmental and service-related issues may correlate with crime patterns

---

## Business Value

This project demonstrates how combining datasets can support:

* **Proactive resource allocation**
* **Operational planning**
* **Urban data-driven decision-making**

---

## Limitations & Ethics

* Predictions are made at an  **aggregate level** , not individual predictions
* Data may contain **reporting bias**
* Correlation does not imply causation
* Results should not be used for profiling or targeting individuals

---

## Project Structure

```
philly-crime-risk-prediction/
│
├── data/
│   ├── raw/
│   ├── processed/
│
├── notebooks/
│   ├── 01_eda.ipynb
│   ├── 02_data_cleaning.ipynb
│   ├── 03_feature_engineering.ipynb
│   ├── 04_modeling.ipynb
│   ├── 05_evaluation.ipynb
│
├── outputs/
│   ├── charts/
│   ├── results/
│
├── README.md
```

---

## Future Improvements

* Incorporate weather data
* Add demographic or census data
* Improve spatial modeling (GIS features)
* Deploy an interactive dashboard

---

## Conclusion

This project highlights the value of integrating **operational data (311 requests)** with **historical crime data** to better understand urban risk patterns.

It demonstrates end-to-end data workflow skills including:

* Data cleaning
* Feature engineering
* Predictive modeling
* Insight generation

---

## Contact

If you'd like to connect or discuss this project:

**Ramar Huntley**

[Title]

[Email]

---
