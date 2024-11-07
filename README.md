# Brain Stroke Detection

## Introduction
Brain stroke is a severe medical condition caused by the disruption of blood flow to the brain, leading to potential brain damage. This project focuses on building a machine learning model to predict brain stroke occurrence using various health and lifestyle indicators. Early detection is crucial for providing timely medical intervention, thus potentially saving lives.

## Project Overview
This project involves building a machine learning model to detect brain stroke risk. The project is executed on Google Colab and follows a sequence of data preprocessing, analysis, and model training. Using a logistic regression model, we aim to achieve high prediction accuracy for stroke detection.

## Dataset Overview
The dataset contains records of individuals with various health and demographic factors relevant to brain stroke risk. Key features such as age, BMI, and average glucose levels are used to predict the likelihood of a stroke.

### Data Columns
The original dataset contains the following columns:

- `id`: Unique identifier (dropped)
- `gender`: Gender of the individual (processed and encoded)
- `age`: Age of the individual
- `hypertension`: 1 if the patient has hypertension; 0 otherwise
- `heart_disease`: 1 if the patient has heart disease; 0 otherwise
- `ever_married`: Marital status (processed and encoded)
- `work_type`: Type of work (dropped)
- `Residence_type`: Type of residence (dropped)
- `avg_glucose_level`: Average glucose level in blood
- `bmi`: Body mass index
- `smoking_status`: Smoking status (processed and encoded)
- `stroke`: 1 if the patient had a stroke; 0 otherwise (target column)

### Preprocessing
- **Dropped Columns**: `id`, `work_type`, and `Residence_type`.
- **Encoded Columns**:
  - `gender` → `gender_encoded` (female=1, male=0)
  - `ever_married` → `married_encoded` (yes=1, no=0)
  - `smoking_status` → `smoking` (formerly smoked=1, never smoked=0)

## Data Analysis
Exploratory Data Analysis (EDA) was conducted to understand the distribution and correlation of features. Insights gained from the analysis guided the feature engineering and preprocessing steps, helping to enhance the model’s performance.

## Model Selection
The models chosen for this Brain Stroke Detection task are Logistic Regression and Random Forest, both of which are suitable for binary classification problems like this one. Here’s why each model is appropriate for your dataset.

## Model Training
- **Data Split**: The dataset was split into 80% for training and 20% for testing to evaluate the model's performance.
- **Training Results**: The training accuracy achieved is 95.43%.
- **Testing Results**: The testing accuracy achieved is 93.93%.

## Results
The model performs well on both the training and testing data, indicating good generalization and predictive capability.

| Metric       | Training Accuracy | Testing Accuracy |
|--------------|-------------------|-------------------|
| **Accuracy** | 0.9543            | 0.9393            |

## Conclusion
This project demonstrates a reliable approach for detecting brain stroke risk based on demographic and health-related features. With high accuracy on both training and testing sets, the model shows potential for real-world application in preliminary stroke risk screening.

