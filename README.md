# ARI5102: Data Analysis Techniques
Project created in fulfilment of the UoM Masters in AI study unit 'ARI5102 - Data Analysis Techniques'.

## Dataset

The dataset `dataset.csv` includes responses from individuals who participated in a survey and responded to various questions. Each question offers one or more selectable options for the respondents. 

Some notes regarding the dataset structure are the following: 
1. Each row in the dataset corresponds to a respondent. 
2. Options that belong to the same question share the same prefix, e.g., q3\_1 and q3\_3 correspond to answer options 1 and 3 for question q3, while q1_1 represents the first 
option for question q1. 
3. A respondent selects an option if its value in the corresponding column is set to 1.0. 
4. Some questions are single-selection, i.e. their options are mutually exclusive, and thus, a respondent may select exactly one option, while others are multiple-selection questions. 
5. There are questions not answered by all respondents, and thus, NaN values appear in the respective columns. 

## Deliverables

The responses can be found in `nathan_portelli.ipynb`. A presentation with the summarised results could be found in `ARI5102 Presentation.pdf`.

### Task 1
1. How many questions exist in the survey?
2. How many respondents are in the survey?
3. What are the different question types based on their selection options?

### Task 2
If you were asked to build a model for a question in the dataset, using the rest of the questions explanatory variables:  
1. Which performance measures would you use?
2. Does the selection of the performance metric depend on the type of question?

### Task 3

Consider the fifth question (q5) as a response variable and build a predictive model using some all other questions as explanatory variables. 
1. Implement a suitable algorithm for this task.
2. Evaluate the implemented model using the metrics you proposed in Task 2.
3. Interpret the trained model (if possible) and the obtained results.

Let’s assume that the options of the fifth question (q5) are semantically ordered, e.g. q5 corresponds to the question “How much do you like this photograph from 1-10?” with options q5_1=1, q5_2=2 and so on.  
1. Implement a predictive model incorporating this new piece of information.
2. Select appropriate metrics to evaluate the performance of the model in this scenario.

### Task 4

In this task, you should identify similar respondents. Specifically, you should do the following: 
1. Create groups of “like-minded”/similar respondents by proposing and implementing one or more suitable algorithms.
2. Evaluate whether the clusters you created are good enough.
3. Compare different algorithms against each other to select one of them.
4. Describe the groups you identified.
5. Create visualisations for the clustering results.
6. How would you assign a new respondent to an existing group?

### Task 5

Based on the results obtained from Task 4: 
1. Explain whether the clustering information could be used to build more accurate models for Task 3, and describe what you would do to build such models.
