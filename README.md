# Microsoft-Classifying-Cybersecurity-Incidents-with-Machine-Learning

Project Overview :
This project focuses on building a machine learning model to classify cybersecurity incidents into True Positive (TP), Benign Positive (BP), and False Positive (FP) using Microsoft’s GUIDE dataset (4M+ records). The goal is to assist Security Operation Centers (SOCs) in automating incident triage, reducing false positives, and improving response times.

Problem Statement :
Develop a robust ML model that predicts incident triage grades based on historical evidence and customer responses. The model should generalize well to unseen incidents, enabling guided response systems to provide precise, context-rich recommendations to SOC analysts.

Business Use Cases :
- SOC Automation: Prioritize true threats and reduce analyst workload.
- Incident Response: Enable guided systems to suggest quick mitigation steps.
- Threat Intelligence: Improve detection by leveraging historical incident patterns.
- Enterprise Security: Reduce false positives, strengthening security posture.

Approach :
1. Data Preprocessing & Feature Engineering
   - Handled missing data, encoding, and scaling.
   - Stratified splitting to preserve class balance.

2. Model Training & Selection
   - Baseline: Logistic Regression, Decision Tree.
   - Advanced: Random Forest, XGBoost.
   - Addressed imbalance using class_weight='balanced'.

3. Hyperparameter Tuning
   - Used RandomizedSearchCV for Random Forest.
   - Optimized with F1-macro as primary metric.

4. Evaluation Metrics
   - Focused on Macro-F1 Score, Precision, Recall (class-imbalance aware).
   - Compared multiple models for best trade-off.

5. Final Model
   - Random Forest significantly outperformed Logistic Regression, Decision Tree, and XGBoost.
   - Tuned Random Forest Classifier selected as best performer.

Results :
1. Accuracy - 89%
2. Macro-F1 Score - 88%
3. Precision - 88%
4. Recall - 88%

Skills Demonstrated :
- Data Preprocessing & Feature Engineering
- Handling Imbalanced Datasets (class weights, stratified sampling)
- Model Training & Benchmarking (RF, XGBoost, Logistic Regression, Decision Tree)
- Hyperparameter Tuning (RandomizedSearchCV)
- Evaluation Metrics (Macro-F1, Precision, Recall, Confusion Matrix)
- Feature Importance (Permutation Importance)
- Model Deployment (Joblib)

Deliverables :
- Final Random Forest model (final_random_forest_model.pkl)
- Cleaned and processed dataset (cleaned_test_data.joblib)
- Source code with preprocessing, training, and evaluation pipelines
