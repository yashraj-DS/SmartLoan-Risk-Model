# SmartLoan-Approval-Risk-Model
Building smarter loan approval decisions by combining machine learning with business-driven risk control.
________________________________________
### 📌 Project Overview  
This project builds multiple machine learning models to predict loan approval decisions under different business priorities.
Instead of selecting a single “best” model, this system provides three decision strategies, allowing the bank to choose the model based on its current risk appetite and growth goals.  
The objective is not just prediction — but controlled decision-making.  

### 🎯 Business Objective  
Loan approval systems must balance:  
•	Reducing risky approvals (minimizing financial loss)
•	Maintaining customer growth
•	Optimizing overall operational performance
This project translates those priorities into three deployable model strategies.  
________________________________________
### 🤖 Final Model Strategies  
After evaluation, three final decision configurations were selected:
________________________________________
#### 🔴 1️⃣ Risk-Control Priority (Minimize Wrong Approvals)    
Model: Logistic Regression  
Threshold: 0.72  
•	Precision (Class 1): 77%  
•	Recall: 91%  
•	Accuracy: 76%  
•	False Positives: 33  
•	False Negatives: 11  
📌 Use when minimizing risky approvals is the primary concern.  
________________________________________
#### 🟡 2️⃣ Balanced Growth Strategy  
Model: Logistic Regression  
Threshold: 0.66  
Balanced trade-off between:  
•	Revenue growth  
•	Risk control  
•	Operational stability  
📌 Use when business wants sustainable growth with controlled exposure.  
________________________________________
#### 🟢 3️⃣ High Recall Strategy  
Model: K-Nearest Neighbors  
Threshold: 0.70  
Confusion Matrix (KNN):  
[[49 16]  
 [55 65]]  
Logistic (Model 2 comparison):  
•	Precision (Class 1): 0.80  
•	Recall (Class 1): 0.54  
•	Accuracy: 62%  
📌 Use when capturing maximum potential approvals is important, even if false positives increase slightly.  
________________________________________
### 📊 Key Technical Highlights  
•	Proper preprocessing (encoding + scaling without leakage)  
•	Hyperparameter tuning using GridSearchCV  
•	Precision-based optimization  
•	Manual threshold tuning  
•	Precision–Recall curve analysis  
•	Confusion matrix comparison across models  
•	Business-driven model selection framework  
________________________________________
### 🧠 Core Insight  
There is no single “best” model.  
Model performance depends on business objectives.  
By adjusting thresholds and comparing models, we convert machine learning output into strategic decision options.  
________________________________________
### 🛠 Tech Stack  
• Python  
• Pandas  
• NumPy  
• Matplotlib  
• Scikit-learn  
________________________________________
### 🌟 Final Thought  
This project demonstrates how machine learning can support real-world decision systems by aligning model performance with business priorities — rather than relying on accuracy alone.
