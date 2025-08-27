# 🚢 Titanic-survival-prediction-using-ML-Model

*COMPANY NAME* : CODTECH IT SOLUTIONS 

*NAME*: MITTUL BASWALA

*INTERN ID*: CT06DZ2256

*DOMAIN*: DATA ANALYTICS

*MENTOR*: NEELA SANTOSH

# 📌 TASK DESCRIPTION  
This project is focused on predictive analysis using machine learning. The objective is to build a classification model that predicts whether a passenger survived the Titanic disaster based on demographic and travel-related features. The project demonstrates end-to-end data science workflow—from data preprocessing to model evaluation—while emphasizing clarity, reproducibility, and storytelling.



## 🎯 Objective  
- Perform **feature selection** to identify key predictors of survival  
- Train and evaluate **machine learning models** for classification  
- Document the process in a **clear, professional notebook** suitable for portfolio presentation  
- Showcase technical and analytical skills using real-world data  


## 📂 Dataset  
- **Source**: [Kaggle Titanic Dataset](https://www.kaggle.com/datasets/yasserh/titanic-dataset)  
- **File**: `Titanic.csv`  
- **Size**: ~891 rows  
- **Features**:
  - `PassengerId`, `Name`, `Sex`, `Age`, `SibSp`, `Parch`, `Ticket`, `Fare`, `Cabin`, `Embarked`, `Survived`


## ⚙️ Tools & Technologies  
- **Python 3.10+** – Core programming language  
- **Pandas** – Data manipulation and cleaning  
- **NumPy** – Numerical operations  
- **Matplotlib & Seaborn** – Data visualization  
- **Scikit-learn** – Machine learning models and evaluation  
- **Jupyter Notebook** – Interactive development and documentation  


## 🧪 Methodology  

### 1️⃣ Data Preprocessing  
- Dropped irrelevant columns: `PassengerId`, `Name`, `Ticket`, `Cabin`  
- Handled missing values:
  - Imputed `Age` using median  
  - Filled `Embarked` with mode  
- Encoded categorical variables:
  - `Sex` mapped to binary  
  - `Embarked` one-hot encoded  
- Engineered new feature:
  - `FamilySize = SibSp + Parch` to capture family influence on survival  

### 2️⃣ Feature Selection  
- Used **correlation matrix** to identify relationships between features and target  
- Applied **Random Forest feature importance** to rank predictors  
- Selected top features: `Sex`, `Pclass`, `Fare`, `Age`, `FamilySize`  
- Visualized feature relationships using heatmaps and bar plots  

### 3️⃣ Model Training  
- Split dataset into **training (80%)** and **testing (20%)** sets  
- Trained a **Random Forest Classifier** using Scikit-learn  
- Compared performance with baseline models (e.g., Logistic Regression)  
- Ensured reproducibility with fixed random seed  

### 4️⃣ Model Evaluation  
- Evaluated using:
  - **Accuracy**
  - **Precision**
  - **Recall**
  - **F1-score**
- Visualized:
  - **Confusion matrix**
  - **Classification report**
- Discussed strengths and weaknesses of the model  


## 🧠 Insights  
- **Gender** was the most influential predictor—female passengers had significantly higher survival rates  
- **Passenger class (Pclass)** showed strong correlation—first-class passengers had better survival odds  
- **Fare** and **Age** contributed meaningfully to survival prediction  
- **FamilySize** revealed that passengers with small families had higher survival rates  
- The model achieved **high accuracy and balanced precision/recall**, making it suitable for binary classification tasks  
- Visual storytelling helped uncover patterns that raw numbers alone couldn’t reveal  

## 📊 Visualizations  
- 📉 **Bar Plot**: Survival count by gender  
- 📊 **Histogram**: Age distribution of passengers  
- 🔥 **Heatmap**: Correlation matrix of numerical features  
- 🌊 **Boxplot**: Fare distribution across passenger classes  
- 🧮 **Feature Importance Plot**: Ranked predictors from Random Forest  
- 🧾 **Confusion Matrix**: Model performance breakdown  
<img width="778" height="527" alt="Image" src="https://github.com/user-attachments/assets/eb426112-a6d7-4181-af93-f55e87201d84" />
<img width="1076" height="741" alt="Image" src="https://github.com/user-attachments/assets/d5b24423-468d-447f-af39-2077eca6b949" />



