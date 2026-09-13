# 💻 Laptop Price Exploratory Data Analysis (EDA)

An end-to-end Exploratory Data Analysis (EDA) exploring the pricing mechanics, hardware configurations, and market segmentation of laptops. This project combines statistical validation with domain hardware knowledge to identify key value drivers in laptop pricing.

---

## 📌 Project Overview & Key Findings

- **Primary Numerical Proxy (r = 0.74):** **RAM capacity** exhibits the strongest positive linear correlation with price among continuous variables. Rather than being a standalone cost driver, RAM acts as a strong **proxy indicator** for overall device tier (paired with higher CPUs/GPUs).
- **Hardware Bundling Effect:** Prices are determined by holistic "hardware packages" rather than single components. Performance-oriented categories (**Workstation** & **Gaming**) command the highest average price tiers due to high RAM, dedicated **Nvidia** GPUs, and advanced cooling systems.
- **Premium Display Features:** **4K Ultra HD** resolutions and **Touchscreen** capability significantly elevate baseline device pricing and narrow the price variance toward higher brackets.
- **Market Dominance:** **Intel** dominates CPU market share (~93%), while **Nvidia** leads the performance GPU segment. **SSD** technology serves as the de facto storage standard.

---

## 📊 Analytical Methodology & Workflow

The analysis follows a strict top-down structure to ensure narrative and statistical cohesion:

1. **Univariate & Bivariate Distribution Analysis:** Evaluating CPU/GPU manufacturers, RAM capacities, storage types, and display resolutions.
2. **Categorical Segmentation (`TypeName` Analysis):** Examining market share vs. average price across Gaming, Ultrabook, Workstation, and Notebook types.
3. **Feature Impact Analysis (`Touchscreen` Study):** Assessing mean price differentials and outlier distributions (IQR method) between Touchscreen and Non-Touchscreen models.
4. **High-End Archetype Case Study:** Deep-diving into the dataset's highest-priced model (**Razer Gaming Laptop**) to validate the "Holistic Hardware Bundle" hypothesis (*Gaming + 4K Panel + Touchscreen + 32GB RAM + High-End GPU/CPU*).

---

## 🛠️ Tech Stack & Libraries

- **Language:** Python
- **Data Manipulation:** `pandas`, `numpy`
- **Data Visualization:** `seaborn`, `matplotlib`

---

## 💡 Executive Conclusion

In summary, while **RAM capacity (r = 0.74)** serves as the strongest numerical indicator of a laptop's hardware tier, target market category (`TypeName`), display technologies, and CPU/GPU synergies act as the primary structural **value drivers** of laptop pricing.
