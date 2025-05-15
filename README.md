# ☕ Coffee Chain Sales Data Analysis

This project explores and analyzes the **Coffee Chain Sales dataset** to uncover business insights, identify outliers, assess variable distributions, and apply statistical transformations for better modeling readiness.

---

## 📊 Project Overview

The main objectives of this analysis are:

* Perform **Exploratory Data Analysis (EDA)** to understand the distribution, correlations, and anomalies within the dataset.
* Detect and handle **skewness** in numerical variables, especially `Profit`, through various transformations.
* Visualize insights to assist in making data-driven business decisions.

---

## 📁 Files Included

| File Name                        | Description                                                                       |
| -------------------------------- | --------------------------------------------------------------------------------- |
| `Coffee_Chain_Sales.csv`         | Original dataset                                                                  |
| `Updated_Coffee_Chain_Sales.csv` | Cleaned and updated dataset                                                       |
| `EDA_MK.R`                       | Script for initial EDA, correlation matrix, outlier detection, and histograms     |
| `Log_Trans_MK.R`                 | Advanced data transformation including log, square root, Box-Cox, and Yeo-Johnson |
| `project.Rmd`                    | R Markdown document summarizing the workflow and visuals (report-ready format)    |

---

## 🔍 EDA Highlights

Performed in `EDA_MK.R`:

* Summary statistics for numerical and categorical variables
* Missing value check (none found)
* Correlation matrix to identify strong linear relationships
* Boxplot visualization of `Profit` to detect outliers
* Histogram plots for all numeric features

---

## 🔁 Data Transformation

Performed in `Log_Trans_MK.R`:

**Skewness Reduction Techniques:**

* Log Transformation
* Square Root Transformation
* Box-Cox Transformation (λ optimized)
* Yeo-Johnson Transformation (via `caret::preProcess`)

**Profit Variable Transformation Example:**

| Transformation | Skewness |
| -------------- | -------- |
| Original       | High     |
| Log            | Reduced  |
| Square Root    | Reduced  |
| Box-Cox        | Optimal  |
| Yeo-Johnson    | Optimal  |

**Additional Transformed Variables:**

* `Log_Profit`
* `Log_Sales`
* `Log_Total_expenses`

**Exported File:**
📁 `Updated_Coffee_Chain_Sales_with_Log_Transforms.csv` – includes all transformed columns

---

## 📈 Visualizations

* Histograms (before vs after transformation)
* Correlation matrices (pre and post transformation)
* Boxplots for outlier detection
* Distribution comparisons

---

## 💡 Key Takeaways

* `Profit`, `Sales`, and `Total_expenses` were highly skewed — log-based transformations improved normality.
* Box-Cox and Yeo-Johnson methods were most effective in reducing skewness.
* Insights derived can support better modeling, forecasting, and decision-making for business operations.

---

## 🛠️ Tools Used

* Language: **R**
* Libraries: `ggplot2`, `dplyr`, `MASS`, `e1071`, `caret`, `corrplot`

---

## 📌 How to Run

1. Install required R packages (listed in the scripts).
2. Load the dataset using `read.csv`.
3. Source and run either `EDA_MK.R` or `Log_Trans_MK.R`.
4. View results in RStudio Plots or export as needed from `project.Rmd`.

---

## 📬 Contact

Created by **Manoj Kumar Ashok**
📧 [Email Me](mailto:your-email@example.com)
🔗 [LinkedIn](https://www.linkedin.com/in/manoj-kumar-ashok-078241211/)
🐙 [GitHub](https://github.com/MK-Github03)

---

