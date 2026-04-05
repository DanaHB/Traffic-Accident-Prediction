# Traffic Accident Analysis & Predictive Modeling
### Focus: Data Management, Strategic Feature Engineering, and Statistical Visualization

## 1. Project Overview
This project presents a comprehensive study on traffic accident data, aiming to identify key risk factors and predict accident occurrences. The core objective is to demonstrate how **Data Management** and analytical preprocessing can transform raw environmental and behavioral data into actionable safety insights.

## 2. Methodology & Data Pipeline
The project follows a structured data science pipeline, emphasizing the importance of feature quality over simple model application:
* **Data Management:** Implemented a robust pipeline for data cleaning, handling missing values, and categorical encoding for variables such as `Weather` and `Road_Type`.
* **Strategic Feature Engineering:** A key technical decision was the creation of the **`Age_Experience`** interaction feature. By analyzing the high linear correlation between `Driver_Age` and `Driver_Experience` in the dataset, these variables were merged to eliminate redundancy and better represent "Driving Wisdom."
* **Exploratory Data Analysis (EDA):** Leveraged statistical visualization to uncover non-obvious patterns between accident frequency and factors like `Speed_Limit` and `Light_Conditions`.
* **Predictive Modeling:** Deployed a **Random Forest Classifier** to evaluate the impact of the processed data. The **`Age_Experience`** feature was statistically validated as the **Most Influential Predictor**, outperforming all raw individual features.

## 3. Analytical Observations (Model Performance)
* **Accuracy:** The model achieved a baseline accuracy of **69.4%**.
* **Model Bias Insight:** Evaluation through Confusion Matrices indicated a predictive bias toward the majority class (No Accident). This serves as a critical study on **Class Imbalance** in real-world, small-scale datasets (843 rows) and highlights the necessity of data-centric AI refinement.

## 4. Future Roadmap
* **Advanced Balancing:** Integrating **SMOTE** (Synthetic Minority Over-sampling Technique) to improve sensitivity toward accident cases.
* **Algorithm Tuning:** Implementing cost-sensitive learning by adjusting **Class Weights** within the classifier.

## 5. Implementation Files
* [Source Code (Colab Notebook)](./DataManagementAndVisualizationProject.ipynb)
* [Technical Report (PDF)](./Data Management Project.pdf)
