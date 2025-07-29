# Overall Survival Prediction for patients diagnosed with Myeloid Leukemia

## Repository Link

https://github.com/kaSae6/PredictLeukemiaSurvival

## Description


Project description: Survival Analysis

[The dataset](https://challengedata.ens.fr/challenges/162) was a challenge for the prediction of the Overall Survival of Cancer Patients with Acute Myeloid Leukemia. 
One of the main goals was to predict the overall survival of AML-patients with Methods of the field of Survival Analysis. 
The Survival analysis describes a time-to event regression problem which is different to a regular regression due to "censoring". The dataset was "right-censored", i.e., a data point is above a certain value but it is unknown by how much. This often occurs in the field of Life-Sciences and Medicine.

The provided dataset included information of a time variable and event-indicator for each patient, which means the survived time from receiving diagnosis until death, or the last time of a check-up appointment when alive.  This created the problem of different states (event: alive or dead), together with survival-time and other possible covariates as blood work data to create a prediction of survival. 

For the baseline models we have chosen linear regression and random forest methods, which, however, meant to only include patients with the event of "death" since linear regression can't handle censoring.
Further methods were chosen especially to to examine right-censored data, included non-parametric Kaplan-Meier Survival Probability, semi-parametric Cox Proportional Hazard,and Deep-Cox model.




### Task Type

Time-to-event regression

### Results Summary

- **Best Model:** Random Forest according to RMSE and MAE scores, Deep cox according to the C-Index
- **Evaluation Metric:** MAE, RMSE, C-Index
- **Result:** Deep Cox C-Index = 0.73

## Documentation

1. **[Literature Review](https://github.com/kaSae6/PredictLeukemiaSurvival/blob/main/0_LiteratureReview/README.md)**
2. **[Dataset Characteristics](https://github.com/kaSae6/PredictLeukemiaSurvival/blob/main/1_DatasetCharacteristics/exploratory_data_analysis.ipynb)**
3. **[Baseline Model](https://github.com/kaSae6/PredictLeukemiaSurvival/blob/main/2_BaselineModel/baseline_model.ipynb)**
4. **[Model Definition and Evaluation](https://github.com/kaSae6/PredictLeukemiaSurvival/blob/main/3_Model/model_definition_evaluation.ipynb)**
5. **[Presentation](https://github.com/kaSae6/PredictLeukemiaSurvival/blob/main/4_Presentation/Survival_Analysis_Saegner_Muszelewski​.pdf)**

## Cover Image

![Project Cover Image](https://github.com/kaSae6/PredictLeukemiaSurvival/blob/main/CoverImage/cover_image.png)
