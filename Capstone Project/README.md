# Travel Prediction Project

[Data source](https://www.kaggle.com/tejashvi14/travel-insurance-prediction-data)

## Introduction

A Tour & Travels company is an Indian company which is offering travel insurance packages to their customers. The new insurance package also includes covid coverage. The company wants to know which customers would be interested to buy it based on the existing historical dataset.
The insurance was offered to some of the customers in 2019 and the data has been extracted from the performance/sales of the package during that period. The data is provided for almost 2000 previous customers.

### Goals of this project

- Building a classification model that can predict if the customer will be interested to buy the travel insurance package.
- Build a demographic portrait of an average insurance buyer using Tableau.

### Research Questions

- To examine the travel insurance ratio in the data set.
- To examine the relationship between the family size, age, annual income and whether they buy the insurance.
- To examine how annual income correlate with experience in travel(flight frequency, travelling abroad) with regard to buying the insurance.
- To analyze if the presence of chronic diseases influence the desicion of buyng the insurance.

## Technologies

-  **Google sheets** for data cleaning. I used if statements to convert data into binary data type.
-  Data Exploration and Modeling was all done in **Python** using **the Jupyter Notebook**.
-  **Tableau** was used for a data visualisation.

## Important findings

![Travel insurance and all variables](Travel_insurance_variables.png)

At 25, there are more people buying the insurance. At 27-29, a lot more people opt not to take the coverage. It could be attributed to the expiry of the family insurance pack and since in India many people are starting families at this age they could choose not to buy an insurance.

![Age and annual income](Age_annual_income.png)

In every age group, customers with higher income are more likely to buy insurance and travel abroad.

![Age and family size](Age_family_size.png)

When customer's family size is from 5 to 9 members, there are more customers that prefer to buy an insurance.

### Demographic analysis in **Tableau**

![Dashboard](Dashboard.png)

### Modeling

-   My best performing model was a decision tree after hyperparameter tuning with an F1-Score of 81%. The model guessed 0("No insurance") correctly in 86% of all cases and guessed 1("Insurance") correctly in 70% of all cases. 
   
-   I performed cross-validation with the average result of 77% accuracy score to ensure that every observation from the original dataset has the chance of appearing in training and test set

-   I identified top 3 features by it's importance for prediction modeling.
   1) Annual income 
   2) Family members
   3) Age
    
## Recommendations  

-   Review this demographic analysis, since this data sample is limited. The customer's age is in the range of 25-35 years. 

-   Rise an awareness regarding risks associated with traveling and convince first-time flyers and travellers of the need of insurance. That might increase the sales of the new insurance package.

-   Create a more inclusive medical scope in the new insurance package to include more chronic diseases. The data shows a high count of customers with chronic diseases who have never bought a travel insurance.
