# Password Strength Classification using Natural Language Processing

**A Predictive Model for Classifying Passwords into Strong, Good, or Weak Categories to Enhance Password Security.**

---

## Table of Contents

- [Project Overview](#project-overview)
- [Features](#features)
- [Tech Stack](#tech-stack)
- [Data Pipeline](#data-pipeline)
- [Modeling](#modeling)
- [Evaluation Metrics](#evaluation-metrics)
- [Setup Instructions](#setup-instructions)
- [Usage](#usage)
- [Future Enhancements](#future-enhancements)
- [Contributing](#contributing)
- [License](#license)

---

## Project Overview

The **Password Strength Classification** project aims to enhance password security by developing a predictive model that classifies passwords into three categories: **Strong**, **Good**, and **Weak**. This classification helps users understand the strength of their passwords and mitigates the risk of breaches by encouraging the use of stronger passwords.

The key goals of this project are:
- To provide an intuitive model for classifying passwords based on strength.
- To analyze and clean data from an SQL database for high-quality input.
- To apply advanced natural language processing techniques to enhance prediction accuracy.

---

## Features

- **Password Classification**: Classifies passwords into Strong, Good, or Weak categories based on learned features.
- **Data Visualization**: Provides insights into password strength distribution and common characteristics of each category.
- **User-Friendly Interface**: Allows users to input passwords and receive immediate feedback on strength classification.
- **Robust Data Analysis**: Uses thorough data cleaning and transformation techniques to ensure accurate model training.

---

## Tech Stack

- **Programming Language**: Python
- **NLP Libraries**: Scikit-learn, NLTK, Pandas
- **Data Processing**: NumPy, SQLAlchemy
- **Machine Learning**: Logistic Regression, TF-IDF (Term Frequency-Inverse Document Frequency)
- **Visualization**: Matplotlib, Seaborn
- **Deployment**: Flask (optional for web app), Jupyter Notebooks (for development)

---

## Data Pipeline

1. **Data Collection**: Password data is collected from an SQL database, containing a diverse set of password samples.
  
2. **Data Cleaning**:
   - Removed duplicates and irrelevant entries to ensure data quality.
   - Handled missing values by imputing or removing incomplete records.

3. **Data Transformation**:
   - Utilized the **TF-IDF** technique to convert password strings into numerical vectors for model training.
   - Engineered additional features such as password length, character variety (uppercase, lowercase, numbers, symbols), and common patterns.

4. **Exploratory Data Analysis (EDA)**:
   - Visualized the distribution of password strengths and analyzed common characteristics of Strong, Good, and Weak passwords.
   - Identified patterns that contribute to password strength.

---

## Modeling

### 1. **Logistic Regression Model**
   - Chose Logistic Regression for its effectiveness in binary classification problems and its interpretability.
   - Trained the model using the TF-IDF transformed features and the corresponding strength labels.

### 2. **Model Training**:
   - Split the dataset into training and testing sets to validate model performance.
   - Performed hyperparameter tuning to optimize the model’s performance.

### 3. **Model Validation**:
   - Evaluated the model using cross-validation techniques to ensure generalization.
   - Assessed performance metrics on the test set to confirm model reliability.

---

## Evaluation Metrics

The model is evaluated using the following metrics to ensure accurate password classification:

- **Accuracy**: Measures the overall correctness of the model's predictions.
- **Precision**: The ratio of true positive predictions to the total predicted positives, indicating the model's ability to identify Strong passwords.
- **Recall**: The ratio of true positive predictions to the total actual positives, reflecting the model's ability to capture all Strong passwords.
- **F1 Score**: The harmonic mean of precision and recall, providing a balanced measure of performance.

The Logistic Regression model achieved a high accuracy score, demonstrating its effectiveness in classifying password strengths accurately.

---

## Setup Instructions

### Prerequisites

- Python 3.7+
- Required libraries: Pandas, NumPy, Scikit-learn, NLTK, SQLAlchemy, Matplotlib, Seaborn

### Installation

1. Clone the repository:
   git clone https://github.com/SamJoeSilvano/Password_Strength_Prediction_using_NLP.git

2. Navigate to the project directory:
   cd password-strength-classification

3. Install the dependencies:
   pip install -r requirements.txt

4. Run the Jupyter Notebook or Flask app (optional):
   jupyter notebook

   or 

   python app.py

---

## Usage

1. **Load Data**: Import password data from the SQL database.
2. **Visualize Trends**: Generate visualizations to understand password strength distribution.
3. **Train Model**: The Logistic Regression model is trained on the processed password data.
4. **Classify Passwords**: Input passwords into the model to receive classification as Strong, Good, or Weak.
5. **Evaluate Model**: Analyze performance metrics to ensure classification accuracy.

---

## Future Enhancements

- **Advanced NLP Techniques**: Explore advanced models such as recurrent neural networks (RNNs) or transformers for improved classification.
- **User Interface**: Develop a more robust web application to allow users to test and visualize password strength interactively.
- **Real-time Feedback**: Implement real-time password strength feedback as users create passwords.
- **Broader Dataset**: Incorporate a wider range of password samples to enhance model robustness.

---

## Contributing

Contributions are welcome! Here’s how you can help:

1. Fork the project.
2. Create a new feature branch (`git checkout -b feature-branch`).
3. Commit your changes (`git commit -m 'Add new feature'`).
4. Push to the branch (`git push origin feature-branch`).
5. Open a pull request.

---

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for more details.

---

## Acknowledgements

- Thanks to the open-source community for their invaluable libraries and resources that made this project possible.
- Special recognition to the researchers and developers focused on enhancing password security.
```
