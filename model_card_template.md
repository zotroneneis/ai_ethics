# Model Card Template

## Introduction
This is a template for a model card. The original paper from which the contents were taken can be found [here](https://arxiv.org/abs/1810.03993). The goal of a model card is to document machine learning models in a standardized way. 

## Model Details
- Description of the model
- Person/Organization developing model
– Model date (when was the model deployed)
- Model version (which version and how is it different from previous ones)
– Model type (what type of model is it?)
- Input(s)
- Output(s)
– Training algorithm(s)
– Resources for more information (e.g. papers)
– Citation details
– License
– Where to send questions or comments about the model

## Intended Use
Why was the model developed? What should and should not it be used for?
– Primary intended uses
– Primary intended users
– Out-of-scope use cases (technology that the model might easily be confused with, or related contexts that users could try to apply the model to)

## Factors
Model performance across different factors. Example factors: demographic or phenotypic groups, environmental conditions, technical attributes.
– Relevant factors (What are foreseeable salient factors for which model performance may vary, and how were these determined?
– Evaluation factors (Which factors are being reported, and why were these chosen? If the relevant factors and evaluation factors are different, why?)

## Metrics
Metrics used to evaluate the performance of a model. Metrics should be chosen to reflect potential real-world impacts of the model.
– Model performance measures
– Decision thresholds (in case they were used)
– Approaches to uncertainty and variability

## Evaluation Data
Details on the dataset(s) used for the quantitative analyses in the card.
– Datasets
– Motivation (why were these datasets chosen?)
– Preprocessing

## Training Data
Details on the dataset(s) used for training. Detailed information about training data may not be possible to provide in practice.
– Datasets
– Motivation (why were these datasets chosen?)
– Preprocessing

## Quantitative Analyses
Quantitative analyses should be disaggregated, that is, broken down by the chosen factors. Quantitative analyses should provide the results of evaluating the model according to the chosen metrics, providing confidence interval values when possible.  

– Unitary results (How did the model perform with respect to each factor?)
– Intersectional results (How did the model perform with respect to the intersection of evaluated factors?)

## Ethical Considerations
Example topics:
- Data: Does the model use any sensitive data (e.g., protected classes)?
- Risks and harms: What risks may be present in model usage?

## Caveats and Recommendations
Additional concerns and thoughts not listed in the other sections.
