# 🏁 Burnout 2025: MotoGP Lap Time Prediction

This repository presents our advanced machine learning pipeline developed for the **Burnout 2025 Datathon**.  
Our objective was to predict **MotoGP riders' average lap times** with high precision by modeling complex racing dynamics using ensemble learning and domain-driven feature engineering.

🔗 [View my Kaggle Notebook](https://www.kaggle.com/code/pranalichitre/notebook911854fcba?scriptVersionId=245457168)

---

## 🚀 Key Highlights

### 🔧 Advanced Data Preprocessing
- ✅ Forward-fill & median imputation for numerical features (e.g., lap times)
- ✅ Mode imputation for categorical features
- ✅ Robust encoding for teams, bikes, weather, and tire types

### 🧠 Domain-Specific Feature Engineering
- **Track Dynamics:**
  - Corner density, average speed per corner, track flow
- **Tire Strategy Modeling:**
  - Grip/durability multipliers, tire mismatch penalties
- **Weather Factors:**
  - Impact of rain, temperature-based time shifts
- **Rider Performance:**
  - Win rate, podium consistency, career momentum index
- **Session Dynamics:**
  - Context-aware multipliers for qualifying vs. race
- **Psychological Grid Effects:**
  - Front-row advantage vs. back-of-grid pressure

---

## 🧪 Sophisticated Feature Selection
- 🔍 Variance thresholding (remove low-informative features)
- 📊 F-test regression for statistical feature relevance
- 🔁 Cross-validated feature importance aggregation

---

## 🤖 Ultra-Ensemble Modeling Architecture
| Model       | Contribution | Notes                               |
|-------------|--------------|-------------------------------------|
| XGBoost     | 35%          | Highly effective with structured data |
| LightGBM    | 30%          | Extremely fast, handles large data well |
| CatBoost    | 25%          | Excellent with categorical features |
| Neural Net  | 10%          | Captures deep feature interactions |

✔ Models are combined using a weighted ensemble for maximum RMSE minimization.

---

## 🛠️ Advanced Post-Processing
- 🌧️ Weather-specific adjustments (rain-induced delays)
- 📈 Session-level corrections (qualifying vs. race)
- ⚠️ Outlier clipping using percentile-based thresholds

---

## 📁 Files in This Repository
| File | Description |
|------|-------------|
| `solution.csv` | Final predictions in correct submission format |
| `README.md` | This documentation |

---

## 👥 Team
- **Pranali Chitre** – Data Science & Modeling Lead  


## 📬 Contact
For any queries or feedback, feel free to reach out via GitHub or connect on [LinkedIn](
https://www.linkedin.com/in/pranali-chitre/).

---

🏆 *"Data meets speed in MotoGP. Our model turns laps into predictions."*
