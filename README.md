<h1 align="center">House Price Prediction using Machine Learning</h1>
<h2 align="center">IBM Naan Mudhalvan AI Project</h2>

<div align="center">

[![Program](https://img.shields.io/badge/Program-IBM%20Naan%20Mudhalvan-054ADA?style=flat-square&logo=ibm&logoColor=white)](https://naanmudhalvan.tn.gov.in/)
[![Language](https://img.shields.io/badge/Language-Python-3776AB?style=flat-square&logo=python&logoColor=white)](https://www.python.org/)
[![ML](https://img.shields.io/badge/Library-Scikit--Learn-F7931E?style=flat-square&logo=scikitlearn&logoColor=white)](https://scikit-learn.org/)
[![Data](https://img.shields.io/badge/Data-Pandas-150458?style=flat-square&logo=pandas&logoColor=white)](https://pandas.pydata.org/)
[![Model](https://img.shields.io/badge/Model-Linear%20Regression-70a5fd?style=flat-square)](https://github.com/arunkarthi-03)
[![Phases](https://img.shields.io/badge/Phases-5%20Completed-success?style=flat-square)](https://github.com/arunkarthi-03/IBM-Naan-Mudhalvan)
[![Status](https://img.shields.io/badge/Status-Completed-brightgreen?style=flat-square)](https://github.com/arunkarthi-03/IBM-Naan-Mudhalvan)

</div>

---

## 📋 Table of Contents

- [Overview](#-overview)
- [About IBM Naan Mudhalvan](#-about-ibm-naan-mudhalvan)
- [Problem Statement](#-problem-statement)
- [Dataset](#-dataset)
- [Tech Stack](#-tech-stack)
- [Model Architecture](#-model-architecture)
- [Project Phases](#-project-phases)
- [Project Structure](#-project-structure)
- [Getting Started](#-getting-started)
- [Code Walkthrough](#-code-walkthrough)
- [Results](#-results)
- [Author](#-author)

---

## 📄 Overview

This repository contains the complete **5-phase AI project submission** for the **IBM Naan Mudhalvan** initiative — a Government of Tamil Nadu skilling program delivered in partnership with IBM.

The project builds a **House Price Prediction** system using **Supervised Machine Learning (Linear Regression)** trained on the **King County House Sales dataset (`kc_house_data.csv`)**. The model takes key property features as input and predicts the market price of a house.

> 🏠 The system learns patterns from real housing data — bedrooms, bathrooms, living area, floor count, and location (ZIP code) — to output an accurate price estimate.

---

## 🏛️ About IBM Naan Mudhalvan

**Naan Mudhalvan** is a flagship skilling initiative by the **Government of Tamil Nadu**, designed to bridge the gap between academic learning and industry needs. The **IBM AI track** covers core concepts in:

- Artificial Intelligence & Machine Learning
- Python for Data Science
- IBM Cloud & Watson tools
- Real-world project implementation (Phases 1–5)

---

## 🎯 Problem Statement

> **"Given a set of house features, can we accurately predict the sale price of a residential property?"**

Accurately predicting real estate prices is a critical challenge for buyers, sellers, banks, and urban planners. Manual estimation is subjective and unreliable. This project automates price prediction using a **data-driven Linear Regression model** trained on historical King County housing data.

---

## 📊 Dataset

| Property | Details |
|:---|:---|
| **Name** | King County House Sales Dataset |
| **File** | `kc_house_data.csv` |
| **Region** | King County, Washington, USA |
| **Features Used** | `bedrooms`, `bathrooms`, `sqft_living`, `sqft_lot`, `floors`, `zipcode` |
| **Target Variable** | `price` (USD) |
| **Split** | 80% Training / 20% Testing |

### Feature Description

| Feature | Type | Description |
|:---|:---:|:---|
| `bedrooms` | Integer | Number of bedrooms |
| `bathrooms` | Float | Number of bathrooms |
| `sqft_living` | Integer | Square footage of living space |
| `sqft_lot` | Integer | Square footage of the lot |
| `floors` | Float | Number of floors |
| `zipcode` | Integer | ZIP code of the property location |
| `price` ⭐ | Float | **Target — Sale price in USD** |

---

## 🛠️ Tech Stack

| Tool / Library | Purpose |
|:---|:---|
| ![Python](https://img.shields.io/badge/Python-3776AB?style=flat-square&logo=python&logoColor=white) | Core programming language |
| ![Pandas](https://img.shields.io/badge/Pandas-150458?style=flat-square&logo=pandas&logoColor=white) | Data loading & manipulation |
| ![Scikit-Learn](https://img.shields.io/badge/Scikit--Learn-F7931E?style=flat-square&logo=scikitlearn&logoColor=white) | Linear Regression model & train/test split |
| ![Anaconda](https://img.shields.io/badge/Anaconda-44A833?style=flat-square&logo=anaconda&logoColor=white) | Environment & package management |
| ![Jupyter](https://img.shields.io/badge/Jupyter-F37626?style=flat-square&logo=jupyter&logoColor=white) | Interactive development & documentation |

---

## 🧠 Model Architecture

```
┌────────────────────────────────────────────────────────────────┐
│                    INPUT FEATURES (X)                          │
│  bedrooms │ bathrooms │ sqft_living │ sqft_lot │ floors │ zip  │
└────────────────────────┬───────────────────────────────────────┘
                         │
              ┌──────────▼──────────┐
              │   Data Preprocessing│
              │  pandas.read_csv()  │
              │  Feature Selection  │
              └──────────┬──────────┘
                         │
              ┌──────────▼──────────┐
              │   Train/Test Split  │
              │  80% Train / 20%    │
              │  random_state = 42  │
              └──────────┬──────────┘
                         │
              ┌──────────▼──────────┐
              │  Linear Regression  │
              │  model.fit(X_train, │
              │            y_train) │
              └──────────┬──────────┘
                         │
              ┌──────────▼──────────┐
              │    Prediction       │
              │  model.predict(X)   │
              └──────────┬──────────┘
                         │
              ┌──────────▼──────────┐
              │    Evaluation       │
              │  R² Score (model    │
              │  .score(X_test,     │
              │   y_test))          │
              └─────────────────────┘
```

---

## 📅 Project Phases

The IBM Naan Mudhalvan submission is structured across **5 phases**, each building on the previous:

| Phase | File | Description |
|:---:|:---|:---|
| 📘 **Phase 1** | `AI_Phase 1.pptx` | Problem definition, objectives, and initial ideation |
| 📗 **Phase 2** | `AI_Phase 2.pptx` | Dataset selection, feature analysis & EDA planning |
| 📙 **Phase 3** | `AI_Phase 3.pptx / .pdf` | Model design, algorithm selection & data preprocessing |
| 📕 **Phase 4** | `AI_Phase 4.pdf` | Model training, evaluation & results |
| 📓 **Phase 5** | `AI_Phase 5.pdf` | Final report, conclusions & future enhancements |

<details>
<summary><strong>📘 Phase 1 — Problem Definition & Ideation</strong></summary>

<br/>

> Identified the real-world problem of inaccurate manual house price estimation. Defined project objectives, scope, and expected outcomes. Proposed using a regression-based ML model to bring data-driven prediction to real estate.

</details>

<details>
<summary><strong>📗 Phase 2 — Dataset & EDA Planning</strong></summary>

<br/>

> Selected the **King County House Sales dataset** as the training source. Identified key features influencing house price. Planned Exploratory Data Analysis (EDA) steps to understand data distributions and correlations.

</details>

<details>
<summary><strong>📙 Phase 3 — Model Design & Preprocessing</strong></summary>

<br/>

> Finalized **Linear Regression** as the model of choice. Performed feature selection — narrowed to 6 most impactful attributes. Implemented data loading with `pandas` and prepared training/test splits using `sklearn`.

</details>

<details>
<summary><strong>📕 Phase 4 — Training, Prediction & Evaluation</strong></summary>

<br/>

> Trained the Linear Regression model on 80% of data. Generated predictions on the test set. Evaluated model accuracy using the **R² (coefficient of determination)** score. Demonstrated a working prediction for a new, unseen house configuration.

</details>

<details>
<summary><strong>📓 Phase 5 — Final Report & Conclusions</strong></summary>

<br/>

> Compiled the complete project journey into a formal report. Documented results, limitations, and proposed future enhancements — including advanced models (Random Forest, XGBoost) and a web-based deployment interface.

</details>

---

## 📁 Project Structure

```
IBM-Naan-Mudhalvan/
│
├── AI_Phase 1.pptx        # Phase 1 — Problem definition & ideation
├── AI_Phase 2.pptx        # Phase 2 — Dataset analysis & EDA
├── AI_Phase 3.pptx        # Phase 3 — Model design & preprocessing
├── AI_Phase 3.pdf         # Phase 3 — PDF submission
├── AI_Phase 4.pdf         # Phase 4 — Training, prediction & evaluation
├── AI_Phase 5.pdf         # Phase 5 — Final report & conclusions
│
├── kc_house_data.csv      # Dataset (King County House Sales)  ← add this
├── house_price_model.py   # Main Python ML script              ← add this
└── README.md              # Project documentation
```

---

## 🚀 Getting Started

### Prerequisites

```bash
pip install pandas scikit-learn
```

Or with Anaconda (recommended):
```bash
conda install pandas scikit-learn
```

### Run the Model

1. **Clone the repository**
   ```bash
   git clone https://github.com/arunkarthi-03/IBM-Naan-Mudhalvan.git
   cd IBM-Naan-Mudhalvan
   ```

2. **Place the dataset** — download `kc_house_data.csv` and put it in the project root.

3. **Run the script**
   ```bash
   python house_price_model.py
   ```

---

## 💻 Code Walkthrough

```python
from sklearn.model_selection import train_test_split
from sklearn.linear_model import LinearRegression
import pandas as pd

# 1. Load the dataset
data = pd.read_csv('kc_house_data.csv')

# 2. Select features and target
features = ['bedrooms', 'bathrooms', 'sqft_living', 'sqft_lot', 'floors', 'zipcode']
X = data[features]
y = data['price']

# 3. Split into training (80%) and testing (20%) sets
X_train, X_test, y_train, y_test = train_test_split(X, y, test_size=0.2, random_state=42)

# 4. Create and train the Linear Regression model
model = LinearRegression()
model.fit(X_train, y_train)

# 5. Evaluate the model
score = model.score(X_test, y_test)
print(f"Model R² Score: {score:.4f}")

# 6. Predict the price of a new house
new_house = pd.DataFrame({
    'bedrooms': [2], 'bathrooms': [2.5],
    'sqft_living': [600], 'sqft_lot': [600],
    'floors': [2], 'zipcode': [98008]
})
predicted_price = model.predict(new_house)
print(f"Predicted Price: ${predicted_price[0]:,.2f}")
```

---

## 📈 Results

| Metric | Value |
|:---|:---|
| **Algorithm** | Linear Regression |
| **Evaluation Metric** | R² Score (Coefficient of Determination) |
| **Train / Test Split** | 80% / 20% |
| **Random State** | 42 |
| **Sample Prediction** | 2 bed / 2.5 bath / 600 sqft / ZIP 98008 → model output |

> 📌 **R² Score** measures how well the model explains variance in house prices. A score closer to **1.0** means near-perfect prediction accuracy.

---

## 👤 Author

<div align="center">

**Karthikeyan Arun Kumar**
B.E. Electronics & Communication Engineering
Panimalar Institute of Technology, Chennai | Anna University | 2025

[![GitHub](https://img.shields.io/badge/GitHub-arunkarthi--03-181717?style=flat-square&logo=github&logoColor=white)](https://github.com/arunkarthi-03)
[![Email](https://img.shields.io/badge/Email-arunkarthi4761%40gmail.com-D14836?style=flat-square&logo=gmail&logoColor=white)](mailto:arunkarthi4761@gmail.com)

</div>

---

<div align="center">

*"Turning data into decisions — one feature at a time."* 🤖

⭐ **If this project was useful, drop a star!** ⭐

</div>
