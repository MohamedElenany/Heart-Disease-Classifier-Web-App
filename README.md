# Heart Disease Classifier Web App
## Main Objective and Business Value:
The project's objective is to predict the presence of heart disease in patients. It is designed for use by medical professionals, primarily relying on the patient's medical data collected during checkup examinations conducted by a doctor. This tool would offer significant value to doctors in their clinical practice, as diagnosing heart disease is often a challenging and complex task, involving expensive additional tests and reports. Therefore, having such a tool to assist in identifying and forecasting patient diagnoses would be highly beneficial and lead to substantial cost savings.

Disclaimer: This tool is NOT 100% accurate. There is no algorithm that can predict heart disease with absolute precision. However, if you choose to use this tool for medical purposes, please do so at your own discretion.

## Producing Results:
**Data Pre-processing:** The dataset from UCI, containing 920 instances and 16 features, underwent rigorous cleaning and enhancement. Irrelevant columns were removed, and the dataset was prepared for modeling with one-hot encoding for categorical data. Multicollinearity issues were addressed to eliminate redundant information. Additionally, mode substitution was used to handle missing data. Columns with significant missing data were retained due to their correlations with the outcome, and their missing values were imputed.
**Models Used:** I attempted the problem through two distinct approaches: random forest classifiers and decision trees with bagging. In pursuit of optimal performance, I engaged in hyperparameter tuning for both models, employing 5-fold cross-validation to mitigate overfitting and enhance generalization accuracy. Remarkably, both models consistently demonstrated exceptional performance, however, my preference leaned toward the random forest classifier due to its superior accuracy and enhanced stability across all runs, on average. Another factor influencing my choice was the random forest's ability to strike a better bias-variance tradeoff compared to bagging decision trees, all while maintaining faster computation times. The inherent randomness within random forests substantially diminishes the correlation between the decision trees, thereby reducing the adverse effects of overfitting and noise in the data.
**Test Results:** By employing the random forest classifier on the pre-processed data, the model achieved a testing accuracy performance of 90%.

## How to Run:
To run the web app, please clone the repository and execute the following command in the command line, while being in the same directory as the cloned repository:
```python app.py```

If you wish to review the notebook where I pre-processed the data and tested the models, navigate to the Notebooks folder and execute the notebook by running all code blocks consecutively. For additional details, please refer to the project report provided above.
