# 💳 Credit Risk Prediction
 
🚀 *Objective:* Build a classification model to predict *credit risk*. Multiple machine learning algorithms are implemented and compared for performance evaluation.
  
## 📦 1. Import Libraries
 
The following libraries were used:
 
 
- numpy, pandas: Data manipulation and analysis.
 
- matplotlib, seaborn: Data visualization.
 
- sklearn: Model training, evaluation, and preprocessing.
 

  
## 📂 2. Load Data
 
Read the dataset *credit_risk_dataset.csv* into a pandas DataFrame for analysis:
 `df = pd.read_csv('credit_risk_dataset.csv') `  
## 🔍 3. Exploratory Data Analysis (EDA)
 
Initial data exploration included:
 
 
- df.info() ➜ Check dataset structure and data types.
 
- df.describe() ➜ Get basic statistics (mean, std, min, max, etc.).
 
- *Target Distribution Visualization*:
 

 `sns.countplot(x='loan_status', data=df, palette='Set2') plt.title("Class Distribution (Loan Status)") plt.show() `  
## 🛠 4. Handling Missing Values
 
 
- Filled missing values in person_emp_length and loan_int_rate columns with their *median* values to ensure no data loss.
 

  
## 🔑 5. Encoding Categorical Features
 
 
- Applied LabelEncoder on binary categorical features: loan_grade, cb_person_default_on_file.
 
- Used pd.get_dummies() to one-hot encode person_home_ownership and loan_intent.
 

  
## ✂ 6. Train/Test Split & Scaling
 
 
- Split data into *80% training* and *20% testing* sets.
 
- Standardized features using StandardScaler to improve model performance.
 

  
## 📈 7. Logistic Regression
 
 
- Trained a Logistic Regression model.
 
- Evaluated using Accuracy, Precision, Recall, F1 Score, and ROC-AUC.
 
- Visualized results in a *bar chart*.
 

  
## 🌳 8. Decision Tree Classifier
 
 
- Built a Decision Tree model.
 
- Evaluated with the same metrics and visualized results.
 

  
## 🌲 9. Random Forest Classifier
 
 
- Implemented Random Forest for improved predictive power.
 
- Evaluated metrics and plotted bar chart results.
 

  
## 📊 10. Model Comparison
 
 
- Compared all three models side by side using bar charts for metrics: *Accuracy, Precision, Recall, F1 Score, ROC-AUC*.
 
- Results showed that ensemble methods like *Random Forest* generally provide better performance.
 

  
### 💡 Summary
 
This project demonstrates a full *end-to-end machine learning pipeline*: ✔ Data Cleaning & Preprocessing ✔ Feature Encoding & Scaling ✔ Model Training with Multiple Algorithms ✔ Visualization & Comparison of Model Performance
 
🔗 Perfect starting point for building scalable and interpretable credit risk models!
