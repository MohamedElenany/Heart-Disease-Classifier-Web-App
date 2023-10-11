# Heart Disease Classifier Web App
## Main Objective and Business Value:
The project's objective is to predict the presence of heart disease in patients. It is designed for use by medical professionals, primarily relying on the patient's medical data collected during checkup examinations conducted by a doctor. This tool would offer significant value to doctors in their clinical practice, as diagnosing heart disease is often a challenging and complex task, involving expensive additional tests and reports. Therefore, having such a tool to assist in identifying and forecasting patient diagnoses would be highly beneficial and lead to substantial cost savings.

Disclaimer: This tool is NOT 100% accurate. There is no algorithm that can predict heart disease with absolute precision. However, if you choose to use this tool for medical purposes, please do so at your own discretion.

## Models Used:
I attempted to solve this problem using two different approaches, one was random forest classifiers and the other was decision trees with bagging. For both models, I performed hyperparameter tuning using 5-fold cross validation, which helped reduce overfitting and improve generalization accuracy. Both models were performing extremely well with both achieving 85%+ accuracy in most runs, but I decided to use the random forest classifier as it was achieving better accuracies and better stability during all runs on average. Another reason I selected the random forest is because it gives a better bias-variance tradeoff than bagging decision tree, and with faster computation time. The randomness in the forests decreases the correlation between decision trees in the forest, which results in decreasing the effects of overfitting and noise in the data.

## How to Run:
To run the web app, please clone the repository and execute the following command in the command line, while being in the same directory as the cloned repository:
```python app.py```

If you wish to review the notebook where I pre-processed the data and tested the models, navigate to the Notebooks folder and execute the notebook by running all code blocks consecutively.
