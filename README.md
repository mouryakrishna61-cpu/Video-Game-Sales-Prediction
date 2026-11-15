# 🎮 Video Game Sales Analysis and Prediction

## 📌 Project Overview

This project focuses on analyzing video game sales data using **Exploratory Data Analysis (EDA)** and **Machine Learning**.

The main objective is to explore historical video game sales, identify patterns across different regions, platforms, genres and publishers, and build a regression model to predict global video game sales.

The project also compares multiple Machine Learning algorithms to identify the best-performing model.

## 🎯 Project Objectives

- Understand and explore the video game sales dataset.
- Perform data cleaning and preprocessing.
- Analyze video game sales trends and patterns.
- Explore relationships between different features and global sales.
- Build and compare multiple regression models.
- Improve model performance using hyperparameter tuning.
- Predict global video game sales.

## 📂 Dataset Information

- Dataset: Video Game Sales Dataset (`vgsales.csv`)
- Total Records: 16,598
- Target Variable: `Global_Sales`

The dataset contains information about video games, including:
- Game Name
- Platform
- Year
- Genre
- Publisher
- North American Sales
- European Sales
- Japanese Sales
- Other Regional Sales
- Global Sales

## 🛠️ Technologies and Libraries Used

| Technology | Purpose |
|---|---|
| Python | Programming Language |
| Google Colab | Development Environment |
| Pandas | Data Manipulation |
| NumPy | Numerical Operations |
| Matplotlib | Data Visualization |
| Seaborn | Statistical Visualization |
| Scikit-learn | Machine Learning |
| StandardScaler | Feature Scaling |
| GridSearchCV | Hyperparameter Tuning |
| Pickle | Saving Model Files |

## 🔍 Project Workflow

### 1. Data Loading and Exploration
- Imported the dataset using Pandas.
- Examined dataset dimensions and column information.
- Checked data types and missing values.
- Explored the dataset using descriptive statistics.

### 2. Data Cleaning and Preprocessing
- Handled missing values.
- Prepared the dataset for analysis.
- Converted categorical variables into numerical values using encoding.
- Separated independent variables (X) and the target variable (y).

### 3. Exploratory Data Analysis (EDA)
- Explored video game sales patterns.
- Analyzed sales across different regions.
- Examined relationships between dataset features.
- Used visualizations to understand data distributions and patterns.

### 4. Feature Scaling
Applied `StandardScaler` to scale the training and testing features.

### 5. Machine Learning Model Development

Developed and compared three regression algorithms:

- Linear Regression
- Decision Tree Regressor
- Random Forest Regressor

### 6. Model Evaluation

Evaluated model performance using:

- **MAE:** Mean Absolute Error
- **MSE:** Mean Squared Error
- **R² Score:** Coefficient of Determination

### 7. Hyperparameter Tuning

Used `GridSearchCV` with 5-fold cross-validation to tune Decision Tree and Random Forest models.

Selected the best parameters based on R² scoring.

## 🤖 Model Performance Comparison

The following results were obtained after hyperparameter tuning.

| Model | MAE | MSE | R² Score |
|---|---:|---:|---:|
| Linear Regression | 0.5445 | 3.2228 | 0.0890 |
| Decision Tree | 0.5352 | 3.2900 | 0.0700 |
| Random Forest | **0.5222** | **3.1301** | **0.1152** |

### Best Performing Model: Random Forest Regressor

Random Forest achieved:
- Lowest Mean Absolute Error (MAE).
- Lowest Mean Squared Error (MSE).
- Highest R² Score.

The results indicate that Random Forest performed better than the other two models on the test dataset.

**Note:** The R² score indicates that the model's predictive performance is limited, leaving scope for further improvement.

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

The project includes three saved files:

- `video_game_sales_model.pkl` – Saved Machine Learning model.
- `video_game_sales_scaler.pkl` – Saved feature scaler.
- `video_game_sales_features.pkl` – Saved feature information.

These files can be used for future model loading and prediction workflows.

## 📚 Key Learnings

Through this project, I gained practical experience in:

- Data Exploration and Analysis.
- Data Cleaning and Preprocessing.
- Data Visualization.
- Categorical Feature Encoding.
- Feature Scaling.
- Regression Algorithms.
- Model Evaluation.
- Hyperparameter Tuning using GridSearchCV.
- Saving Machine Learning models using Pickle.

## 👨‍💻 Author

**Krishna Shiva Mourya**

 Python | Machine Learning
