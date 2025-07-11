

🚧 This project is currently under development. Not ready for production use. 🚧







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
│ ├── 02_ab_test_analysis.ipynb # Statistical A/B test (z-test, chi2, effect size)
│ └── 03_report.ipynb # Summary insights and final report
│
├── outputs/
│ └── figures/ # Visualization images
│
├── reports/
│ └── final_report.pdf # Exportable summary (optional)
│
├── requirements.txt # Python dependencies
└── README.md # Project overview
```


---

## 🎯 Objective

To evaluate whether a newly implemented landing page results in a statistically significant improvement in conversion rate versus the original (control) version.

---

## 📊 Methodology

- **Cleaning and filtering** inconsistent entries between assigned groups and landing pages
- **Exploratory Data Analysis (EDA)** of conversion trends by group and country
- **Hypothesis Testing** using:
  - Proportions z-test
  - Chi-squared test
  - Cohen’s h (effect size)
- **Statistical interpretation** with confidence intervals

---

## 🧠 Key Findings

- Control group had a slightly higher conversion rate (12.04%) than the treatment group (11.89%)
- No statistically significant difference between groups (`p = 0.2151`)
- Effect size was negligible (`Cohen’s h = 0.0046`)
- 95% confidence intervals overlapped, reinforcing non-significance:
  - Control: [0.1187, 0.1221]
  - Treatment: [0.1173, 0.1206]

---

## 📦 Requirements

Install dependencies with:

```bash
pip install -r requirements.txt

🧾 Author Note
This project was developed as a supplementary portfolio submission for Master's degree program applications.
It demonstrates practical application of A/B testing, statistical hypothesis testing, and reproducible reporting in Python.
