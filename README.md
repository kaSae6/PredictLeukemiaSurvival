# Overall Survival Prediction for patients diagnosed with Myeloid Leukemia

## Repository Link

https://github.com/kaSae6/PredictLeukemiaSurvival

## Description

[Short project description here. Briefly summarize the problem you are trying to solve and the approach you're taking.]

Project description:Survival Analysis

The dataset from [https://challengedata.ens.fr/challenges/162]
 , was a Challenge for the prediction of the Overall Survival of Cancer Patientx with Acute Myeloid Leukemia. One of the main goals was to predict the overall survival of AML-patients with Methods of the field of Survival Analysis.
The Survival analysis describes a time-to event regression problem which is different to a regular regression due to "censoring", which means that the provided dataset included information about the survived time from diagnosis to death or the last time of a check-up appointment when alive. This creates the problem of different states ( Event: alive or dead), together with survival time and other possible covariates as blood work data to create a prediction of survival.
After thorough Analysis, wee approached this problem naively with a linear regression, which meant to only include patients with the event of "death" since linear regression can't handle censoring.



### Task Type

[Image Classification / Chatbot / Regression / Clustering / Other]

### Results Summary

- **Best Model:** [Name of the best-performing model]
- **Evaluation Metric:** [e.g., Accuracy, F1-Score, MSE]
- **Result:** [e.g., 95% accuracy, F1-score of 0.8]

## Documentation

1. **[Literature Review](0_LiteratureReview/README.md)**
2. **[Dataset Characteristics](1_DatasetCharacteristics/exploratory_data_analysis.ipynb)**
3. **[Baseline Model](2_BaselineModel/baseline_model.ipynb)**
4. **[Model Definition and Evaluation](3_Model/model_definition_evaluation)**
5. **[Presentation](4_Presentation/README.md)**

## Cover Image

![Project Cover Image](CoverImage/cover_image.png)
