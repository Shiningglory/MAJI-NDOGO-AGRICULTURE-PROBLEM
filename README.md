# MAJI-NDOGO-AGRICULTURE-PROBLEM
***Python Data Analysis & Regression Modeling***

<img width="626" height="351" alt="image" src="https://github.com/user-attachments/assets/538666be-e11d-471c-b4f3-f6e44122a57c" />

# INTRODUCTION
Maji Ndogo, an imaginary country, is facing agricultural challenges due to geographic, weather, and soil conditions. This project aims to analyze farming data, understand key factors influencing crop yield, and develop a predictive model to assist in optimizing farm production.

By leveraging data analysis and regression modeling, we can recommend best farming practices for different regions and conditions.

# PROBLEM STATEMENT
Farmers in Maji Ndogo need insights into where and what to plant based on environmental conditions.
Key challenges include:

- Identifying the best locations for specific crops based on soil, weather, and geography.
- Understanding the relationship between environmental factors and crop yield.
- Predicting standardized crop yield using linear regression.

# SKILL DEMONSTRATION
- Data Extraction & Cleaning: Importing from SQLite database and merging multiple tables.
- Exploratory Data Analysis (EDA): Identifying trends and relationships.
- Feature Engineering: Creating meaningful variables for prediction.
- Machine Learning (Regression): Building a Simple Linear Regression Model.
- Data Visualization: Using matplotlib & seaborn to analyze trends.

# DATA SOURCING
The dataset is stored in an SQLite database and consists of multiple tables:

1. ### Geographic Features
- Field_ID – Unique identifier for each field.
- Elevation, Latitude, Longitude – Geospatial data.
- Slope – Measures land inclination.
2. ### Weather Features
- Rainfall (mm)
- Minimum & Maximum Temperature (°C)
- Average Temperature (°C)
3. ### Soil & Crop Features
- Soil Fertility Index (0-1)
- Soil Type & pH Level
- Chosen Crop & Standardized Yield
4. ### Farm Management Features
- Pollution Level (0-1)
- Plot Size (Hectares)
- Annual Yield

# EXPLORATORY DATA ANALYSIS (EDA)
EDA was performed to explore how environmental factors influence crop yield.

<img width="571" height="455" alt="image" src="https://github.com/user-attachments/assets/69794865-87f7-4bea-8b1a-626ab72739b1" />

1. ### Data Overview
- Extracted multiple tables from SQLite and merged into a single pandas DataFrame.
- Checked for missing values and handled inconsistencies.
2. ### Feature Distributions
- Histograms & Box Plots for rainfall, temperature, soil fertility, and pollution levels.
- Scatter Plots to visualize relationships between yield and environmental factors.

<img width="567" height="497" alt="image" src="https://github.com/user-attachments/assets/39a3920a-13fe-4561-8d09-f5f19a8ace6f" />
<img width="567" height="498" alt="image" src="https://github.com/user-attachments/assets/e94a81be-b3e8-4909-bce5-fef63f708866" />

3. ### Correlation Analysis
- Heatmap showing relationships between rainfall, temperature, soil type, and crop yield.
- Pairplot to analyze interactions between multiple variables.
4. ### Key Insights
- Temperature and Rainfall are major predictors of crop yield.
- Soil Fertility significantly influences standardized yield.
- Some locations are more suitable for specific crops due to their environmental conditions.

<img width="567" height="455" alt="image" src="https://github.com/user-attachments/assets/81e19f72-f02b-444f-be4d-9022327b5ee7" />
<img width="567" height="455" alt="image" src="https://github.com/user-attachments/assets/ccb55620-2405-4a32-887b-609a798fc964" />

# MODELLING
To predict standardized crop yield, we implemented Simple Linear Regression.

1. Model Implementation
- Independent Variable (X): Selected environmental factors (e.g., temperature, rainfall, soil fertility).
- Dependent Variable (y): Standardized crop yield.
- Model Used: sklearn.linear_model.LinearRegression
- Training & Testing: Dataset split into 80% training, 20% testing.

<img width="567" height="433" alt="image" src="https://github.com/user-attachments/assets/8163df51-1bf0-4e42-b0e5-89721ac37737" />

2. ### Model Evaluation
- Mean Absolute Error (MAE) – Measures average prediction error.
- Mean Squared Error (MSE) – Penalizes large errors.
- R² Score – Explains variance in crop yield due to environmental factors.

# ANALYSIS & VISUALIZATION
- Scatter Plot: Relationship between rainfall, temperature, and crop yield.
- Correlation Heatmap: Identifies strongest predictors for crop yield.
- Regression Line Plot: Shows linear relationship between environmental factors and yield.
- Residual Plot: Evaluates model accuracy by checking prediction errors.

<img width="850" height="547" alt="image" src="https://github.com/user-attachments/assets/d6f427bc-2cfe-42c4-b8be-86f626fb16e4" />
<img width="857" height="547" alt="image" src="https://github.com/user-attachments/assets/12d8fad5-f4e5-4601-aaad-c226cdaa4d35" />

# CONCLUSION
1. Rainfall & Temperature are the strongest predictors of crop yield.
2. Soil Fertility has a significant impact on standardized yield.
3. The Simple Linear Regression model successfully predicts crop yield trends.
4. Future improvements should include multiple regression models for better accuracy.
   
# HOW TO RUN THE PROJECT
1. Prerequisites
Ensure you have Python installed along with the required libraries:

```pip install numpy pandas sqlite3 seaborn scikit-learn matplotlib```

2. Clone the Repository
   
```git clone https://github.com/yourusername/Maji-Ndogo-Agriculture.git  cd Maji-Ndogo-Agriculture```

4. Run the Jupyter Notebooks

```jupyter notebook Code_challenge_Integrated_Project_P1_model_solution.ipynb
jupyter notebook Linear_regression_Code_challenge_model_solution.ipynb```


