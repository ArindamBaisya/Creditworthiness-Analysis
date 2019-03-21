# Random-Undersampling-Creditworthiness-Analysis

Modeling Creditworthiness of Customers via Rare Event Phenomenon modeling using Random Under Sampling techniques and calculation of "Loss Function" to minimize Dollar Loss for banks, simultanously ensuring fair credit evaluation for customers

Problem Statement:
Credit Evaluation is a problem which requires special techniques as it poses a number of unique challenges to the modeller and to the bank.

1. Law requires a bank to inform the customer the reason, if denied credit. This automatically limits the types of modelling techniques that can be deployed by the modeler. Specifically, "black-box" techniques like Neural Network should be avoided to ensure the required level of determinism and fairness.

2. Credit evaluation falls under the realm of "Rare Event Phenomenon". Vast majority of people who apply for credit will probably receive credit from a bank and only a small fraction will not. In such situations, a model tends to predict everything as "good credit", which results in "Low Error Rate" (since bad credit are a rare event.), but completely defeats the purpose of credit evaluation.

Solution:
We tackle this two-fold problem by:

1. Using Deterministic modeling techniques like Logistic Regression which meet the requirement of fairness
2. Devising a "Loss Function" which calculates the Dollar Value of Loss and uses this function as a benchmark for performance
3. Using Random Undersampling with 10 fold Cross Validation on the Loss function to optimize decision making
