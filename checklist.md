# Data Science Ethics Checklist

## A. Data Collection
 - [ ] **A.1 Informed consent**: If there are human subjects, have they given informed consent, where subjects affirmatively opt-in and have a clear understanding of the data uses to which they consent?
 - [ ] **A.2 Collection bias**: Have we considered sources of bias that could be introduced during data collection and survey design and taken steps to mitigate those?
 - [ ] **A.3 Limit PII exposure**: Have we considered ways to minimize exposure of personally identifiable information (PII) for example through anonymization or not collecting information that isn't relevant for analysis?
 - [ ] **A.4 Downstream bias mitigation**: Have we considered ways to enable testing downstream results for biased outcomes (e.g., collecting data on protected group status like race or gender)?

## B. Data Storage
 - [ ] **B.1 Data security**: Do we have a plan to protect and secure data (e.g., encryption at rest and in transit, access controls on internal users and third parties, access logs, and up-to-date software)?
 - [ ] **B.2 Right to be forgotten**: Do we have a mechanism through which an individual can request their personal information be removed?
 - [ ] **B.3 Data retention plan**: Is there a schedule or plan to delete the data after it is no longer needed?

## C. Analysis
 - [ ] **C.1 Missing perspectives**: Have we sought to address blindspots in the analysis through engagement with relevant stakeholders (e.g., checking assumptions and discussing implications with affected communities and subject matter experts)?
 - [ ] **C.2 Dataset bias**: Have we examined the data for possible sources of bias and taken steps to mitigate or address these biases (e.g., stereotype perpetuation, confirmation bias, imbalanced classes, or omitted confounding variables)?
 - [ ] **C.3 Honest representation**: Are our visualizations, summary statistics, and reports designed to honestly represent the underlying data?
 - [ ] **C.4 Privacy in analysis**: Have we ensured that data with PII are not used or displayed unless necessary for the analysis?
 - [ ] **C.5 Auditability**: Is the process of generating the analysis well documented and reproducible if we discover issues in the future?
 

## D. Modeling
 - [ ] **D.1 Proxy discrimination**: Have we ensured that the model does not rely on variables or proxies for variables that are unfairly discriminatory?
 - [ ] **D.2 Fairness across groups**: Have we tested model results for fairness with respect to different affected groups (e.g., tested for disparate error rates)?
 - [ ] **D.3 Metric selection**: Have we considered the effects of optimizing for our defined metrics and considered additional metrics?
 - [ ] **D.4 Explainability**: Can we explain in understandable terms a decision the model made in cases where a justification is needed?
 - [ ] **D.5 Communicate bias**: Have we communicated the shortcomings, limitations, and biases of the model to relevant stakeholders in ways that can be generally understood?

## E. Deployment
 - [ ] **E.1 Redress**: Have we discussed with our organization a plan for response if users are harmed by the results (e.g., how does the data science team evaluate these cases and update analysis and models to prevent future harm)?
 - [ ] **E.2 Roll back**: Is there a way to turn off or roll back the model in production if necessary?
 - [ ] **E.3 Concept drift**: Do we test and monitor for concept drift to ensure the model remains fair over time?
 - [ ] **E.4 Unintended use**: Have we taken steps to identify and prevent unintended uses and abuse of the model and do we have a plan to monitor these once the model is deployed?

## G. Other
 - [ ] **G.1 Representation**: Is our data representative for the target population?
 - [ ] **G.2 Re-Identification**: Is it possible to re-identify the underlying person by the data or information disclosed? (Anonymous/ masked data)
 - [ ] **G.3 System existence**: Have we discussed whether the system should exist in the first place?
 - [ ] **G.4 Tool**: Have we discussed whether AI/ML is the right tool for the job?
 - [ ] **G.5 Fairness-related harm**: When analyzing the results consider each groupt and combinations of groups separately (e.g. stakeholders, developers, race, gender, age)
 - [ ] **G.6 Input from other groups**: Have we asked for input from different groups? For example from members of the stakeholder groups, domain experts and team members?
 - [ ] **G.7 Model card**: Have we documented system characteristics and limitations in form of a model card?
 - [ ] **G.8 Dataset card**: Have we documented dataset characteristics and limitations in form of a dataset card?
 - [ ] **G.9 Stakeholder feedback**: Do we have a system in place for monitoring stakeholder feedback? Have we identified who is responsible for this?
 - [ ] **G.10 Common goal**: Have we engaged with the developers, users, consumers, and other key stakeholders to ensure a common understanding of the goal of the system and related risks of using AI/ML to achieve this goal?
 - [ ] **G.11 Document goal**: Have we documented the goals and risks?
 - [ ] **G.12 Legal requirements**: Have we considered legal oblications and policy considerations that apply to the model and data?
 - [ ] **G.13 Bias in training data**: Did we try to learn what types of bias exist in the training data (statistical, contextual, historical, or other) and how they can be mitigated?
 - [ ] **G.14 Bias in predictions**: Has the system been evaluated for potential biased outcomes?
 - [ ] **G.15 System security**: Was the system tested for potential security threats in any/all levels of its stack (e.g. software level, AI framework level, model level, etc.)?
 - [ ] **G.16 Periodic review**: Do we have a system in place for periodic reviews of the system to determine whether it still meets its purpose?
