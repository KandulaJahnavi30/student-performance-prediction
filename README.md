# Student Performance Prediction Using Machine Learning

## Project Overview

**Student Performance Prediction Using Machine Learning** is a machine learning project developed in **Google Colab** to analyze student academic data and predict student performance.

The project uses a dataset containing **5,000 student records** with academic, attendance, study, lifestyle, and other student-related features.

Three machine learning models are implemented:

1. **Decision Tree Classifier** – predicts student performance category.
2. **Random Forest Classifier** – predicts student performance category.
3. **Decision Tree Regressor** – predicts the student's final score.

The project also includes data preprocessing, missing-value handling, categorical data encoding, model evaluation, model comparison, and visualization.

---

## Objectives

The main objectives of this project are:

* To analyze student performance data.
* To handle missing values in the dataset.
* To convert categorical data into numerical form.
* To predict student performance categories.
* To predict students' final scores.
* To compare the performance of different machine learning models.
* To visualize model results.

---

## Dataset

The dataset contains **5,000 synthetic student records**.

### Dataset Features

| Feature                    | Description                                 |
| -------------------------- | ------------------------------------------- |
| Student_ID                 | Unique student identifier                   |
| Study_Hours                | Number of hours spent studying              |
| Attendance                 | Student attendance percentage               |
| Previous_Marks             | Previous academic marks                     |
| Assignment_Score           | Assignment performance                      |
| Internal_Exam_Score        | Internal examination score                  |
| Sleep_Hours                | Average sleeping hours                      |
| Extracurricular_Activities | Participation in extracurricular activities |
| Internet_Access            | Availability of internet access             |
| Parent_Education           | Education level of parents                  |
| Final_Score                | Final examination/academic score            |
| Performance                | Student performance category                |

The dataset contains both **numerical and categorical features**.

---

## Technologies Used

* Python
* Google Colab
* Pandas
* NumPy
* Scikit-learn
* Matplotlib

---

## Machine Learning Models

### 1. Decision Tree Classifier

The Decision Tree Classifier is used to predict the student's **Performance** category.

The model learns decision rules from the student features and classifies students into their respective performance categories.

### 2. Random Forest Classifier

The Random Forest Classifier is also used to predict the **Performance** category.

Random Forest uses multiple decision trees and combines their predictions to produce the final classification result.

### 3. Decision Tree Regressor

The Decision Tree Regressor is used to predict the student's **Final_Score**.

The regression model is evaluated using:

* MAE – Mean Absolute Error
* MSE – Mean Squared Error
* RMSE – Root Mean Squared Error
* R² Score – Coefficient of Determination

---

## Project Workflow

The project follows these steps:

```text
Load Dataset
      ↓
Explore Dataset
      ↓
Check Missing Values
      ↓
Handle Missing Values
      ↓
Encode Categorical Features
      ↓
Select Features and Targets
      ↓
Split Dataset into Training and Testing Data
      ↓
Decision Tree Classification
      ↓
Random Forest Classification
      ↓
Decision Tree Regression
      ↓
Evaluate Models
      ↓
Compare Results
      ↓
Visualize Results
```

---

## Data Preprocessing

### Missing Values

Missing numerical values are replaced using the **median** of the corresponding column.

Missing categorical values are replaced using the **most frequent value (mode)**.

### Categorical Encoding

The following categorical columns are converted into numerical values using one-hot encoding:

* Extracurricular_Activities
* Internet_Access
* Parent_Education

### Student ID

`Student_ID` is removed before model training because it is only an identifier and does not provide useful information for prediction.

---

## Train-Test Split

The dataset is divided into:

* **80% Training Data**
* **20% Testing Data**

A `random_state` of `42` is used to make the split reproducible.

---

## Model Evaluation

### Classification Models

The classification models are evaluated using:

* Accuracy
* Classification Report

### Regression Model

The regression model is evaluated using:

* MAE
* MSE
* RMSE
* R² Score

---

## Model Comparison

The project creates a comparison table containing the results of all three models.

| Model                    | Task                   | Evaluation Metric |
| ------------------------ | ---------------------- | ----------------- |
| Decision Tree Classifier | Performance Prediction | Accuracy          |
| Random Forest Classifier | Performance Prediction | Accuracy          |
| Decision Tree Regressor  | Final Score Prediction | R² Score          |

The notebook also generates graphs for:

* Classification Model Accuracy
* Actual vs Predicted Final Score

---

## Results

The actual results are generated when the Google Colab notebook is executed.

### Classification Results

| Model                    |              Accuracy |
| ------------------------ | --------------------: |
| Decision Tree Classifier | Generated by notebook |
| Random Forest Classifier | Generated by notebook |

### Regression Results

| Metric   |                Result |
| -------- | --------------------: |
| MAE      | Generated by notebook |
| MSE      | Generated by notebook |
| RMSE     | Generated by notebook |
| R² Score | Generated by notebook |

---

## Project Structure

```text
student-performance-prediction/
│
├── student_performance.ipynb
├── student_performance_5000.csv
├── README.md
└── requirements.txt
```

---

## How to Run the Project

### Step 1: Open Google Colab

Open the project notebook in Google Colab.

### Step 2: Upload the Dataset

Upload:

```text
student_performance_5000.csv
```

### Step 3: Run the Notebook

Run the notebook cells from beginning to end.

The notebook will:

* Load the dataset
* Analyze the data
* Clean missing values
* Encode categorical features
* Train the machine learning models
* Evaluate the models
* Display model comparison results
* Generate graphs

---

## Example Predictions

The project can be used to understand student performance based on features such as:

* Study hours
* Attendance
* Previous marks
* Assignment score
* Internal examination score
* Sleep hours
* Extracurricular activities
* Internet access
* Parent education

The classification models predict the student's **Performance** category, while the regression model predicts the **Final Score**.

---

## Advantages

* Uses a large dataset containing 5,000 records.
* Handles missing data.
* Supports both classification and regression.
* Uses multiple machine learning models.
* Provides model evaluation metrics.
* Includes visualizations.
* Can be executed completely in Google Colab.

---

## Future Scope

The project can be improved in the future by:

* Using larger real-world datasets.
* Adding more student-related features.
* Improving model performance through hyperparameter tuning.
* Developing a user-friendly prediction interface.
* Creating a web-based dashboard.
* Providing personalized student performance insights.
* Identifying students who may require additional academic support.
* Deploying the trained model for real-time predictions.

---

## Conclusion

This project demonstrates how machine learning can be used to analyze and predict student academic performance.

The project implements **Decision Tree Classification, Random Forest Classification, and Decision Tree Regression** to perform both performance-category prediction and final-score prediction.

The complete workflow, from data preprocessing to model evaluation and visualization, is implemented using **Python and Google Colab**.

---

## Author

**Student Performance Prediction Using Machine Learning**

Developed as a machine learning academic project using Python and Google Colab.
