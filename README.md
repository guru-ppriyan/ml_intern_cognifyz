# ml_intern_cognifyz
# Task 1 : 🍽️ Restaurant Rating Prediction using Machine Learning

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
# Task 2: Restaurant Recommendation System

## Overview

This project was completed as part of the Machine Learning Internship at Cognifyz Technologies.

The objective of this task is to develop a restaurant recommendation system that provides personalized restaurant recommendations based on user preferences such as cuisine and price range.

A content-based filtering approach is used to identify restaurants that are similar to the user's preferred criteria.

---

## Objective

To create a restaurant recommendation system based on user preferences and recommend restaurants that closely match the user's selected cuisine and price range.

---

## Technologies Used

- Python
- Pandas
- NumPy
- Scikit-learn
- Matplotlib
- Google Colab

---

## Dataset

The project uses a restaurant dataset containing information such as:

- Restaurant Name
- Cuisines
- City
- Price Range
- Aggregate Rating
- Votes

---

## Data Preprocessing

The following preprocessing steps were performed:

1. Loaded the restaurant dataset.
2. Checked for missing values.
3. Removed duplicate records.
4. Selected relevant features required for recommendation.
5. Converted cuisine information into lowercase text.
6. Prepared a combined content feature using cuisine, city, and price range.

---

## Recommendation Criteria

The recommendation system uses the following user preferences:

- Cuisine Preference
- Price Range

These criteria are used to identify restaurants that are most relevant to the user's requirements.

---

## Recommendation Approach

A content-based filtering approach was implemented.

### TF-IDF Vectorization

TF-IDF (Term Frequency-Inverse Document Frequency) was used to convert the textual restaurant content into numerical feature vectors.

### Cosine Similarity

Cosine similarity was used to measure the similarity between the user's preferences and the restaurants in the dataset.

Restaurants with higher similarity scores are considered more relevant to the user's preferences.

---

## Recommendation Process

The recommendation system follows these steps:

1. Accept user preferences.
2. Create a preference representation using cuisine and price range.
3. Convert the preferences into a TF-IDF vector.
4. Calculate cosine similarity with all restaurants.
5. Rank restaurants according to their similarity scores.
6. Return the top recommended restaurants.

---

## Sample User Testing

A sample user preference was provided to test the recommendation system.

**Cuisine Preference:** North Indian

**Price Range:** 2

The system generated the top 5 restaurants matching the user's preferences.

The recommendations include:

- Restaurant Name
- Cuisine
- City
- Price Range
- Aggregate Rating
- Similarity Score

---

## Recommendation Quality Evaluation

The recommendation system was evaluated using:

- Number of cuisine matches
- Number of price-range matches
- Average similarity score

These measures help determine how closely the recommended restaurants match the sample user's preferences.

---

## Visualization

A bar chart was created to visualize the similarity scores of the top recommended restaurants.

The visualization makes it easier to compare the relevance of the recommended restaurants.

---

## Key Features

- Personalized restaurant recommendations
- Cuisine-based filtering
- Price-range consideration
- TF-IDF text vectorization
- Cosine similarity
- Recommendation quality evaluation
- Similarity score visualization

---

## Conclusion

A content-based restaurant recommendation system was successfully developed using user preferences such as cuisine and price range.

TF-IDF vectorization and cosine similarity were used to identify restaurants that closely match the user's preferences. The system was tested using sample preferences and evaluated based on cuisine matching, price-range matching, and similarity scores.

Overall, the project demonstrates how content-based filtering can be applied to provide personalized restaurant recommendations.

---

