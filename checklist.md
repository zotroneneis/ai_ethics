# Data Science Ethics Checklist

## A. Project planning
 - [ ] **A.1 System existence**: Have we discussed whether the system should exist in the first place?
 - [ ] **A.2 Tool choices**: Have we discussed whether AI/ML is the right tool for the job?
 - [ ] **A.3 Common goal**: Have we engaged with the developers, users, consumers, and other key stakeholders to ensure a common understanding of the goal of the system and related risks of using AI/ML to achieve this goal? Have we documented the goal?
 - [ ] **A.4 Input from other groups**: Have we asked for input from different groups? For example from members of the stakeholder groups, domain experts and team members?

## B. Data Collection
 - [ ] **B.1 Informed consent**: If there are human subjects, have they given informed consent, where subjects affirmatively opt-in and have a clear understanding of the data uses to which they consent?
 - [ ] **B.2 Collection bias**: Have we considered sources of bias that could be introduced during data collection and survey design and taken steps to mitigate those? Take a look at existing tools like [Fairlearn](https://fairlearn.org) and the [AI Fairness Toolkit](https://github.com/Trusted-AI/AIF360).
 - [ ] **B.3 Limit PII exposure**: Have we considered ways to minimize exposure of personally identifiable information (PII) for example through anonymization or not collecting information that isn't relevant for analysis?
 - [ ] **B.4 Downstream bias mitigation**: Have we considered ways to enable testing downstream results for biased outcomes (e.g., collecting data on protected group status like race or gender)?
 - [ ] **B.5 Target population**: Is our data representative for the target population?
 - [ ] **B.6 Dataset card**: Have we documented dataset characteristics and limitations in form of a [dataset card](dataset_card_template.md)?
 - [ ] **B.7 Legal requirements**: Have we considered legal oblications and policy considerations that apply to the data?

## C. Data Storage
 - [ ] **C.1 Data security**: Do we have a plan to protect and secure data (e.g., encryption at rest and in transit, access controls on internal users and third parties, access logs, and up-to-date software)?
 - [ ] **C.2 Right to be forgotten**: Do we have a mechanism through which an individual can request their personal information be removed?
 - [ ] **C.3 Data retention plan**: Is there a schedule or plan to delete the data after it is no longer needed?

## D. Analysis
 - [ ] **D.1 Missing perspectives**: Have we sought to address blindspots in the analysis through engagement with relevant stakeholders (e.g., checking assumptions and discussing implications with affected communities and subject matter experts)?
 - [ ] **D.2 Dataset bias**: Have we examined the data for possible sources of bias and taken steps to mitigate or address these biases (e.g., stereotype perpetuation, confirmation bias, imbalanced classes, or omitted confounding variables)?
 - [ ] **D.3 Honest representation**: Are our visualizations, summary statistics, and reports designed to honestly represent the underlying data?
 - [ ] **D.4 Privacy in analysis**: Have we ensured that data with PII are not used or displayed unless necessary for the analysis? Have we ensured that it is not possible to re-identify the underlying person by the data or information disclosed?
 - [ ] **D.5 Auditability**: Is the process of generating the analysis well documented and reproducible if we discover issues in the future?

## E. Modeling
 - [ ] **E.1 Proxy discrimination**: Have we ensured that the model does not rely on variables or proxies for variables that are unfairly discriminatory?
 - [ ] **E.2 Fairness across groups**: Have we tested model results for fairness with respect to different affected groups (e.g., tested for disparate error rates)? We should consider each group and combinations of groups separately (e.g. stakeholders, developers, race, gender, age)
 - [ ] **E.3 Metric selection**: Have we considered the effects of optimizing for our defined metrics and considered additional metrics?
 - [ ] **E.4 Explainability**: Can we explain in understandable terms a decision the model made in cases where a justification is needed?
 - [ ] **E.5 Bias in predictions**: Has the system been evaluated for potential biased outcomes? Take a look at existing tools like [Fairlearn](https://fairlearn.org) and the [AI Fairness Toolkit](https://github.com/Trusted-AI/AIF360).
 - [ ] **E.6 Communicate bias**: Have we communicated the shortcomings, limitations, and biases of the model to relevant stakeholders in ways that can be generally understood?
 - [ ] **E.7 Model card**: Have we documented system characteristics and limitations in form of a [model card](model_card_template.md)?
 - [ ] **E.8 Legal requirements**: Have we considered legal oblications and policy considerations that apply to the model?
 - [ ] **E.9 System security**: Was the system tested for potential security threats in any/all levels of its stack (e.g. software level, AI framework level, model level, etc.)?

## F. Deployment
 - [ ] **F.1 Monitoring and evaluation**: How are we planning to monitor the model and its impacts after it is deployed (e.g., performance monitoring, regular audit of sample predictions, human review of high-stakes decisions, reviewing downstream impacts of errors or low-confidence decisions, testing for concept drift)?
 - [ ] **F.2 Stakeholder feedback**: Do we have a system in place for monitoring stakeholder feedback? Have we identified who is responsible for this?
 - [ ] **F.3 Redress**: Have we discussed with our organization a plan for response if users are harmed by the results (e.g., how does the data science team evaluate these cases and update analysis and models to prevent future harm)?
 - [ ] **F.4 Roll back**: Is there a way to turn off or roll back the model in production if necessary?
 - [ ] **F.5 Unintended use**: Have we taken steps to identify and prevent unintended uses and abuse of the model and do we have a plan to monitor these once the model is deployed?
