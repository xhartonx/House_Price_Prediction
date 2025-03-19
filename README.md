# House Price Prediction Project

This project is focused on house price prediction using advanced regression techniques. We analyze a dataset from Kaggle, apply data preprocessing, exploratory data analysis, feature engineering, and various machine learning models. The goal is to identify the most appropriate model to apply in accurate price predictions and to comprehend key factors influencing the prices of homes.

Data source: [https://www.kaggle.com/competitions/house-prices-advanced-regression-](https://www.kaggle.com/competitions/house-prices-advanced-regression-techniques)

---

## Table of Contents
- [Methods Used](#methods-used)
- [EDA and Feature Selection](#eda-and-feature-selection)
- [Result and Reports](#result-and-reports)
- [Model Insights](#model-insights)
- [Learnings and Takeaways](#learnings-and-takeaways)

---

## Methods used
### **Data Preprocessing**
- Setting thresholds to filter features and replace null values
- Handling missing values in numerical and categorical columns using imputation or deletion

### **Exploratory Data Analysis (EDA)**
- Visualizations: Histograms, Box Plots, Scatter Plots, Heatmaps, Pair Plots
- Identifying data distributions, outliers, and relationships between variables

### **Feature Engineering**
- Creating and transforming features to better represent the data

### **Correlation Analysis**
- Calculating correlation coefficients to identify potential relationships
- Visualizing correlations with heatmaps

### **Feature Importance**
- Using correlation analysis and machine learning models to determine key features

### **Building Models**
- **Algorithms used**: Linear Regression, Random Forest, XGBoost, Keras, Torch


---

## EDA and Feature Selection

### **Correlation Heatmap Analysis**
The heatmap reveals strong correlations between sale prices and factors like overall quality and living area size.

<img width="509" alt="heatmap" src="https://github.com/user-attachments/assets/964a7466-d697-4641-9b58-8ea20641a6a8">

### **Scatter Plot**
Scatter plot showing the relationship between living area size and sale price.

<img width="481" alt="scatterplot" src="https://github.com/user-attachments/assets/d9d5c00e-55f1-4ef7-b606-6f991c288afa">

### **Boxplot of Sale price by Sale Type**
Boxplot highlights a clear preference for newly built houses, leading to notably higher sale prices.

<img width="544" alt="boxplot1" src="https://github.com/user-attachments/assets/00994238-c1bc-4be7-aef3-f9fc595d50a6">

### **Scatter plot**
Demonstrating string relationship between above grade living area square feet and sales price depicted in the heatmap. The points align closely aling a discernible trend line, indicating a clear positive correlation between the variables.

<img width="481" alt="scatterplot" src="https://github.com/user-attachments/assets/4d7e71fa-7927-4012-b854-775e07053984">

### **Bar chart**
The bar chart indicates that house with public utilities command higher sale prices. This can be attributed to the convenience, reliability, and regulatory compliance associated with such properties.

<img width="519" alt="bar chart" src="https://github.com/user-attachments/assets/6c447d68-b0eb-4d2d-895c-2178f7dae3d4">

### **Bar chart and Scatter plot**
We uncover a strong correlation between overall quality and sales price. The bar chart highlights neighborhoods like NoRidge, NridgHt, and StoneBr with the highest quality ratings, suggesting that properties in these areas have the highest sale prices due to their superior quality.

<img width="617" alt="bar chart   scatter plot" src="https://github.com/user-attachments/assets/0e5eab08-eb96-4b9f-a3f7-547acdb698c8">

### **Bar chart and Violin plot**
From the bar chart above, it's evident that house equipped with Gas A heating boast the highest quality ratings. Moreover, there's a notable prevalence of homes ultilizing Gas A heating. Consequently, it can be inferred that properties featuring Gas A heating systems tend to command the highest sale prices.

<img width="624" alt="violin" src="https://github.com/user-attachments/assets/44f30002-5d1f-46c3-8c5f-7a5db2b931f2">

### **Box plot for Central air condition and Sale price**
Houses equipped with central air conditioning systems consistently exhibit higher sale prices, suggesting a strong positive correlation between the presence of central air conditioning and the sale proce. This finding underscores the importance of central air conditioning as a desirable feature in the real estate market.

<img width="543" alt="boxplot2" src="https://github.com/user-attachments/assets/82910b91-98b3-402d-8696-78f71710bbab">

---

## Result and Reports

We tested five different models and submitted predictions to Kaggle. The scores are as follows:

<img width="604" alt="score" src="https://github.com/xhartonx/House_Price_Prediction/blob/main/image/model%20performence.jpg">

## Model Insights

1. **Linear Regression**: Performed best with Lasso-selected features.
2. **Random Forest**: Struggled with feature importance and overfitting.
3. **XGBoost**: Performed well after extensive parameter tuning; optimal learning rate found at 0.0082.
4. **Keras**: Achieved the second-best score after hyperparameter tuning.
5. **Torch**: Underperformed compared to other models despite optimized layers and activation functions.

---

## Learnings and Takeaways

### Challenges Faced
- **Data Cleaning**: The most time-consuming part, as properly processed data was crucial for model performance.
- **Feature Selection**: Even with Lasso, important features might have been overlooked.
- **Model Optimization**: Tuning parameters did not always yield significant improvements.

### Future Improvements
- Explore advanced feature selection techniques such as model-based feature ranking (e.g., feature importance from Random Forest).
- Implement polynomial and interaction features to capture complex relationships.
- Consider deep learning approaches for further model improvement.


