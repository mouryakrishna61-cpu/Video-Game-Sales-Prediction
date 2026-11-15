# 🎮 Video Game Sales Analysis and Prediction using Python

## 📌 Project Overview

This project focuses on analyzing video game sales data using Exploratory Data Analysis (EDA) and Machine Learning.

The objective is to explore historical video game sales, understand sales patterns across different regions, platforms, genres and publishers, and develop a Machine Learning model to predict global video game sales.

Three regression algorithms were trained and compared, followed by hyperparameter tuning to identify the best-performing model.

## 🎯 Project Objectives

- Explore and understand video game sales data.
- Perform data cleaning and preprocessing.
- Analyze sales patterns across different regions.
- Identify relationships between different features.
- Visualize important trends and patterns.
- Build and compare multiple regression models.
- Improve model performance using hyperparameter tuning.
- Predict global video game sales.

## 📊 Dataset Information

- **Dataset:** Video Game Sales (`vgsales.csv`)
- **Total Records:** 16,598
- **Prediction Target:** `Global_Sales`

### Dataset Features

The dataset contains information such as:

- Name
- Platform
- Year
- Genre
- Publisher
- NA_Sales
- EU_Sales
- JP_Sales
- Other_Sales
- Global_Sales

## 🛠️ Technologies and Libraries Used

| Technology | Purpose |
|---|---|
| Python | Programming |
| Google Colab | Development Environment |
| Pandas | Data Manipulation |
| NumPy | Numerical Operations |
| Matplotlib | Data Visualization |
| Seaborn | Statistical Visualization |
| Scikit-learn | Machine Learning |
| StandardScaler | Feature Scaling |
| GridSearchCV | Hyperparameter Tuning |
| Joblib | Model Serialization |

## 🔍 Project Workflow

### 1. Data Loading and Exploration
- Imported the dataset using Pandas.
- Examined dataset dimensions and data types.
- Explored columns and descriptive statistics.
- Checked missing values.

### 2. Data Cleaning and Preprocessing
- Prepared the dataset for analysis.
- Handled missing values.
- Converted categorical variables into numerical values using encoding.
- Prepared independent variables (X) and the target variable (y).

### 3. Exploratory Data Analysis (EDA)
- Explored video game sales patterns.
- Analyzed regional sales.
- Examined relationships between dataset features.
- Used visualizations to understand distributions and trends.

### 4. Feature Scaling
Applied `StandardScaler` to scale the training and testing features.

### 5. Machine Learning Model Development

Trained and compared three regression algorithms:

- Linear Regression
- Decision Tree Regressor
- Random Forest Regressor

### 6. Model Evaluation

Evaluated model performance using:

- **MAE:** Mean Absolute Error
- **MSE:** Mean Squared Error
- **R² Score:** Coefficient of Determination

### 7. Hyperparameter Tuning

Used `GridSearchCV` with 5-fold cross-validation and R² scoring to tune the Decision Tree and Random Forest models.

### Best Random Forest Parameters

| Parameter | Value |
|---|---:|
| n_estimators | 100 |
| max_depth | 10 |
| min_samples_split | 5 |
| random_state | 42 |

## 🤖 Model Performance Comparison

The following results were obtained after hyperparameter tuning.

| Model | MAE | MSE | R² Score |
|---|---:|---:|---:|
| Linear Regression | 0.5445 | 3.2228 | 0.0890 |
| Decision Tree | 0.5352 | 3.2900 | 0.0700 |
| Random Forest | **0.5222** | **3.1301** | **0.1152** |

### Best Performing Model: Random Forest Regressor

Random Forest achieved:

- Lowest MAE among the three models.
- Lowest MSE among the three models.
- Highest R² score among the three models.

The tuned Random Forest model was selected as the final model and saved for future predictions.

**Note:** The R² score of approximately 0.115 indicates that the model has limited predictive performance. Further feature engineering and model improvements could help improve the results.

## 📁 Project Structure

```text
Video-Game-Sales-Prediction/
│
├── EDA_PROJECT.ipynb
├── vgsales.csv
├── video_game_sales_model.pkl
├── video_game_sales_scaler.pkl
├── video_game_sales_features.pkl
├── requirements.txt
└── README.md
```

## 💾 Saved Model Files

The project contains three saved files:

- **video_game_sales_model.pkl:** Tuned Random Forest regression model.
- **video_game_sales_scaler.pkl:** Saved StandardScaler object.
- **video_game_sales_features.pkl:** Saved feature column information.

All three files were saved using Joblib for future model loading and prediction.

## 📚 Key Learnings

Through this project, I gained practical experience in:

- Exploratory Data Analysis.
- Data Cleaning and Preprocessing.
- Data Visualization.
- Categorical Feature Encoding.
- Feature Scaling.
- Regression Algorithms.
- Model Evaluation.
- Hyperparameter Tuning using GridSearchCV.
- Model Saving and Reusability using Joblib.

## 👨‍💻 Author

**Krishna Shiva Mourya**

 Python | Machine Learning
