# ml_intern_cognifyz
# 🍽️ Restaurant Rating Prediction using Machine Learning

## 📌 Project Overview

This project was developed as part of the **Cognifyz Technologies Machine Learning Internship**.

The objective of this task is to build a machine learning model that predicts the **aggregate rating of restaurants** based on features such as cost, price range, votes, booking options, online delivery, city, and cuisines.

Multiple regression algorithms were implemented and compared to identify the best-performing model.

---

## 🎯 Objective

Build a machine learning regression model to predict restaurant ratings and analyze the factors that influence the ratings.

---

## 🛠️ Technologies Used

- Python
- Google Colab
- Pandas
- NumPy
- Matplotlib
- Scikit-learn
- Jupyter Notebook

---

## 📊 Dataset

The dataset contains information about restaurants, including:

- Restaurant ID
- Restaurant Name
- City
- Cuisines
- Average Cost for two
- Price Range
- Votes
- Has Table Booking
- Has Online Delivery
- Aggregate Rating

### Data Preprocessing

The following preprocessing steps were performed:

- Checked for missing values
- Handled missing cuisine values
- Removed duplicate records
- Selected relevant features
- Encoded categorical variables using One-Hot Encoding
- Split the dataset into training and testing sets

---

## 🤖 Machine Learning Models

Three regression models were implemented:

1. **Linear Regression**
2. **Decision Tree Regression**
3. **Random Forest Regression**

The models were trained using an 80:20 train-test split.

---

## 📈 Model Evaluation

The models were evaluated using:

- Mean Absolute Error (MAE)
- Mean Squared Error (MSE)
- Root Mean Squared Error (RMSE)
- R² Score

### Results

| Model | MAE | RMSE | R² Score |
|---|---:|---:|---:|
| Linear Regression | 0.992 | 1.209 | 0.358 |
| Decision Tree | 0.257 | 0.409 | 0.927 |
| **Random Forest** | **0.205** | **0.320** | **0.955** |

---

## 🏆 Best Performing Model

The **Random Forest Regression** model achieved the best performance.

- **MAE:** 0.205
- **RMSE:** 0.320
- **R² Score:** 0.955

The R² score indicates that the Random Forest model explains approximately **95.5% of the variation in the test-set restaurant ratings**.

---

## 📊 Visualizations

The project includes:

- Restaurant Rating Distribution
- Actual vs Predicted Restaurant Ratings
- Feature Importance Analysis

These visualizations help understand model performance and the factors contributing to restaurant rating predictions.

---

## 🔍 Feature Importance

Feature importance analysis was performed using the Random Forest model to identify the features that contribute most to predicting restaurant ratings.

---

## 💡 Key Insights

- Tree-based regression models performed considerably better than Linear Regression for this dataset.
- Random Forest achieved the highest predictive performance among the tested models.
- Restaurant characteristics such as cost, votes, price range, location, booking options, delivery options, and cuisines were considered for prediction.
- Feature importance analysis provides insights into which input features contribute most to the model's predictions.

---

## ✅ Conclusion

The restaurant rating prediction task was successfully completed using multiple machine learning regression techniques.

Among the evaluated models, **Random Forest Regression** performed the best with an **R² score of 0.955** and an **RMSE of 0.320**.

The project demonstrates the complete machine learning workflow, including data preprocessing, feature selection, model training, evaluation, comparison, visualization, and feature importance analysis.

---
