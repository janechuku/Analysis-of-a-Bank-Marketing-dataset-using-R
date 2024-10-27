# Analysis-of-a-Bank-Marketing-dataset-using-R-Studio
This entire analysis was done on R-Studio. It was an analysis of a dataset of a Portugese bank's marketing strategy to get customers to subscribe to their term deposit

![image](https://github.com/user-attachments/assets/34db5342-035c-4456-8db3-7d87db2791be)


## Introduction
The bank marketing dataset contained information from a Portuguese banking institution, primarily focused on a marketing campaign to promote term deposits.
The dataset includes demographic and financial details about the bank’s customers and attributes related to their interactions with its campaigns.
It is structured with multiple features that help to identify patterns that influence whether or not a customer subscribes to a term deposit (the target variable "y").

![image](https://github.com/user-attachments/assets/5cb12cd8-6a69-4d5d-a576-7d7b0fdc9f21)
![image](https://github.com/user-attachments/assets/5242e9af-4f7b-4890-9b2c-82e1ba06a717)

### Analysis of the Demographic Distribution
From the demographic distribution of the data, below is a summary of the findings:

**Marital Status:** Married individuals lead in term deposit subscriptions (66.7%), likely due to greater financial stability than single or divorced clients.

**Education:** Most subscribers have secondary education, while those with tertiary or primary education show lower subscription rates, potentially reflecting varying financial priorities or constraints.

**Age:** Middle-aged individuals, predominantly in their 30s and 40s, form the bulk of subscribers, indicating higher interest from those in prime working years.

**Job Distribution:** Key job groups include blue-collar, management, and technicians, revealing diverse income levels. This data helps tailor targeted marketing toward specific job sectors.

![image](https://github.com/user-attachments/assets/70263ead-ec56-4072-867e-5ee1e17e65f3)

![image](https://github.com/user-attachments/assets/6a0be5bf-6512-46a8-a180-49ccaa0bb3f0)

![image](https://github.com/user-attachments/assets/c5073c45-3e9a-4623-b92c-cf1b077d011d)

### Correlation analysis

Using the corr function on R, below is a summary of the findings from the correlation analysis:

**Age & Balance:** Older customers generally have higher balances, suggesting opportunities for retirement-focused financial products.

**Default & Balance:** Customers with higher balances show lower default risks, allowing them to subscribe to the term deposit.

**Loans & Default Risk:** Existing loan holders have a slightly higher risk of default, indicating a need for debt management support, rather than the subscription.

**Loans & Balance:** Those with loans tend to have lower balances, emphasizing the importance of cross-sell opportunities like savings or budgeting products.

**Call Duration:** Longer call durations slightly reduce term deposit subscription rates, pointing to a focus on concise, quality conversations.

**Campaign History:** Customers with previous campaign contact and high balances could be valuable targets for high-value promotions.

**Housing Loans & Deposits:** Customers with housing loans are less likely to subscribe to term deposits, highlighting a focus on debt-related products.

![image](https://github.com/user-attachments/assets/f4eea006-491b-4530-a451-ae8b847fc507)


![image](https://github.com/user-attachments/assets/f4dc7de1-18b2-47a8-9374-e562fc9e3713)

### Campaign Strategy Analysis

It was important to assess the success of the campaign strategy to serve as a learning point for future campaigns. See the findings below:

**Call Duration:** Successful term deposit subscriptions have longer call durations.
Action: Train agents to focus on quality engagement without excessively long calls.

**Contact Type:** Cellular contacts yield higher success rates than telephones.
Action: Prioritize mobile outreach for better engagement.

**Number of Contacts:** Success plateaus after an optimal contact frequency.
Action: Limit contacts to an optimal range to maximize efficiency and impact.

![image](https://github.com/user-attachments/assets/4d3dc8d5-84c5-4d34-b5d0-acb9ccf7e5f7)

![image](https://github.com/user-attachments/assets/8d6d6f31-7d86-4ca9-8593-9332d4f71fd3)

![image](https://github.com/user-attachments/assets/6e1ceab2-2a4d-4dab-8b27-61575af61f08)


### Financial Analysis
The financial analysis was to give an insight into the financial stability of the target population. See the below findings:

**Housing Vs Subscription:** Homeowners are less likely to subscribe, likely due to financial stability and other priorities.
Implication: Adjust marketing to address homeowners’ unique needs and priorities.

**Loan Vs Subscription:** Individuals with loans show a slight decrease in subscription response.
Implication: Target customers with manageable debt or offer products that align with financial obligations.

**Default Vs Subscription:** Minimal negative impact of default history on subscription likelihood.
Implication: Consider other factors alongside default for effective targeting in campaigns.

![image](https://github.com/user-attachments/assets/594aa844-cf5a-4476-ae61-16a8603195ab)

![image](https://github.com/user-attachments/assets/53e9ff43-2259-4a9d-b178-14b8de9ce6db)


### Regression Analysis & Modeling
We then did a little bit of machine learning
The logistic regression model identified the key variables in the bank dataset that significantly affect the outcome variable 'y', enabling us to understand the most important factors driving the prediction.

**Age's Impact on Predictions:** We found that age is a significant factor in predicting the outcome 'y', with the predicted probabilities plotted against age revealing the impact of age on the prediction.

**Good Model Accuracy:** The ROC curve analysis demonstrated that the model can effectively distinguish between the two classes, indicating good accuracy in predicting the outcome 'y' based on the given data.

![image](https://github.com/user-attachments/assets/9314da44-89d2-4807-a1af-37b017056918)

![image](https://github.com/user-attachments/assets/b2172613-695a-42b5-9e23-35548658ddbe)


## Conclusion

This analysis is useful for:
1. targeted marketing via demographic insights which enables the bank to tailor campaigns to the most responsive customer segments, boosting conversion rates.
2. campaign optimization, with the analysis of contact methods like mobile calls and call duration for more engaging and successful customer interactions.
3. risk management and product development, by understanding the impact of loans on term deposit subscriptions which helps the bank develop supportive financial products.
4. strategic decision-making via data-driven insights that aid in resource allocation, focusing on high-potential segments and managing lower-likelihood customer risks.

### Source of Data:
https://archive.ics.uci.edu/dataset/222/bank+marketing
