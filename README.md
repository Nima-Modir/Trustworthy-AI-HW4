# Security, Privacy, and Fairness in machine learning models

## Task 1: Security - Backdoor Attack and Model Cleansing
### Objective:
Detect and mitigate backdoor attacks in a neural network model trained on the MNIST dataset.
### Steps:
**Trigger Identification**: Use the Neural Cleanse method to identify the backdoor trigger by analyzing model behavior. The key assumption is that the model's weights are available, and clean data is accessible.

**Trigger Reconstruction**: Rebuild the trigger for each class label using optimization techniques. You will analyze and explain the terms involved in the objective function.

**Attack Label Identification**: Use the Median Absolute Deviation (MAD) method to identify the label under attack and explain the logic behind using this method.

**Model Cleansing**: Implement methods to cleanse the model from the backdoor attack, focusing on unlearning the backdoor while retaining model performance. Report accuracy and attack success rates for both the attacked and cleaned models.
## Task 2: Privacy - Differential Privacy Mechanisms
### Objective: 
Implement and analyze mechanisms that preserve differential privacy in responses to queries on income data.
### Steps:
**Laplace Mechanism**: Apply the Laplace mechanism to compute the amount of noise to add to income queries to preserve privacy (ε-differentially private).

**Noisy Query Responses**: Compute noisy responses for both average and total income based on the Laplace distribution. Report and compare results.

**Compositional Privacy Loss**: Adjust privacy budgets (ε1, ε2) to ensure the overall privacy loss stays below a certain threshold when multiple queries are applied.

**Counting Queries**: Implement and analyze Laplace noise for counting queries in a dataset and calculate the probability of noisy responses exceeding a threshold.
## Task 3: Fairness - Building Fair Machine Learning Models
### Objective: 
Create a fair machine learning model to predict employee income while addressing gender bias.
### Steps:
**Dataset Loading and Evaluation**: Load the provided dataset and evaluate a classifier that predicts whether an employee earns more than 50K based on features such as gender. Use metrics like Disparate Impact and Zemel Fairness to assess fairness.

**Baseline Model**: Split the dataset into training and testing sets, train a model, and evaluate its fairness for different gender groups.

**Fair Model Training**: Implement a method to mitigate bias by modifying the dataset and retrain the model. Analyze the fairness of the retrained model.

**Comparison**: Compare the results of the baseline and fair models in terms of accuracy and fairness. Suggest another approach to improve fairness and provide a detailed explanation of its effectiveness.
