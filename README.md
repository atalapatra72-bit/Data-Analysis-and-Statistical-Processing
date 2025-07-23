By Arjun Talapatra

This project uses regression analysis and statistical modeling techniques in **R** to explore relationships between independent and dependent variables in incomplete datasets. It is divided into two parts:

- **Part A**: Linear regression and missing value imputation
- **Part B**: Data transformation, binning, and lack-of-fit testing

---

## 🎯 Objectives

### Part A
- Impute missing values using the `mice` package
- Fit a simple linear regression model
- Evaluate significance using t-tests and F-tests
- Compute confidence intervals and determine the strength of the linear relationship

### Part B
- Experiment with transformations to improve model fit
- Perform data binning using `cut()` and averaging techniques
- Apply a **lack-of-fit test** using `pureErrorAnova()` from the `alr3` package
- Compare model performance before and after transformation

---

## 🧰 Tools & Technologies

- 💻 **R** and **RStudio**
- 📦 `mice`, `knitr`, `alr3`
- 🗃️ CSV datasets with missing and complete entries
- 📈 Statistical tools: t-test, F-test, ANOVA, R², residual analysis

---

## 📂 Files Included

| File | Description |
|------|-------------|
| `602237_IV.csv` | Independent variable dataset |
| `602237_DV.csv` | Dependent variable dataset |
| `602237_partB.csv` | Dataset for Part B transformation |
| `Project_Report.pdf` | Full write-up with methodology, output, and discussion |
| `regression_analysis.R` | All R code used for Parts A and B |

---

## 📊 Key Results

### Part A:
- Fitted model: **𝑦 = 35.5603 + 3.1801𝑥**
- p-value for slope: < `2e-16` (highly significant)
- R² = 0.5444, Adjusted R² = 0.5436
- Strong evidence of a linear relationship between IV and DV

### Part B:
- Best transformation: **y^(-2/3)**
- Transformed model fit significantly better (R² increased from ~0.53 to ~0.58)
- F-statistic and t-tests showed improved model performance
- Lack-of-fit p-value = 0.4388 → No evidence of model misfit
- Residuals appeared normally distributed and homoscedastic

---

## 🧠 Concepts Demonstrated

- Handling missing data with imputation
- Simple linear regression & hypothesis testing
- Confidence intervals for regression coefficients
- Model selection via transformation & validation
- Visual and statistical diagnostics for fit quality

---

## 📝 Report
https://github.com/atalapatra72-bit/Data-Analysis-and-Statistical-Processing/blob/main/Data%20Analysis%20and%20Statistical%20Processing.pdf


Includes detailed discussion, statistical output, code snippets, and result interpretation for both parts.

---
