# **Exploratory Data Analysis (EDA) on the Titanic Dataset**  

## **Step 1: Loading the Dataset**  
I started by importing the Titanic dataset into my Python environment using Pandas. To understand the dataset structure, I examined the column names, data types, and overall size. I displayed the first few rows to get an overview of the data. Additionally, I checked for missing values to identify which columns required cleaning.  

---

## **Step 2: Data Cleaning**  
### **Handling Missing Values**  
I identified columns with missing values and calculated the percentage of missing data. To handle these:  
- For numerical columns like **Age** and **Fare**, I used the median to fill in missing values.  
- For categorical columns like **Embarked**, I filled missing values with the most frequent category.  
- I dropped the **Cabin** column as it had excessive missing values and did not contribute significant insights.  

### **Removing Duplicates**  
I checked for duplicate rows in the dataset and removed any found to prevent biased results.  

### **Identifying and Managing Outliers**  
To detect outliers in numerical columns like **Fare** and **Age**, I used box plots. Based on the analysis, I removed extreme values from the **Fare** column that were above the 99th percentile, as they significantly skewed the data.  

---

## **Step 3: Data Visualization**  
### **Bar Charts for Categorical Variables**  
I created bar charts to visualize the distribution of categorical variables such as **Sex, Pclass, and Survived**. This helped me observe patterns like higher survival rates for females and first-class passengers.  

### **Histograms for Numeric Distributions**  
I plotted histograms for continuous variables like **Age** and **Fare** to analyze their distributions. The **Age** distribution showed most passengers were between 20-40 years old, while the **Fare** histogram revealed some skewness due to high-value outliers.  

### **Correlation Heatmap for Numeric Features**  
I generated a heatmap to explore correlations between numerical features. The analysis showed a strong correlation between **Fare** and **Survived**, indicating that passengers who paid higher fares had a better chance of survival.  

---

## **Step 4: Summarizing Insights**  
From my analysis, I observed the following key insights:  
- **Gender and class had a strong impact on survival rates** – Females and first-class passengers had higher chances of survival.  
- **Age distribution was mostly centered between 20-40 years**, with some outliers in older age groups.  
- **Fare had significant outliers**, and after removing extreme values, it showed a positive correlation with survival.  
- **Missing values were primarily in the Age, Cabin, and Embarked columns**, which were handled appropriately.  

This analysis provided a clear understanding of the Titanic dataset and its key influencing factors. 🚢✨


 

