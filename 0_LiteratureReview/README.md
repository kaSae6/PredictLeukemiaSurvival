# Literature Review

Approaches or solutions that have been tried before on similar projects.

**Summary of Each Work**:

- **Source 1**: Application of machine learning in breast cancer survival prediction using a multimethod approach

  - **[Link](https://www.nature.com/articles/s41598-024-81734-y)**
  - **Objective**: To create a machine learning model aiding clinicians in breast cancer survival prediction, which can help optimise the medical decisions and improve disease prognosis.
  - **Methods**: **Deep Neural Network** and **11 conventional Machine Learning** methods. Feature selection: Initially, modeling was executed using all features, which were chosen based on a review of relevant articles. Subsequently, features were selected based on a two-tailed p value criterion (< 0.05) using scikit-learn. Lastly, features were chosen through a questionnaire completed by five oncologists. A total of **34 features** were selected. The data used for the models was collected from **2644 patients**. 80% of the data was used for training the models. For the DNN, The Neural Architecture Search method, a technique in deep learning for automatically exploring optimal neural network architectures, was applied. Hyperparameters were adjusted following this exploration. To determine the optimal architecture and set hyperparameters, the Autokeras library was utilized.
  - **Outcomes**: DNN had the highest accuracy of 85.56% (While the DNN model showed superior accuracy in external validation, it did not consistently achieve the highest performance across all evaluation metrics).
  - **Relation to the Project**: Uses patient data to predict cancer survival; uses multiple different feature selection methods, different and many different models.

- **Source 2**: A novel perspective on survival prediction for AML patients: Integration of machine learning in SEER database applications!

  - **[Link]()** https://pmc.ncbi.nlm.nih.gov/articles/PMC11795080/

  - **Objective**: To establish a model for prognosis- prediction of  acute myeloid leukemia (AML) patients while exploring the epidemiological characteristics based on the SEER database to obtain insights to clinical and demographic prognosis -influencing features.

  - **Methods**: The approach to integrate traditional survival analysis with machine learning with large-scale clinical data of a total of 87,090 AML patients between 1975 and 2019 was conducted after statistical analysis of independent factors that influenced the overall survival. 

  - **Outcomes**: Successful establishment of a prediction model for assistance of clinicians in making individualized prognostic predictions.

  - **Relation to the Project**: The process of the establishment of a machine learning model to predict overall survival might be beneficial to the Project, as the goal is the development of a neural network - model to predict the overall survival of a very similar, but smaller and more recent dataset of AML patients.


- **Source 3**: [Title of Source 3]

  - **[Link]()**
  - **Objective**:
  - **Methods**:
  - **Outcomes**:
  - **Relation to the Project**:
