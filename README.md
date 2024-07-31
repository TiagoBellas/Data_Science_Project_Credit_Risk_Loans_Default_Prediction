# Data_Science_Project_Credit_Risk_Loans_Default_Prediction

This is an Academic project Postgraduate in Data Science made in collaboration with my colleagues below:

- https://github.com/Przon | [Fernando Reis]
- https://github.com/lfbr0 | [Luis Ribeiro]
- https://github.com/renato747 | [Renato Morais]

**Loans data**

train_validation_kaggle = pd.read_csv('train_validation_kaggle.csv', encoding='ISO-8859-1')

unseen_kaggle = pd.read_csv('unseen_kaggle.csv', encoding='ISO-8859-1')

**1. Introduction**

In this group project, our primary goal was to design and implement a predictive model capable of accurately assessing credit risk and forecasting loan defaults. We utilized advanced machine learning techniques to analyze a rich  financial dataset that captured detailed borrower information, including loan amounts, loan terms, and employment titles among other things. This dataset required meticulous preprocessing to prepare for model training, involving comprehensive data cleaning, normalization, and exploratory data analysis. Such steps were crucial to ensure the integrity and accuracy of our predictive models. One of the significant challenges in credit risk modeling is addressing the imbalance typically present in datasets where defaults are much less common than non-defaults. To overcome this, we employed the Synthetic Minority Over-sampling Technique (SMOTE), a method proven to improve model outcomes by balancing class distribution, which in turn enhanced the predictive performance of our models. Our methodological framework was systematic and robust, starting with a basic logistic regression model and progressively incorporating more sophisticated algorithms such as Random Forest and XGBoost and ending up with a deep learning model. This approach allowed us to evaluate and compare the effectiveness of various models in a controlled manner, ensuring that we selected the most suitable model based on performance metrics tailored to credit risk assessment. Through this project, we aimed to contribute valuable insights and tools to the field of financial risk management, supporting better decision-making processes in loan approvals and risk mitigation.

**2. Exploratory data analysis**

This exploratory data analysis data reveals interesting patterns that can provide insights for financial institutions, investors, companies, and policymakers. Loan Distribution In terms of loans, the majority are concentrated between $10,000 and $20,000, a range that suggests the customers are seeking moderate sums. Investors tend to finance in this bracket, which could be considered an ideal point of accessibility and appeal. The tenure of financial products is short, implying a demand for quicker settlements. Interest rates, often situated between 10% and 15%, indicate a sought-after balance between risk and return, while higher rates point to products intended for clients with higher risk or less favorable credit.

**_Payment Regularity_**

Regarding payments, monthly installments tend to vary from $300 to $400, although larger loans, less frequent, are also present. This could signal an opportunity for institutions to adjust their products to different installment sizes. The distribution of credit categories falls in a middle zone, indicating a medium risk profile in the loan portfolio. Stability in the Job Market and Economic Implications Analyzing the job market, a great diversity of positions and levels of specialization is observed. There is a predominance of individuals who remain in their jobs for extended periods, primarily in highly 5 qualified professions, suggesting employment stability. Interestingly, no seasonal pattern in the job market is observed, and most loans tend to be paid on time, with clear distinctions between nonperforming and delayed loans, which could reflect efficient collections management or a tendency of borrowers to avoid default.
The correlations between the data suggest that specialized professions are associated with greater employment stability, while less specialized roles may have higher turnover. Finally, borrowers' ability to pay loans may be linked to overall economic health, suggesting a resilient job market.
We observe a decrease in the frequency of job titles as we move from left to right of the graph, suggesting that subsequent positions are progressively less common. The diversity of professions, which includes managers, drivers, nurses, and accountants, reflects a wide range of work fields and the distribution of job types within the studied population. This indicates a variety of available employment opportunities but may also signal fierce competition in certain areas.

**_Payment Regularity and Economic Health_**

The analysis of loan status indicates that the majority are paid punctually, with a clear distinction between those who are up-to-date and those with delays. This may be reflective of proactive debt collection management and borrowers motivated to preserve a healthy credit reputation. Additional insights with Exploratory Data Analysis The combination of a stable economy, efficient loan management, and a diversified job market suggests a virtuous cycle. Highly qualified professionals tend to enjoy greater job security, contributing to higher repayment rates. The absence of seasonal variation in both employment and loan repayments reinforces an overall stability that benefits both financial institutions and workers. These indicators are essential for the development of effective economic and social policies, ensuring the continuity of economic health.

Finally, the analysis of loan status shows that most loans tend to be fully paid. However, there is a clear distinction between non-performing loans and those that are overdue. This may reflect efficiency in debt management, with borrowers willing to regularize debts before entering complete default, which could be motivated by effective collection policies or the borrowers' desire to maintain a good credit reputation.

Through this exploratory analysis, we can infer that a combination of a stable economy with effective loan management and a diversified job market creates a positive cycle. Highly qualified professionals are more likely to maintain employment stability, which could contribute to a higher loan repayment rate. In contrast, the absence of a seasonal pattern in both jobs and loan repayments suggests a stability that benefits both financial institutions and workers. The ability to pay loans and employment stability can be seen as indicators of economic health and are crucial for planning effective economic and social development policies.
