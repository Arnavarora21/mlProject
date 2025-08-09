# EPL Match Outcome Prediction using Machine Learning

## 1. Project Overview

This project focuses on the **development of a machine learning model designed to predict the outcomes of English Premier League (EPL) matches**. Recognizing the inherent unpredictability of football results and the complexity of performance metrics, this initiative explores the potential of machine learning to provide accurate, data-driven match predictions. The comprehensive process — encompassing dataset acquisition, systematic preprocessing, exploratory analysis, model training, and performance evaluation — was conducted using established data science methodologies.

---

## 2. Problem Statement

The EPL is one of the most competitive football leagues in the world, with outcomes influenced by a wide range of factors such as team form, venue, player performance, and historical results. Traditional statistical approaches often fail to capture these complex, non-linear relationships. This project seeks to address this challenge by leveraging **machine learning classification techniques** to predict match outcomes, thereby providing valuable insights for sports analysts, betting companies, and fan engagement platforms.

---

## 3. Project Objective

The primary objective of this project is to **construct and rigorously evaluate a machine learning model capable of predicting whether an EPL match will result in a win, draw, or loss for a given team**. By achieving reliable predictive performance, this work aims to contribute a valuable analytical tool to the domain of sports analytics.

---

## 4. Technologies and Libraries Used

The project was developed in **Python**, using a comprehensive suite of widely adopted data science and machine learning libraries:

- **Pandas**: For robust data manipulation and analysis.  
- **NumPy**: For fundamental numerical operations and array handling.  
- **Matplotlib / Seaborn**: For in-depth data visualization and Exploratory Data Analysis (EDA).  
- **Scikit-learn (Sklearn)**: For machine learning model implementation, train-test splitting, categorical encoding, feature scaling, and evaluation metrics.  
- **Jupyter Notebook**: For an interactive development environment supporting iterative experimentation.  

---

## 6. Methodology

The project followed a structured pipeline to ensure reproducibility and reliability:

### 6.1 Data Cleaning and Preprocessing
- Removed irrelevant columns such as `comp` and `notes`.  
- Filled missing numerical values with median imputation.  
- Converted categorical variables (venue, opponent) into numerical form using label encoding.  
- Extracted **temporal features** (day-of-week, match time) from the `date` and `time` fields.  

### 6.2 Exploratory Data Analysis (EDA)
- Analyzed class distribution, revealing a moderate imbalance (more wins than draws or losses).  
- Visualized goals scored, shots on target, and win rates by venue.  
- Observed that home teams generally performed better than away teams.  

### 6.3 Feature Engineering
- Created **rolling averages** of goals, shots, and fouls to capture recent team performance trends.  
- Mapped match results into numerical outcome labels.  

### 6.4 Model Training and Evaluation
- Split the dataset chronologically into:
  - **Training Set**: Matches before 2022
  - **Testing Set**: Matches from 2022 onwards
- Trained a **Random Forest Classifier** with selected features.
- Evaluated performance using:
  - **Accuracy**
  - **Precision**
  - **Recall**
  - **Confusion Matrix**  
- Achieved ~47% precision on unseen data, with strong performance in predicting home wins and reduced accuracy for draws.

---

## 7. Project Impact

This project demonstrates the **practical application of machine learning in sports analytics**, providing a reproducible framework for predicting football match outcomes. The methodology can be extended to other leagues or sports, integrated into betting strategy tools, or adapted for real-time predictions with live match data. By transforming historical match statistics into actionable insights, the model supports data-driven decision-making for analysts, coaches, and fans.

    * scikit-learn
    
