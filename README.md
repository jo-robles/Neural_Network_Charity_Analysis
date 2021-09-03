# Neural_Network_Charity_Analysis

# Overview

In order to predict whether applicants will be successful if funded by Alphabet Soup, we utilize machine learning to predict whether or not the applicant will have success.

# Results

## Data Preprocessing

* What variable(s) are considered the target(s) for your model?
 * As we are interested in exploring an applicant's success, we are specifically interested in the "IS_SUCCESSFUL" column.
* What variable(s) are considered to be the features for your model?
 * The features of our model are: 
   * Status
   * Ask_Amt
   * Application_Type
   * Affiliation
   * Classification
   * Use_Case
   * Organization
   * Income_Amt
   * Special Considerations
  * Of specific note here is that when preprocessing the data, the following columns where further binned out:
   * Application_Type
   * Affiliation
   * Classification
   * Use_Case
   * Organization
   * Income_Amt
   * Special_Considerations
* What variable(s) are neither targets nor features, and should be removed from the input data?
 * When the dataset was being cleaned, the following columns were removed:
   * EIN
   * Name
 * As these columns would not have any influence on the machine learning model, they were chosen to be removed. 

## Compiling, Training, and Evaluating the Model

* How many neurons, layers, and activation functions did you select for your neural network model, and why?
  * We utilized the following structure:
   * Insert picture here
  * Adding additional layers, neurons and a different activation feature were meant to hopefully optimize the target model.
* Were you able to achieve the target model performance?
  * Unfortunately not. 
* What steps did you take to try and increase model performance?
  * The following:
   * Attempted to remove variables from model (e.g., Special considerations)
   * Added neurons
   * Added hidden layers
   * Changed activation features
   * Increase number of epocs

# Summary

In summary, the original model reports an overall 73% accuracy rate and a .56 loss:

INSERT PICTURE

Overall, this model could stand to be improved and perhaps utilization of a K-Nearest Neighbor model may do the job. As we understand the target variable (e.g., Is successful) we do have an idea of what values we are looking for. 
