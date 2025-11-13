# Project Requirements

Researchers at CSU Fullerton’s College of Health and Human Development have been conducting a long running study to understand the factors affecting the physical health of college students. The attached dataset was collected as part of that study. One of the variables is Total Fitness Factor Score (column with header FFTotal) which is computed using a formula hidden from you. The goal of this project is to come up with an approximation of Total Fitness Factor Score for a subject using only the other available variables. 

# Approach
There are three steps in this project:

1. Exploratory data analysis to identify variables (and combinations of variables) that are correlated to Total Fitness Factor Score, and to discard variables that have lots of missing values. The dataset contains approximately 35 variables, so it is not realistic to explore every variable and combination of variables. For this project, it is sufficient to consider any 5 variables and visualize them with FFTotal. The attached Data dictionary file gives information on the units and meaning of the different columns. (Note: this file will not be read into the Python code. This is provided so that you can use your knowledge of physical fitness to pick variables.)

2. Linear modeling to develop a model to predict FFTotal using only the other variables, including any transformations.
- Generate some (at least 3) transformed variables. For example, these could combine variables (e.g., bmi = Wt / Ht**2).
- Split your dataset into equal-sized train and test subsets (randomly chosen): The train subset should be used for building/training the linear models. Use statsmodels or scikit-learn as appropriate.
- Run linear regression with at least 5 different combinations of predictor variables. -    Hint: a model created with the statsmodels formula API might look like:
FFTotal ~ Age + Wt + Waist

3. Evaluate the best linear model by comparing its predicted Fitness Score with the true value of FFTotal.
- Select the best of the 5 models for evaluation
- For your best models, report the Root Mean Squared Error (RMSE) and other relevant metrics comparing the predicted values and FFTotal for the test subset.

# Project checklist
Grading will be based on how complete your report is and if the Python code does the analysis correctly. It will NOT be based on how accurate is your approximation to total fitness factor score (though you should strive for higher accuracy).
- Every team member’s name
1. Data exploration
    - Code to load data
    - Visualized at least 5 variables with FFTotal
    - Split into test and train subsets
2. Modeling
    - Tried at least 5 different combinations of variables for modeling
    - Included at least 3 variable transformations
    - Code that correctly implements the above
3. Evaluation
    - Generate the R2 of all models
    - Identified the best model and calculated its RMSE
    - Code that correctly implements the above
4. Written report
    - Brief description of how variables were chosen for data modeling
    - Descriptions of variable transformations
    - A table that shows the R2 of the different models
    - RMSE of the best model from training using test data
    - A conclusion
    - Clarity of the report (e.g., appropriate section headings)
5. Code
    - Style: readability, use of Python modules, no unnecessary use of complex functions.
    - Code has adequate comments
    - Code contributes to the written report, but is not the report itself.
    - Note: include only the final code, i.e., do not submit errors or unused code
Submission on time
