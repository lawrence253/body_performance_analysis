
# 📊 Statistical Processing Project — [Group_10]_Project_Final_03

This project is a comprehensive statistical analysis of the `bodyPerformance.csv` dataset. It includes data preprocessing, descriptive statistics, exploratory data analysis, and machine learning modeling using R.

---

## 📁 Project Structure

```
.
├── Statistical_Processing_Project_Report.Rmd  # Main R Markdown report
├── bodyPerformance.csv                        # Dataset used in the analysis
├── README.md                                  # Project documentation
```

---

## 📝 Project Overview

The project follows these key steps:

### 1. Data Loading
- Dataset: `bodyPerformance.csv`
- Cleaned column names using `janitor::clean_names`.

### 2. Descriptive Statistics
- Structure of data inspected with `dim()` and `glimpse()`.
- Summary statistics provided for each variable.
- Variables categorized into:
  - **Numerical:** age, height, weight, body fat, blood pressure, grip strength, flexibility, sit-ups, broad jump.
  - **Categorical:** gender, class.

### 3. Data Preprocessing
- **Missing Values:** Checked and confirmed there are no missing values.
- **Duplicates:** Identified and removed 1 duplicate row.
- **Outliers:** Boxplots used for visual inspection of outliers.

### 4. Exploratory Data Analysis
- Visualizations and correlation plots created using `ggplot2`, `corrplot`, etc.
- Analysis of relationships among numerical variables and between class labels.

### 5. Modeling
- Classification models to predict physical performance class:
  - Multinomial Logistic Regression
  - Decision Tree (`rpart`)
  - Random Forest
  - XGBoost
- Cross-validation using `caret` and `tidymodels` for performance evaluation.
- Feature importance visualized for interpretability.

### 6. Conclusion
- Models were evaluated and compared.
- Final remarks made regarding the best predictive methods and important variables.

---

## ▶️ How to Run

### Requirements

Make sure you have the following installed:

- **R (>= 4.0.0)**
- R packages:
  ```R
  install.packages(c("tidyverse", "janitor", "corrplot", "gridExtra", "nnet",
                     "caret", "rpart.plot", "randomForest", "xgboost", 
                     "themis", "tidymodels", "VIM", "lmPerm"))
  ```

### Running the Report

In R or RStudio, execute:

```R
rmarkdown::render("Statistical_Processing_Project_Report.Rmd")
```

Or open the Rmd file in RStudio and click **"Knit"** to render the report as HTML.

---

## 📌 Notes

- Ensure `bodyPerformance.csv` is located in the same directory as the Rmd file.
- To generate PDF output, install LaTeX (e.g., via TinyTeX with `tinytex::install_tinytex()`).

---

## 📬 Contact

For questions or collaboration inquiries, please contact **Group 10**.
