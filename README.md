# Data Analysis of Gym Members and Exercise Data

---

## **Table of Contents**
1. [Introduction](#introduction)  
2. [Dataset Description](#dataset-description)  
3. [Project Objectives](#project-objectives)  
4. [Installation and Setup](#installation-and-setup)  
5. [Project Workflow](#project-workflow)  
6. [Key Findings](#key-findings)  
7. [Tools and Technologies](#tools-and-technologies)  
8. [Future Work](#future-work)  
9. [Acknowledgments](#acknowledgments)  

---

## **Introduction**
This project explores synthetic gym member and exercise data to predict a member's BMI category using machine learning techniques. The analysis also emphasizes Plotly-dominant visualizations to present findings effectively.  

For the best viewing experience, use the following link to access the notebook with interactive visualizations:  
[View the Analysis in nbviewer](https://nbviewer.org/github/AnalyzerArik/Gym-Member-and-Exercise-Data-Analysis-ML-and-Visualization-focus-/blob/main/gym-member-data-analysis-2.ipynb)

---

## **Dataset Description**
- **Source**: [Kaggle Dataset](https://www.kaggle.com/datasets/valakhorasani/gym-members-exercise-dataset)  
- **Rows**: 973  
- **Columns**: 15  
  - Example columns: `Weight`, `Calories Burned`, `Experience Level`, `Workout Types`, `Fat Percentage`.  

---

## **Project Objectives**
- Predict gym members’ BMI categories using machine learning models.  
- Analyze trends in workout habits and their correlation with body composition.  
- Develop clear, Plotly-dominant visualizations to enhance understanding.  

---

## **Installation and Setup**
1. Clone the repository:
   ```bash
   git clone https://github.com/AnalyzerArik/Gym-Member-and-Exercise-Data-Analysis-ML-and-Visualization-focus.git
2. Navigate to the project directory:
   ```bash
   cd Gym-Member-and-Exercise-Data-Analysis-ML-and-Visualization-focus
3. Install the required libraries:
   ```bash
   pip install -r requirements.txt
4. Run the Jupyter Notebook:
   ```bash
   jupyter notebook

   
## **Project Workflow**

### **Data Preprocessing**
- Cleaned the dataset by handling missing values and formatting features.
- Standardized data for compatibility with machine learning models.

### **Exploratory Data Analysis (EDA)**
- Visualized trends focusing on BMI distribution and correlations.
- Used interactive Plotly visualizations to present findings.

### **Machine Learning**
- Trained and tested several machine learning models to predict BMI categories.
- Evaluated model performance based on precision, recall, and accuracy metrics.

### **Summary**
- Derived actionable insights from data exploration and machine learning results.

---

## **Key Findings**
1. The dataset requires additional, stronger features for reliable prediction models.
2. **SVC (Support Vector Classifier):** Outperformed other models due to its balance between precision, recall, and accuracy.
3. **HIIT Popularity:** While effective for weight loss, HIIT has lower adoption rates, likely due to its high-intensity nature.
4. **Gender Trends:** Males are moderately more likely to be obese than females.


## **Tools and Technologies**
- **Programming Language**: Python  
- **Libraries**:  
  - `pandas` for data manipulation  
  - `numpy` for statistical calculations  
  - `matplotlib` and `seaborn` for visualizations
  - sklearn for machine learning
- **Platforms**: Kaggle Notebook for analysis and presentation.

---

## **Future Work**
- Enhance the dataset with more diverse and impactful features.
- Explore advanced machine learning models such as neural networks for BMI prediction.
- Analyze the long-term impacts of specific workout types on body composition.

---

## **Acknowledgments**
Special thanks to the dataset creator on Kaggle and the broader data science community for inspiring this project.
