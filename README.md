# Churn-Logistic-Regression-
* Created a logistic regression model calculating the liklihood a customer will switch providers in the next month 
* The model had a accuracy value of 78%
* Using the analysis, developed a course of action to retaining customers 

## Code and Resources Used 
* **RStudio**
* **Packages:** dbplyr, tidyverse, readxl, ggplot2, gridExtra, caret, e1071
* **Data:** Data was given from WGU for an assignment 

### Data Preparation 
* Because the dataset was quite large initially, I created a reduced dataset containing only a unique identifier, the response variable, and predictor variables. 
* Made the variables a foctor, so when building the model, the function will recognize the variable as a binary and not a char 

#### EDA
* Ran summary statistics
* Created univariate and bivariate plots 

##### Logistical Model 
* Used glm() function to create logisica regression model 
* Iniitial model contained all variables I thought was related to the response variable "churn"
* A reduced model was then created with only statistically significant variables 
* A confusion matrix was then made to test the accuracy of the model 
* The reduced model had an accuracy value of 78% 

###### Recommendations 
With the model, the strategy the telecommunication should take is to prioritize the male techie demographic, sign customers to contracts, and push fiber optic services. The telecommunications company can filter which customers are likely to churn and send out discounts, promotional deals, and other ads to retain the customer. They can start by targeting customers that identify as male and techie because those groups have a higher chance to churn. In addition, the company will need to focus on customers that are up for contracts by reaching out to them by phone or email with a new offer. Furthermore, the chance of churn can be lowered at the start if sales agents in the company prioritize signing a new customer onto a long-term contract. The analysis shows that customer with fiber optics internet is more likely to stay with the company. Making this service more available to customers will both increase sales and the likelihood of retaining the customer. The company can develop different strategies and prioritize a selected customer group when using the logistic regression model. 
