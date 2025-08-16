# 📊 Term Deposit Prediction – Exploratory Data Analysis (EDA)

This repository contains an Exploratory Data Analysis (EDA) of the **Bank Marketing Dataset** (`banking_data.csv`).  
The goal is to explore customer demographics, financial features, and marketing interactions to understand factors influencing **term deposit subscription**.

---

## 📂 Repository Contents
- `banking_data.csv` – Dataset file (Bank Marketing data)  
- `notebooks/` – Jupyter Notebook(s) with full EDA code  
- `01.pdf` – Colab-exported notebook (EDA with answers and visualizations)  

---

## 📑 Dataset Description
- **Rows:** ~45,000 (bank client records)  
- **Features:**  
  - `age`, `job`, `marital`, `education`, `default`  
  - `balance`, `housing`, `loan`  
  - `contact`, `day`, `month`, `duration`  
  - `campaign`, `pdays`, `previous`, `poutcome`  
  - Target variable: **`y`** (whether the client subscribed to a term deposit)  

---

## 🔍 EDA Highlights

1. **Client Demographics**
   - Most clients are **30–40 years old**.  
   - Common job: **blue-collar**; least common: *student* and *unknown*.  
   - Majority are **married (60%)**, then single (28%) and divorced (12%).  
   - Most clients have **secondary education**.

2. **Financial & Credit Behavior**
   - Very few clients (~1.5%) have credit in default.  
   - **Balances are right-skewed** – most clients maintain low balances.  
   - Housing loans are more common than personal loans.  

3. **Marketing & Contact**
   - Majority contacted via **cellular**; few via telephone.  
   - Campaigns were concentrated in **May** and **July**.  
   - Most calls are short; majority of clients contacted **1–3 times** in a campaign.  
   - Most values in `pdays` = -1 → no previous contact.  
   - Previous campaign outcomes are mostly *unknown* or *failure*.  

4. **Subscription Target (y)**
   - Dataset is **imbalanced**: majority did **not subscribe** to term deposit.  
   - Correlation heatmaps (numeric + encoded categorical features) highlight potential predictors.  

---

## 🚀 How to Run

1. Clone the repo:
   ```bash
   git clone https://github.com/<your-username>/<repo-name>.git
   cd <repo-name>
```

2. Install dependencies:
```bash
pip install pandas numpy matplotlib seaborn scikit-learn
```

3. Open the notebook:
```bash
jupyter notebook notebooks/term_deposit_eda.ipynb
```
📈 **Key Insights**

Age, job type, marital status, and education strongly shape customer distribution.

Financial status (balance, loans) is skewed; majority are low-balance holders.

Marketing strategy relies heavily on short-duration cellular calls in limited months.

The dataset suffers from class imbalance (very few subscribers).

Feature correlations suggest multiple categorical + numeric variables are relevant for prediction.

📜 **License**

This project is licensed under the MIT License.

👤 **Author**

Manish Lakhode, Contact:
**For questions or contributions, please get in touch with manishlakhode9865@gmail.com**