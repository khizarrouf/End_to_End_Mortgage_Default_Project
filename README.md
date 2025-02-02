# End_to_End_Data_Science_Project
### Project Overview:
This project is an end-to-end data science initiative focused on developing a deep learning model to predict loan defaults. The primary tasks include comprehensive data preprocessing to handle noisy data, detection and removal of outliers, addressing missing values, data stratification, and implementing a custom batch sampler. The model is trained using an Artificial Neural Network (ANN) on MS Azure and deployed locally.

### Dataset Source:
The data for this project was sourced from the Freddie Mac website, consisting of two separate datasets: the Loan Origination and Loan Performance files. These datasets provide valuable information on loan details, borrower characteristics, and the performance of loans over time, which were used for model training.

### Problem Definition:
The goal of this project is to solve a binary classification problem, where the objective is to predict whether a loan will default (1) or not (0). The model is designed to identify high-risk loans to help financial institutions mitigate the risk of defaults.

### Key Technologies and Tools Used:
**Deep Learning:** An Artificial Neural Network (ANN) was employed for predicting loan defaults. The neural network architecture was trained to capture complex patterns in the data.  

**Data Processing:** Extensive data preprocessing was carried out, including cleaning the data, performing feature engineering, and applying feature scaling to improve model performance.  

**Outlier Detection:** Outliers were detected and removed using an unsupervised machine learning algorithm, Scalable Unsupervised Outlier Detection (SUOD), which helped improve the quality and robustness of the model.  

**Web Framework:** FastAPI was utilized to deploy the trained model locally.  

**Model Interpretability:** SHAP (Shapley Additive Explanations) was employed to enhance the interpretability of the model by explaining the contributions of each feature to the final predictions.  

**Model Performance Goals:** The primary goal of the model is to minimize false negatives (i.e., incorrectly classifying defaulting loans as non-defaulting). Another key performance metric is the ROC-AUC (Receiver Operating Characteristic - Area Under Curve), which provides insight into the model's ability to distinguish between the two classes (default vs. non-default) across various decision thresholds.  

### Key Considerations:
Class Imbalance: One of the significant challenges in this project was the class imbalance, as there are significantly more non-defaulting loans than defaulting loans. To address this, techniques such as class weighting and data stratification were employed to ensure the model had a balanced representation of both classes during training.
Computational Limitations: Due to computational constraints, only a subset of the dataset was used for model training. In future work, the model could be improved by leveraging additional computational resources.
