# 🌍 Impact of Climate Change on Global Food Supply

> **Forecasting crop yields under shifting climate conditions using XGBoost, Decision Tree, and LSTM.**
> 
> Top model: **XGBoost with R² = 0.982**. Projected **15% yield sensitivity** under adverse climate scenarios using SHAP-based interpretability.

[![Python](https://img.shields.io/badge/Python-3.9-blue?logo=python&logoColor=white)](https://www.python.org/)
[![XGBoost](https://img.shields.io/badge/XGBoost-Top_Model-orange)](https://xgboost.readthedocs.io/)
[![TensorFlow](https://img.shields.io/badge/TensorFlow-LSTM-FF6F00?logo=tensorflow)](https://www.tensorflow.org/)
[![SHAP](https://img.shields.io/badge/SHAP-Interpretability-purple)](https://shap.readthedocs.io/)
[![scikit-learn](https://img.shields.io/badge/scikit--learn-1.x-orange?logo=scikit-learn)](https://scikit-learn.org/)

---

## 📌 About This Project

As climate-driven events such as droughts, floods, and heatwaves become more frequent, their impact on food systems is growing. This project investigates how climate change affects global food security by analyzing historical crop yield, climate, and environmental data using machine learning.

The goal: build predictive models that forecast crop yields based on environmental variables, so communities and policymakers can plan for food resilience before yields collapse, not after.

**This is a solo end-to-end data science project**, from data merging to model deployment and interpretability.

---

## 🎯 What I Did

**Data Engineering**
- Merged **4 real-world datasets** (crop yield, rainfall, pesticides, temperature) from FAO and World Bank
- Cleaned and consolidated **37,500+ rows** across **104 countries** and **23 years**
- Applied one-hot encoding for categorical features and MinMaxScaler for numerical normalization

**Modeling**
- Built and compared **3 models**: XGBoost, Decision Tree, and LSTM (TensorFlow)
- Hyperparameter tuning with **GridSearchCV** (XGBoost, Decision Tree) and **KerasTuner** (LSTM)
- Evaluated using R² and RMSE on held-out test data

**Interpretability & Insight**
- Applied **SHAP** to identify the strongest yield predictors (rainfall and temperature emerged as top features)
- Projected a **15% yield sensitivity** under adverse climate scenarios
- Translated technical results into actionable insight for food-security planning

---

## 🛠️ Tech Stack

| Layer | Tools |
|---|---|
| **Language** | Python |
| **Data Wrangling** | pandas, NumPy |
| **Modeling** | XGBoost, scikit-learn, TensorFlow (LSTM) |
| **Tuning** | GridSearchCV, KerasTuner |
| **Interpretability** | SHAP |
| **Visualization** | Matplotlib, Seaborn |
| **Environment** | Jupyter Notebook |

---

## 📊 Results

| Model | R² Score | Notes |
|---|---|---|
| **XGBoost** | **0.982** ✅ | Best performer. Captured non-linear relationships effectively. |
| Decision Tree | 0.981 | High accuracy but more prone to overfitting. |
| LSTM | 0.774 | Captured temporal patterns; lower accuracy due to limited sequence depth. |

**XGBoost was selected as the final production model** due to its superior accuracy and robust handling of non-linear, mixed-feature data. Rainfall and temperature surfaced as the most influential predictors, with the model projecting a **15% drop in yield under adverse climate conditions**.

---

## 🧾 Datasets

| Source | Used For |
|---|---|
| **FAOSTAT** | Crop yield, pesticide use, population (1970 to 2023) |
| **World Bank** | Annual precipitation and temperature |
| **IPCC Reports** | Global climate indicators and emissions context |

---

## 📁 Repository Structure

| File | Description |
|---|---|
| `climate_food_supply_analysis.ipynb` | Full analysis notebook (EDA → modeling → SHAP) |
| `PesticidesNew.csv` | Pesticide use dataset |
| `RainfallNew.csv` | Rainfall dataset |
| `YieldNew.csv` | Crop yield dataset |
| `Population.csv` | Population dataset |
| `temp.csv` | Temperature dataset |
| `.gitignore` | Git ignore rules |
| `README.md` | This file |

---

## 🚀 How To Run Locally

```bash
git clone https://github.com/AyushiButani/Impact-of-Climate-on-Global-Food-Supply.git
cd Impact-of-Climate-on-Global-Food-Supply

# (Recommended) Create a virtual environment
python -m venv venv
source venv/bin/activate    # macOS/Linux
# venv\Scripts\activate     # Windows

# Install dependencies
pip install pandas numpy scikit-learn xgboost tensorflow shap matplotlib seaborn jupyter

# Launch the notebook
jupyter notebook climate_food_supply_analysis.ipynb
```

---

## 💡 What I'd Build Next

- Incorporate satellite imagery and soil-quality data for finer-grained yield prediction
- Extend the model with region-specific and crop-specific submodels
- Experiment with Transformer-based architectures for richer temporal modeling
- Integrate near-real-time data feeds (IoT sensors) for precision agriculture pipelines

---

## 📫 Contact

I'm currently looking for full-time Data Analyst and Data Science roles in the US.

- 📧 **Email:** ayushibutani9@gmail.com
- 💼 **LinkedIn:** [linkedin.com/in/ayushi-butani](https://www.linkedin.com/in/ayushi-butani/)
- 🌐 **GitHub:** [github.com/AyushiButani](https://github.com/AyushiButani)
- 📊 **Tableau Public:** [public.tableau.com/app/profile/ayushibutani](https://public.tableau.com/app/profile/ayushibutani)
