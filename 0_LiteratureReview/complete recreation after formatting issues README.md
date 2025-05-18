# Literature Review

Approaches or solutions that have been tried before on similar projects.

**Summary of Each Work**:

- **Source 1**: [Application of machine learning in breast cancer survival prediction using a multimethod approach]

  - **[Link](https://www.nature.com/articles/s41598-024-81734-y!)**
  - **Objective**:To create a machine learning model aiding clinicians in breast cancer survival prediction, which can help optimise the medical decisions and improve disease prognosis.

  - **Methods**:**Deep Neural Network** and **11 conventional Machine Learning** methods. Feature selection: Initially, modeling was executed using all features, which were chosen based on a review of relevant articles. Subsequently, features were selected based on a two-tailed p-value criterion (< 0.05) using scikit-learn. Lastly, features were chosen through a questionnaire completed by five oncologists. A total of **34 features** were  selected. The data used for the models was collected from **2644 patients**. 80% of the data was used for training the models. For the DNN, The Neural Architecture Search method, a technique in deep learning for automatically exploring optimal neural network architectures, was applied. Hyperparameters were adjusted following this exploration. To determine the optimal architecture and set hyperparameters, the Autokeras library was utilized.

  - **Outcomes**: DNN had the highest accuracy of 85.56% (While the DNN model showed superior accuracy in external validation, it did not consistently achieve the highest performance across all evaluation metrics).
  - **Relation to the Project**: Uses patient data to predict cancer survival; uses multiple different feature selection methods, different and many different models.


- **Source 2**: [A novel perspective on survival prediction for AML patients: Integration of machine learning in SEER database applications]

  - **[Link](https://pmc.ncbi.nlm.nih.gov/articles/PMC11795080)**
  - **Objective**:To establish a model for prognosis- prediction of  acute myeloid leukemia (AML) patients while exploring the epidemiological characteristics based on the SEER database to obtain insights to clinical and demographic prognosis -influencing features.

  - **Methods**: The approach to integrate traditional survival analysis with machine learning  with large-scale clinical data of a total of 87,090 AML patients between 1975 and 2019 was conducted after statistical analysis of independent factors that influenced the overall survival. Then, 11 machine learning algorithms as well as five-fold cross-validation with 20 cycles of each model were used in order of prediction- accuracy improvement.
The machine learning models were trained with a  dataset of 60,963 and then validated and evaluated with a dataset of  26,127 patients for the prediction of survival status at 1, 2, and 3 years after AML diagnosis.
The covered 11 models were: XGBoost classifier, cross-validated glmnet classifier, K-Nearest Neighbor classifier, Linear Discriminant Analysis classifier, Logistic Regression classifier, Naive Bayes classifier, Neural Network classifier, Quadratic Discriminant Analysis classifier, Random Forest classifier, Decision Tree classifier and Support Vector Machine classifier. 

  - **Outcomes**: The Successful establishment of a prediction model for the assistance of clinicians in making individualized prognostic predictions after exploration and comparison of 11 machine learning models.
The random forest classifier algorithm showed the best performance for the prediction of survival of 1, 2 and 3 years on multiple evaluation metrics. Additionally, the used neural network classifier and the XGBoost classifier had shown high reliability as well as accuracy at each prediction stage respectively.


  - **Relation to the Project**: The process of the establishment of a machine learning model to predict the survival of AML patients might be beneficial to the Project, as the goal is the development of a neural network - model to predict the overall survival of a very similar, but smaller and more recent dataset of AML patients.


- **Source 3**: [dentification of relevant features using SEQENS to improve supervised machine learning models predicting AML treatment outcome]

  - **[Link](https://link.springer.com/article/10.1186/s12911-025-03001-y)**
  - **Objective**: The evaluation of the selection methodology based on SEQENS, an algorithm for the identification of relevant variables, beside the validation of machine learning models that predict the risk of complications and to develop an assistive tool for clinicians in therapeutic decision-making.
  - **Methods**: To evaluate machine learning models that predict the risk of complications in AML Patients after 90 days, 6 months and 1 year after diagnosis, the dataset of 568 patients was used. For each time point, an enhanced SEQENS feature selection version was applied. Afterwards, 4 classifiers, including the XGBoost, Multi-Layer Perceptron, Logistic Regression and Decision Tree were used to evaluate the impact of feature selection on model performance.
After training, the models were evaluated with an external dataset of 54 AML patients.

  - **Outcomes**: After the identification of different features with Age, TP53, − 7/7Q, and EZH2 that showed consistent relevance for each prediction horizon,the evaluation of the models showed a stable or improved performance after the appliance of the SEQENS feature selection.

  - **Relation to the Project**: The conducted methods, specifically the showed improvements of model -performance after the applied feature- selection algorithm highlights the importance of (medical-) field expertise as well as in-depth exploration of the (clinical-) parameters covered in the datasets as the application field of medical and life sciences affect an extremely vulnerable group. This hints to an thorough approacht to our dataset and the possibility to integrate similar algorithms.

