# MSCS_634_Lab_1


#  Lab 1: Exploratory Data Analysis and Preprocessing

## Purpose

The purpose of this lab was to perform **exploratory data analysis (EDA)** and **data preprocessing** on a real-world dataset. This involved cleaning the data, handling missing values, detecting and removing outliers, reducing data complexity, applying scaling and discretization techniques, and analyzing statistical properties.

---

##  Key Insights

### 🔍 Visualizations:
- **Histogram (Price Distribution):** Most product prices are below 20 units, with a few high-price outliers, suggesting a skewed distribution.
- **Line Plot (Daily Sales):** Clear sales spikes on specific dates indicate potential seasonal effects or promotional periods.
- **Bar Chart (Top Countries by Sales):** The United Kingdom was the leading market, with significantly higher sales than other countries.

###  Statistical Measures:
- **Mean and Median:** Central tendency metrics revealed that the mean price is higher than the median, confirming positive skewness.
- **IQR and Standard Deviation:** Outlier detection showed that a small number of transactions had unusually high prices.
- **Correlation Analysis:** Quantity and price showed weak correlation, suggesting independent behavior for purchasing quantity.

---

##  Challenges and Decisions

- **Encoding Errors:** The dataset required specifying the correct encoding (`ISO-8859-1`) due to special characters.
- **Outlier Handling:** Outliers in `UnitPrice` were filtered using the IQR method to improve the quality of analysis.
- **Missing Data:** Missing `CustomerID` values were handled using forward fill, balancing completeness and integrity.
- **Sampling:** Data was reduced by 90% for efficiency without significantly impacting the representativeness of the dataset.
- **Scaling/Discretization:** Applied Min-Max Scaling to `UnitPrice` and binned `Quantity` into categorical levels for simplified modeling.

---

##  Summary

This lab provided hands-on experience with core data analysis techniques and prepared the dataset for future modeling tasks (regression, classification, etc.) in the Project. The visual and statistical analysis yielded meaningful insights into customer behavior and sales dynamics.
