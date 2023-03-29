# Neural_Network_Charity_Analysis

## Overview 
The project involves analyzing a dataset from Alphabet Soup, a philanthropic organization, to create a binary classifier that can predict whether applicants will be successful if funded by the organization. The dataset includes more than 34,000 organizations that have received funding from Alphabet Soup, and features such as EIN and NAME, APPLICATION_TYPE, AFFILIATION, CLASSIFICATION, USE_CASE, ORGANIZATION, STATUS, INCOME_AMT, SPECIAL_CONSIDERATIONS, ASK_AMT, and IS_SUCCESSFUL.
## Results: Using bulleted lists and images to support your answers, address the following questions.

### Data Preprocessing
- What variable(s) are considered the target(s) for your model?
  - The target variable for the model is the "Is-Successful" column, which indicates whether the funding was used effectively.
- What variable(s) are considered to be the features for your model?
  - The features used for the model are NAME, APPLICATION, TYPE, AFFILIATION, CLASSIFICATION, USE_CASE, ORGANIZATION, INCOME_AMT, SPECIAL_CONSIDERATIONS, STATUS, and ASK_AMT.
- What variable(s) are neither targets nor features, and should be removed from the input data?
  - EIN was removed from the input data because it could potentially confuse the model into giving it too much importance. SPECIAL_CONSIDERATIONS and STATUS were also considered for removal, as the former had low frequency and could not be quantified, and the latter had the same value for all rows.
### Compiling, Training, and Evaluating the Model
- How many neurons, layers, and activation functions did you select for your neural network model, and why?
  - The neural network model used had three hidden layers with multiple neurons, which increased accuracy above 75%. The activation functions used were 'relu' for the first layer, and 'sigmoid' for the second and third layers, with the output function also being 'sigmoid'.
- Were you able to achieve the target model performance?
  - The target model performance was achieved.
- What steps did you take to try and increase model performance?
  - To improve model performance, the NAME column was converted into data points, which had a significant impact. Additionally, a third layer was added and 'sigmoid' was used as the activation function for the second and third layers.
## Summary:
The  model achieved above 75% accuracy predicting funding effectiveness with preprocessing steps and adding a layer and "sigmoid" activation function. For alternative model that could work as well, a decision tree algorithm could be a simpler alternative that handles missing data and outliers, allowing feature selection for better insights.
