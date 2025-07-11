# 🧪 Ecommerce A/B Testing Analysis

This project explores an A/B testing scenario using real-world ecommerce data from Kaggle. The objective is to determine whether a newly designed landing page leads to a higher conversion rate compared to the existing version.

📌 Dataset Source:  
[Kaggle - Ecommerce A/B Testing (2022)](https://www.kaggle.com/datasets/putdejudomthai/ecommerce-ab-testing-2022-dataset1/data)

---

## 📁 Project Structure

```
ecommerce_ab_test/
├── data/
│ ├── raw/ # Raw dataset from Kaggle
│ └── processed/ # Cleaned & transformed datasets
│
├── notebooks/
│ ├── 01_data_eda.ipynb # Exploratory Data Analysis
│ ├── 02_ab_test_analysis.ipynb # Statistical A/B test (z-test, chi2)
│ ├── 03_report.ipynb # Summary insights and conclusions
│ └── 04_subgroup_analysis.ipynb # Country-wise subgroup testing
│
├── outputs/
│ └── figures/ # Visualization images
│
├── reports/
│ └── final_report.pdf # Optional exportable summary
│
├── requirements.txt # Python dependencies
└── README.md # Project overview
```


---

## 🎯 Objective

To evaluate whether a newly implemented landing page results in a statistically significant improvement in conversion rate versus the original (control) version.

---

## 📊 Methodology

- **Cleaning and filtering** inconsistent entries between assigned groups and visited pages
- **Exploratory Data Analysis (EDA)** of conversion trends by group and country
- **Hypothesis Testing:**
  - Proportions z-test
  - Chi-squared test
  - Cohen’s h (effect size)
- **Subgroup Analysis** by country for deeper insight

---

## 🧠 Key Findings

- Control group had a slightly higher conversion rate (12.04%) than the treatment group (11.89%)
- No statistically significant difference between groups (`p = 0.2151`)
- Effect size was negligible (`Cohen’s h = 0.0046`)
- No country showed a statistically significant result (all `p > 0.05`)

---

## 📦 Requirements

Install packages with:

```bash
pip install -r requirements.txt

🧾 Author Note
This project was developed as a supplementary portfolio submission for Master's degree program applications. It demonstrates practical application of A/B testing, hypothesis testing, subgroup analysis, and reproducible reporting in Python.
