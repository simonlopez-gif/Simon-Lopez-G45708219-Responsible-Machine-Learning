# Simon-Lopez-G45708219-Responsible-Machine-Learning
Assignment 1: Reproducing the COMPAS analysis in Python

## Purpose of the analysis

The purpose of this project is to redo the COMPAS analysis from class in Python. The original version we worked from was in R, so I translated the main parts into Python and tried to keep the same steps and results. This includes loading the data, cleaning it, looking at summary tables and graphs, running the logistic regression model, and checking the model results with confusion matrices and race-level metrics.

My goal was to make the Python version match the class workflow as closely as possible.

## Python libraries used

The main libraries I used were:

- pandas
- matplotlib
- statsmodels
- scikit-learn
- math

## Instructions for reproducing the results

1. Open the notebook in Jupyter Notebook or Google Colab.
2. Install the libraries if needed.
3. Run the cells in order.
4. Make sure you have internet access because the dataset is loaded from GitHub.
5. Keep the notebook in order because some later cells depend on earlier ones.

## Notes

I tried to keep the code simple and close to what we did in class. Some outputs may look a little different from R, but the main logic is the same.

## Acknowledgment
I completed this assignment myself. I used ChatGPT only for limited help with debugging, syntax questions, and fixing coding errors during the Python translation process.

# Assignment 2: Explaining the COMPAS Replacement Model

## Purpose of the analysis

The purpose of this assignment is to apply explainability methods to the COMPAS replacement model we worked on in class. Using the cleaned COMPAS dataset from the earlier part of the notebook, I followed the same main pipeline from Lecture 02 and then used different explanation tools to understand how the model behaves. The analysis includes training a logistic regression model and a gradient-boosted tree model, comparing their performance across racial groups, and then using SHAP, LIME, and DiCE to explain individual predictions.

The main goal was not only to get predictions, but also to understand why the model made those predictions and what that means from a governance point of view. I looked at the highest-risk and lowest-risk defendants in the racial groups used in the homework and compared how different explanation methods behaved on the same individuals.

## Python libraries used

The main Python libraries I used were:

- pandas
- numpy
- matplotlib
- scikit-learn
- shap
- lime
- dice-ml

I also used standard Python functions and notebook cells from the earlier part of the assignment for data cleaning and setup.

## Instructions for reproducing the results

1. Open the notebook in Jupyter Notebook or Google Colab.
2. Run the data cleaning and preprocessing cells first, since the Homework 2 section depends on the cleaned COMPAS dataset created earlier in the notebook.
3. Make sure the needed libraries are installed, especially `shap`, `lime`, and `dice-ml`.
4. Run the Homework 2 cells in order from top to bottom.
5. The dataset is loaded from GitHub, so internet access is needed.
6. Do not skip cells, because later explanation steps depend on the models and variables created earlier.

## Notes

I tried to keep the code close to the class pipeline from Lecture 02 while still making sure it worked correctly in Python. Some outputs may look a little different from the slides, but the main logic and explanation steps are the same.

## Acknowledgment
I completed this assignment myself. I used ChatGPT only for limited help with debugging, syntax questions, and fixing coding errors during the Python translation process. And correcting governace memo


## Assignment 3: Disparate Impact Audit of the COMPAS Model

## Purpose of the analysis
The purpose of this assignment is to apply fairness and disparity testing methods to the COMPAS model we worked with in class. Using the cleaned COMPAS dataset and the model pipeline already built in the notebook, I followed the general approach from Lecture 03 and evaluated whether the model produced different outcomes across protected groups. The analysis includes calculating adverse impact ratio (AIR), marginal effect (ME), and standardized mean difference (SMD), separately for race and sex. I also added an intersectional analysis using race × sex subgroups, computed false positive rate (FPR) and false negative rate (FNR) by race, and used a two-proportion z-test to check statistical significance.

The main goal of this assignment was not just to measure model performance, but to test whether the model may create fairness concerns across groups. In other words, the focus here was on bias measurement and compliance-style auditing rather than only prediction accuracy. I also compared practical significance and statistical significance, since both matter when interpreting disparity results.

## Python libraries used
The main Python libraries I used were:
	•	pandas
	•	numpy
	•	matplotlib
	•	scikit-learn
	•	statsmodels
	•	solas-ai-disparity

I also used standard Python functions and notebook cells from the earlier part of the notebook for data cleaning, preprocessing, and model generation.

## Instructions for reproducing the results
	1.	Open the notebook in Jupyter Notebook or Google Colab.
	2.	Run the data cleaning and preprocessing cells first, since the Assignment 3 section depends on the cleaned COMPAS dataset created earlier in the notebook.
	3.	Make sure the needed libraries are installed, especially statsmodels and solas-ai-disparity.
	4.	Run the Assignment 3 cells in order from top to bottom.
	5.	Do not skip cells, because the fairness audit section depends on the model and test-set variables already created earlier in the notebook.

## Notes
I tried to keep the code close to the class pipeline from Lecture 03 while also making sure it worked correctly in Python. Some results, especially for very small subgroups, should be interpreted carefully because small sample sizes can make disparity estimates unstable.

## Acknowledgment
I completed this assignment myself. I used ChatGPT only for limited help with debugging, syntax questions, fixing coding errors during the Python translation process, and improving the wording of the compliance memo.


