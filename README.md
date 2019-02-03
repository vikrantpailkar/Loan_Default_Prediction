# Loan Default Prediction

Author: Vikrant

## Objective
Objective of this project is modeling loan default prediction system by using `Lending Club` data.

## Data Description
Source: [Kaggle Dataset: Lending Club Loan Data](https://www.kaggle.com/wendykan/lending-club-loan-data)
> These files contain complete loan data for all loans issued through the 2007-2015, including the current loan status (Current, Late, Fully Paid, etc.) and latest payment information. The file containing loan data through the "present" contains complete loan data for all loans issued through the previous completed calendar quarter. Additional features include credit scores, number of finance inquiries, address including zip codes, and state, and collections among others. The file is a matrix of about 890 thousand observations and 75 variables. A data dictionary is provided in a separate file.

## Data
* `loan.csv`: 63.6MB (compressed)
* Training Data: 221,712
* Test Data    : 55,428

## Environments
* Python 3.5
* TensorFlow 1.2.1
* Keras 2.0
* scikit-learn 0.18.2
* pandas 0.20.2
* seaborn 0.7.1
* (Optional) imbalanced-learn 0.2.1 (for upsampling by SMOTE)

## Example
Example file can be executed by:
```bash
$ python main.py
```
Dataset should be located in `.data/` directory.

## Performance
1. 3-class("bad", "warning" and "safe" loan) classifying: Approximately 90~94% accuracy
2. 2-class("bad" and "safe") classifying: Approximately: > 98.5% accuracy

## Work-Flow
1. Pre-processing
	* Data Overview
	* Handling Null Valued Features
	* Categorizing Target Variable
2. Feature Engineering with Exploratory Data Analysis
	* Feature Inspection
	* Visualizing Features
	* Handling Missing Values
	* One-Hot Encoding
	* Train-Test Data Split
	* (optional) Oversampling by SMOTE
3. Modeling
	* Label Encoding for Training
	* Neural Network Modeling
	* Structure of neural network Optimization and hyper-parameter Tuning with AWS p2.xlarge (Tesla K80) Instance.
4. Performance
	* Performance on a test set.
	* Confusion Matrix
5. More..

Detailed explanation is provided by [Notebook](https://nbviewer.jupyter.org/github/vikrantpailkar/Loan_Default_Prediction/blob/master/Loan_Default_Prediction.ipynb)
