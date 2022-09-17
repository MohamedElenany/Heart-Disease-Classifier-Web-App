# Heart Disease Classifier Web App
## About:
The aim of the project is to be able to predict whether a patient has heart disease or not. The project is intended to be used by doctors as most of the inputs consist of the medical data of the patient that are observed by a doctor following having a patient’s checkup report. There are many types of heart disease, and sometimes detecting them given the patient report and his symptoms may be troublesome for the doctor without further scans and reports that are mostly very costly. Even though the program is not 100% accurate, it is able to give a somewhat close to true prediction of the result of the patient. 

Disclaimer: This tool is NOT 100% accurate. There exists no algorithm can predict heart disease with absolutely no error. Nevertheless, if you choose to use this tool for medical purposes, please do so at your own discretion.

## Models Used:
I attempted to solve this problem using two different approaches, one was random forest classifiers and the other was decision trees with bagging. For both models, I performed hyperparameter tuning using 5-fold cross validation, which helped reduce overfitting and improve generalization accuracy. Both models were performing extremely well with both achieving 85%+ accuracy in most runs, but I decided to use the random forest classifier as it was achieving better accuracies and better stability during all runs on average. Another reason I selected the random forest is because it gives a better bias-variance tradeoff than bagging decision tree, and with faster computation time. The randomness in the forests decreases the correlation between decision trees in the forest, which results in decreasing the effects of overfitting and noise in the data.

## How to Run:
In order to run the web-app, please clone the repository and run the following prompt in the command line while inside the same directory of the cloned repository:
``` python app.py  ```

If you would like to take a look at the notebook where I pre-processed the data and tested the models, please run the notebook in the Notebooks folder and run all blocks of code consecutively

The pre-processed data is acquired from the UCI heart disease dataset
