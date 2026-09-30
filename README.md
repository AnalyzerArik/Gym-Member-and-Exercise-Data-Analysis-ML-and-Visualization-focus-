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

An earlier portfolio project using synthetic gym-member data to practice data preparation, interactive reporting, and classification-model evaluation. Its relevance to analyst and BI roles is in defining categories, comparing groups, and communicating performance tradeoffs and limitations.

[Current analyst portfolio](https://github.com/AnalyzerArik/AnalyzerArik)

For interactive visualizations:
[View the Analysis in nbviewer](https://nbviewer.org/github/AnalyzerArik/Gym-Member-and-Exercise-Data-Analysis-ML-and-Visualization-focus-/blob/main/gym-member-data-analysis-2.ipynb)

---

## **Dataset Description**

- **Source**: [Kaggle Dataset](https://www.kaggle.com/datasets/valakhorasani/gym-members-exercise-dataset)  
- **Rows**: 973  
- **Columns**: 15  
  - Example columns: `Weight (kg)`, `Calories_Burned`, `Experience_Level`, `Workout_Type`, `Fat_Percentage`.  

---

## **Project Objectives**

- Summarize the synthetic dataset by workout type and notebook-defined BMI category.
- Build interactive Plotly visualizations to compare groups.
- Compare classification models using test-set metrics and cross-validation, with explicit limits on interpretation.

---

## **Installation and Setup**

The linked notebook contains saved outputs for review. To work locally:

```bash
git clone https://github.com/AnalyzerArik/Gym-Member-and-Exercise-Data-Analysis-ML-and-Visualization-focus-.git
cd Gym-Member-and-Exercise-Data-Analysis-ML-and-Visualization-focus-
python -m pip install jupyter pandas numpy matplotlib seaborn plotly scikit-learn xgboost catboost termcolor pillow
jupyter notebook
```

The repository does not include a `requirements.txt` or the input CSV. Download the dataset linked above and supply `gym_members_exercise_tracking.csv` at the notebook's input path. The first code cell also opens an unbundled decorative image, `89.png`; remove that image-loading/display block or provide the file before running it. Dependencies are not pinned, and a clean-environment rerun has not been verified.

---

## **Project Workflow**

### **Data Preprocessing**

- Checked completeness; the saved output reports no missing values in the 15 input columns.
- Converted weight and height units and created BMI categories and encoded features.
- Applied scaling within selected model pipelines.

### **Exploratory Data Analysis (EDA)**

- Compared category counts and feature distributions.
- Used interactive Plotly charts alongside matplotlib and seaborn visualizations.

### **Machine Learning**

- Compared logistic regression, random forest, XGBoost, CatBoost, SVC, and gradient boosting.
- Used grid search, classification reports, confusion matrices, and cross-validation to examine performance.

### **Summary**

- Demonstrates reporting and model-comparison techniques on synthetic data; it does not establish real-world fitness or health outcomes.

---

## **Key Findings**

1. **Category definitions shape reporting.** The saved notebook counts 163 Underweight, 371 Healthy, 242 Overweight, and 197 Obese records, totaling 973. These use the notebook's bin edges of 0, 18.4, 24.9, 29.9, and infinity; counts are specific to those definitions.
2. **The final model comparison has tradeoffs.** The saved classification reports and five-fold cross-validation outputs show:

| Model | Test accuracy* | Weighted precision* | Mean CV accuracy |
| --- | ---: | ---: | ---: |
| XGBoost | 0.64 | 0.68 | 0.6016 |
| SVC | 0.64 | 0.69 | 0.6376 |
| Logistic regression with polynomial features | 0.62 | 0.64 | 0.6402 |

*Test metrics are rounded as printed in the saved reports, with 195 test records. SVC and XGBoost tie on reported test accuracy; logistic regression has the highest mean CV accuracy among these three. These results do not establish a clear overall winner.

### **Interpretation limits**

- The data is synthetic. Group differences do not establish real-world obesity prevalence, workout effectiveness, or reasons for workout preferences.
- BMI categories are derived from the existing BMI field. Classification is a modeling exercise, not a demonstrated operational need or validated health application.
- The notebook's tuned-model comparison chart contains manually entered scores and training/test-label inconsistencies. The table above uses printed evaluation outputs, not that chart.
- The historical notebook's conclusion that SVC has the highest mean CV accuracy conflicts with its saved results. This README corrects that interpretation; notebook code and outputs are preserved.
- Feature selection and repeated comparisons on the same test set limit the strength of generalization claims. Independent validation is needed before treating any model as reliable.

## **Tools and Technologies**

- **Programming Language**: Python  
- **Libraries**:  
  - `pandas` for data manipulation  
  - `numpy` for statistical calculations  
  - `matplotlib` and `seaborn` for visualizations
  - `plotly` for interactive visualizations
  - `scikit-learn`, `xgboost`, and `catboost` for model evaluation
- **Platforms**: Kaggle and JupyterLab for notebook analysis.

---

## **Future Work**

- Reconcile chart labels and manually entered scores with the evaluation outputs.
- Standardize category boundaries across code and chart annotations.
- Add reproducible inputs and pinned dependencies, compare against a simple baseline, and use an independent final evaluation set.

These are proposed improvements, not completed analyses.

---

## **Acknowledgments**

Special thanks to the dataset creator on Kaggle and the broader data science community for inspiring this project.
