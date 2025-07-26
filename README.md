# Advertising
AIM
The ultimate goal of this project is to build a Machine Learning model that identifies which advertising medium (TV, Radio, or Newspaper) is most influential in predicting future sales performance. The model focuses on building and evaluating a Simple Linear Regression to determine the relationship between advertising spend and sales.
📁 Dataset
File: Advertising Dataset (2).csv
Columns:
TV: Budget spent on TV ads
Radio: Budget spent on radio ads
Newspaper: Budget spent on newspaper ads
Sales: Product sales in units
🔍 Workflow Overview
1. 📥 Data Import and Initial Analysis
Loaded CSV data into a pandas DataFrame.
Checked column names, shapes, datatypes, and unique values.
Inspected data using .head(), .tail(), and .info().

2. 📊 Descriptive Statistics
Calculated:
Mean, Median, Mode for TV and Sales.
Range, Variance, and Standard Deviation for Radio and Newspaper.

3. 🧹 Data Cleaning
Removed missing values using .dropna().
Verified missing data percentage per column.

4. 📉 Outlier Analysis & Visualizations
Visualized potential outliers using:
Boxplots, Scatterplots, Violin Plots
Histogram for TV ads
Q-Q Plot to check normality for Radio

5. 📈 Univariate, Bivariate, and Multivariate Analysis
Plotted:
Boxplot and histogram for individual variables
Scatterplot for TV vs Sales
Correlation Heatmap\
Pairplot to explore variable relationships
⚙️ Model Building: Simple Linear Regression
🧮 Mathematical Model
Linear Regression Equation:

𝑦
=
𝑐
+
𝑚
⋅
𝑥
y=c+m⋅x
Where:

y = Predicted Sales

x = Advertising Budget (e.g., Radio)

c = Intercept

m = Coefficient (slope)

📌 Steps
Selected Radio as the predictor variable (X) and Sales as the target (y).
Split dataset into 70% Training and 30% Testing using train_test_split.
Built the linear regression model using statsmodels and sklearn.

🧪 Model Evaluation
🔢 Training Evaluation
Evaluated model summary: Coefficients, R-squared, p-values.
Visualized regression line on training data.
Analyzed residuals (errors) distribution.

🔍 Testing Evaluation
Predicted sales values on test set.
Metrics used:
Mean Squared Error (MSE)
Root Mean Squared Error (RMSE)
R-Squared (R²) Score

Visualized:
Bar and Line Plot of actual vs predicted sales
Regression Line on test scatterplot

📈 Performance Metrics
Metric	Description	Output
MSE	Average squared difference between actual and predicted values	Printed in code
RMSE	Square root of MSE, indicates model error	Printed in code
R² Score	Proportion of variance in sales explained by the model	Printed in code

🛠️ Tools & Technologies
Language: Python
Libraries: pandas, numpy, matplotlib, seaborn, scikit-learn, statsmodels, scipy

📂 Output
Cleaned and saved dataset: Advertising Dataset (2).csv
Visual plots for insights and model evaluation
Regression model trained and tested on advertising data

✅ Conclusion
This project demonstrates how Linear Regression can effectively identify the relationship between advertising mediums and product sales. Among the features, Radio was modeled to understand its direct impact on sales. Further model tuning or adding multiple regression can improve prediction accuracy.
