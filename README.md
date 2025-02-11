# Insurance-Cost-Analysis

## 1. Project Overview
This project aims to analyze medical insurance costs based on various factors such as age, BMI, smoking status, and number of children. By performing exploratory data analysis (EDA) and correlation studies, we identify key contributors to higher insurance costs. The dataset is visualized using different plots, including regression and boxplots, to uncover insights into the distribution and relationship between variables.

## 2. Dataset Description
The dataset consists of multiple attributes related to insurance policyholders:
- **age**: Age of the policyholder
- **gender**: Male or Female
- **bmi**: Body Mass Index, a measure of body fat based on height and weight
- **no_of_children**: Number of dependent children covered by the insurance
- **smoker**: Whether the policyholder is a smoker or not (Yes/No)
- **region**: The geographical region where the policyholder resides
- **charges**: Medical insurance cost

## 3. Data Preprocessing & Cleaning
Before conducting the analysis, we performed the following preprocessing steps:
- **Handling Missing Values**:
  - Categorical variables (e.g., `smoker`) were replaced with the most frequent value.
  - Continuous variables (e.g., `age`) were filled with the mean value.
- **Data Type Conversion**:
  - Converted categorical variables (e.g., `smoker`) into numerical values for analysis.
- **Outlier Detection**:
  - Used boxplots to detect and analyze outliers in `charges`.

## 4. Exploratory Data Analysis (EDA)
Several statistical and visualization techniques were applied to understand the relationships between different features:
- **Correlation Heatmap**: Displayed how strongly different variables are related to each other.
- **Regression Plot**: Used to examine the relationship between `bmi` and `charges`, highlighting trends.
- **Boxplot Analysis**: Showed the impact of smoking on medical costs, revealing that smokers have significantly higher insurance charges.

## 5. Results & Key Findings
- **Smoking status is the most significant factor affecting insurance costs** (Correlation: **0.788**). Smokers pay significantly higher charges compared to non-smokers.
- **Age and BMI have a moderate correlation with insurance costs** (Age: **0.298**, BMI: **0.199**), indicating that older individuals and those with higher BMI tend to incur more medical expenses.
- **Gender, number of children, and region have minimal influence on insurance charges** (correlation values close to zero).
- **The dataset exhibits outliers in insurance charges**, primarily among smokers and individuals with high BMI, suggesting potential cases of high medical expenditures.

## Conclusion
This analysis provides valuable insights into the factors driving medical insurance costs. The findings can help insurance companies develop better pricing models and individuals understand the impact of lifestyle choices on their expenses.

---
### Future Work
- Investigate additional features that might contribute to insurance costs.
- Apply machine learning models to predict insurance charges based on input features.
- Explore regional disparities in insurance costs with more granular data.

### Dependencies
- Python
- Pandas
- Seaborn
- Matplotlib
- NumPy

