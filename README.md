# Loan Lending Model #

Model developed by the George Washington University Summer Class 2021 
Responsible Machine Learning w/ Professor Patrick Hall

Last updated: June 2021

***
## Intended use
* Describe the business value of your group's best remediated model
The purpose of our group business model is to decide whether to lend money or not to a person who has a higher priced mortgage rate. As a result, we need to increase the sign from high price loans? 

* Describe how your group's best remediated model is designed to be used
Our group best model EBM designed to fit with random grid search, and then we need to avoid the discrimination probelm when we find the best cutoff point for Balck vs white AIR. Therefore, it is designed to avoid the discrimination probelm. 

* Describe the intended users for your group's best remediated model
  The intended user for our group best remediated model would be student, professor, 
and researchers who need a specific sample to make certain conclusions.  

* State whether your group's best remediated model can or cannot be used for any additional purposes 
 This model needs more data  in order to make more accuracy. So, it is used only for educational purposes not intended to evaluate the real-world problem.  

***
## Training data
* State the source of training data
* State how training data was divided into training and validation data
* State the number of rows in training and validation data
* Dene the meaning of all training data columns
* Dene the meaning of all engineered columns

***
## Evaluation data
* State the source of evaluation (or test) data
* State the number of rows in evaluation (or test) data
* State any differences in columns between training and evaluation (or test) data

***
## Model details
*  **Input columns include:** ['property_value_std',
               'no_intro_rate_period_std',
               'loan_amount_std',
               'income_std',
               'conforming',
               'intro_rate_period_std',
               'debt_to_income_ratio_std',
               'term_360']
*  **Target columns:** ['high_priced']
*  **Model Type:** Explainable Boosting Machine
*  **Software Implmented:** Python Virtual Environment
*  **Modeling software versions:**  we need to insert our link. currently using professor’s text file link [View software and package versions](https://github.com/jphall663/GWU_rml/blob/master/assignments/requirements.txt)
*  **Parameter settings:** {'max_bins': 512,
              'max_interaction_bins': 16,
              'interactions': 10,
              'outer_bags': 4,
              'inner_bags': 0,
              'learning_rate': 0.001,
              'validation_size': 0.25,
              'min_samples_leaf': 5,
              'max_leaves': 5,
              'early_stopping_rounds': 100.0,
              'n_jobs': 4, 
              'random_state': 12345}


***
## Quantitative analysis
* State the metrics used to evaluate your group's best remediated model
Our group decided to use AUC to evaluate our model. After, we run through the stress testing, residual analyze, remove the outlier. 

* State the values of the metrics for training, validation, and evaluation (or test) data { eval-
uation (or test) metrics come from the most recent class full evaluation results, link under
Assignment 1.
* Provide at least one plot or table from each weekly assignment for a total of at least six plots, that must include the global variable importance and partial dependence of your group's best remediated model.
* Address other alternative models considered

***
## Ethical considerations
* Describe potential negative impacts of using your group's best remediated model:
* Consider math or software problems
* Consider real-world risks: who, what, when and how?
* Describe potential uncertainties relating to the impacts of using your group's best remediated model:
* Consider math or software problems
* Consider real-world risks: who, what, when and how?
* Describe any unexpected or results encountered during training
