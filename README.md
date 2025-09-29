# Task_5
EDA_Analysis

# 🛳️ Titanic Dataset EDA (Exploratory Data Analysis)

## Project Overview
This project performs a **comprehensive exploratory data analysis (EDA)** on the Titanic dataset to extract insights about passenger demographics, survival rates, and relationships between key features. The analysis uses **Python, Pandas, Matplotlib, and Seaborn** to visualize and summarize the findings.

##  Objective
- Understand the dataset structure, features, and missing values.  
- Explore survival patterns based on gender, age, socio-economic status, and embarkation port.  
- Identify correlations and patterns among numerical and categorical variables.  
- Provide actionable insights and observations to summarize Titanic survival trends.

##  Libraries Used
- `pandas` – Data manipulation and cleaning  
- `numpy` – Numerical operations  
- `matplotlib` – Basic plotting and visualization  
- `seaborn` – Advanced visualization and statistical plots  

##  Dataset
- File: `titanic.csv`  
- Contains passenger details, including:  
  - `PassengerId`, `Name`, `Sex`, `Age`, `SibSp`, `Parch`, `Ticket`, `Fare`, `Cabin`, `Embarked`, `Pclass`, `Survived`  

**Note:** Some columns like `PassengerId`, `Name`, `Ticket`, and `Cabin` were dropped due to irrelevance or high cardinality. Missing values for `Age` and `Embarked` were imputed.

##  Analysis Steps
1. **Data Loading & Cleaning**  
   - Handle missing values (`Age` with median, `Embarked` with mode)  
   - Convert `Pclass` to categorical  

2. **Statistical Exploration**  
   - `.info()` to understand dataset structure  
   - `.describe()` for descriptive statistics  
   - `.value_counts()` for categorical feature distribution  

3. **Visual Exploration**  
   - **Histograms & Boxplots:** Age and Fare distributions  
   - **Bar plots:** Survival rate by `Sex`, `Pclass`, and `Embarked`  
   - **Scatterplot:** Age vs Fare segmented by Survival  

4. **Advanced Visualization**  
   - **Pairplot:** Identify relationships among numerical features  
   - **Correlation Heatmap:** Check correlations between key variables  

5. **Observations & Insights**  
   - Gender is the strongest predictor of survival (females survived more)  
   - 1st-class passengers had higher survival rates than 3rd-class  
   - Children (<10 years) had higher survival, supporting the “women and children first” protocol  
   - Port of embarkation affected survival, with Cherbourg passengers surviving more often  
   - Fare and Pclass show socio-economic influence on survival  

##  Key Findings

| Factor | Observation |
|--------|-------------|
| Gender | Females had significantly higher survival rates (+0.54 correlation) |
| Age | Children (<10) had better chances of survival |
| Pclass | 1st class > 2nd class > 3rd class survival trend (-0.34 correlation) |
| Fare | Higher fare correlated with survival (+0.26 correlation) |
| Embarked | Cherbourg passengers survived more than others |

##  Visualizations
- **Age Distribution**: Most passengers between 20–40  
- **Fare Distribution**: Skewed with high-value outliers  
- **Survival by Sex, Pclass, Embarked**: Clear patterns favoring females and 1st-class passengers  
- **Scatterplot (Age vs Fare)**: Survivors clustered at higher fare, younger ages  
- **Pairplot & Heatmap**: Relationships between numerical variables and survival  

## 👤 Author
**Veera Sai Pavan Chavvakula**  
- Email: veerasaipavan6673@gmail.com  
- LinkedIn: [Author](https://www.linkedin.com/in/veera-sai-pavan-chavvakula-6260a72bb)
"""
