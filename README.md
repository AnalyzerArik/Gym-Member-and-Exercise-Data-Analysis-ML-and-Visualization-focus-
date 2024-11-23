# Data Analysis of Gym Members and Exercise Data 
#### [Jupyter nbviewer link](https://nbviewer.org/github/AnalyzerArik/Gym-Member-and-Exercise-Data-Analysis-ML-and-Visualization-focus-/blob/main/gym-member-data-analysis-2.ipynb)

## Description
Project consists of using synthetic gym member and exercise data to mainly see if it were possible to predict a member's BMI category using machine learning techniques.
I also focused on Plotly-dominant visualization, which is why I recommend viewing this analysis in nbviewer. [Open the analysis in nbviewer to view visualizations.](https://nbviewer.org/github/AnalyzerArik/Gym-Member-and-Exercise-Data-Analysis-ML-and-Visualization-focus-/blob/main/gym-member-data-analysis-2.ipynb)

## Data Overview
- **Dataset:** Gym Member and Exercise Data  
- **Rows:** 973  
- **Columns:** 15 (e.g., weight, calories burned, experience level, workout types, fat percentage)  
- **Source:** [Kaggle Dataset](https://www.kaggle.com/datasets/valakhorasani/gym-members-exercise-dataset)

## Methodology
1. Data cleaning and preprocessing.
2. Exploratory Data Analysis (EDA) to visualize trends (BMI focused).
3. Statistical analysis to find correlations.
4. Machine Learning model training and testing.
5. Insights derived from the data analysis machine learning performance.

## Key Findings
- The dataset definitely needs additional, stronger features for a reliable prediction model.
- SVC (Support Vector Classifier) outperformed other models due to its balance between precision, recall, and accuracy.
- HIIT, while effective for weight loss, has lower adoption rates, likely due to its high-intensity nature.
- A moderate positive correlation with males being likelier to be obese than females.

## Tools and Libraries Used
- **Python Libraries:** Pandas, NumPy, Matplotlib, Seaborn, Plotly, SKLearn
- **Tools:** Jupyter Notebook
