# House_Price_Prediction_with_Linear-Regression

A supervised machine learning project focused on predicting residential property prices using the **King County Housing dataset**. This project demonstrates a complete data science pipeline, emphasizing data hygiene, descriptive visualization, and linear modeling.

##  Project Overview
Predicting real estate prices accurately requires evaluating multiple house features (e.g., bedrooms, living space square footage, construction year, grade). This project builds a **Linear Regression** model to infer property values while ensuring all channelling data satisfies regression assumptions through appropriate transformations.

##  Tech Stack & Libraries
- **Language:** Python
- **Data Manipulation:** Pandas, NumPy
- **Machine Learning:** Scikit-learn (LinearRegression, Train-Test-Split, StandardScaler, Metrics)
- **Data Visualization:** Matplotlib, Seaborn

##  Pipeline Stages
1. **Data Understanding:** Explored dataset shape ($21,613 \times 17$), features statistical summaries, and skewness coefficients.
2. **Data Cleaning & Anomaly Resolution:** * Resolved 177 duplicate property records keeping the most recent transaction.
   * Fixed structural data entry errors (e.g., corrected a house with an unrealistic 33 bedrooms down to 3).
   * Filtered out incomplete entries with 0 bedrooms/bathrooms.
   * Converted raw date texts into datetime format for proper feature parsing.
3. **Exploratory Data Analysis (EDA):** Performed target variable analysis, identifying a heavy right-skew ($4.02$). Applied log-transformation (`np.log1p`) to transform price tracking into a Gaussian/normal distribution.
4. **Feature Engineering & Scaling:** Standardized independent variables.
5. **Model Evaluation:** Evaluated performance utilizing $R^2$, Mean Absolute Error (MAE), and Root Mean Squared Error (RMSE).

##  Repository Structure
```text
├── house_price.xlsx            # King County Housing dataset
├── House_Price_Prediction.ipynb # Main Jupyter Notebook with full code
├── House_Price_Prediction.html  # Exported HTML snapshot of outputs
└── README.md                   # Project documentation
