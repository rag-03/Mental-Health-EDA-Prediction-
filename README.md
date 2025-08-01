# Mental-Health-EDA-Prediction-
🧠 Mental Health Analysis & Prediction This project performs end-to-end data preprocessing, exploratory data analysis (EDA), and predictive modeling to classify individuals based on mental health and lifestyle indicators.

🔍 Overview We analyze multiple datasets related to health, lifestyle, and survey responses. After combining them, we handle missing values, drop redundant features, encode categorical data, scale numerical values, and build a predictive model using machine learning.

📁 Dataset Description Combined from: df1 to df7

Rows: ~100,000

Key features: lifestyle habits, medical test results, mental health indicators

Target column: target (mental health classification)

⚙️ Workflow Data Merging

Merged 7 different CSV files into one unified DataFrame.

Data Cleaning & Preprocessing

Dropped columns like bmi_estimated, gene_marker_flag, survey_code, etc.

Imputed missing numerical values using median, and categorical with mode.

Removed outliers based on IQR method.

Applied label encoding for binary/categorical features.

Used pd.get_dummies() for multi-class categorical columns.

Feature Engineering

Removed redundant and correlated features.

Identified numerical, categorical, and boolean columns.

Model Building

Trained a RandomForestClassifier.

Achieved ~95.63% accuracy on the test set.

Encapsulated preprocessing steps in a pipeline.

📊 Key Techniques Used pandas, numpy – Data wrangling

matplotlib, seaborn – EDA and visualization

scikit-learn – Modeling, pipeline, evaluation

Label Encoding, One-Hot Encoding

Feature Scaling, Outlier Detection

Train-Test Split & Accuracy Evaluation

📈 Results Model Accuracy Random Forest (Base) 95.63%

🧪 Future Work Hyperparameter tuning with GridSearchCV

Try XGBoost / LightGBM

Perform SHAP-based feature importance

Deploy as a Streamlit web app

📦 Requirements bash Copy Edit pip install pandas numpy scikit-learn matplotlib seaborn 🚀 How to Run Clone the repo or open the .ipynb file in Jupyter/Colab.

Run the cells sequentially.

Modify preprocessing steps as needed.
