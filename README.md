# Uplift Modeling for Marketing Promotion Campaign Optimization
This repository houses the implementation and analysis of an uplift modeling approach aimed at optimizing marketing promotion campaigns. The project utilizes a dataset of 64,000 customer records, including historical promotion usage (Discount or Buy One Get One), extended offers, and conversion outcomes (purchase or not).

## 🚀 Problem Statement
The company had a dataset of 64,000 customers with brief information, such as historical promotion usage (Discount or Buy One Get One), offers that had been extended, and conversion results (purchase or not). The company wants to optimize Marketing Promotion Campaigns to target promotions at potential customers.

## 🎯 Objectives
The main objective of this project is to build an uplift model to predict the effectiveness of promotional strategies and optimize marketing campaigns to maximize conversions and reduce campaign costs.

## 📈 Develop Uplift Model
### Uplift Distribution
The Uplift Distribution shows the probability distribution of the individual treatment effect (ITE) predicted by the Uplift model. The ITE is the difference between the predicted outcome for an individual if they receive the treatment and the predicted outcome if they do not receive the treatment.
Based on the distributions of these two models, S-Learner and Uplift Tree, both show the majority of ITE is in the positive direction, indicating that the model predicts the treatment will tend to have a positive effect on individual outcomes.

## 📉 Model Evaluation
### Cumulative Gain Plot
The S-Learner Model achieves maximum effectiveness when targeted to approximately 15000 populations, while the Uplift Tree Model achieves maximum effectiveness when targeted to approximately 12000 populations.

### AUUC and Qini Score
#### AUUC Score:
- A higher AUUC Score value indicates a better ability of the model to distinguish between individuals who will benefit from the “offer” treatment and those who will not.
- In this case, Uplift Tree has a slightly higher AUUC Score (0.706158) than S-Learner (0.691273).
- The difference in AUUC Score between the two models is relatively small, but Uplift Tree performs slightly better.

#### Qini Score:
- Qini Score indicates the level of uncertainty in the model's predictions. A lower value indicates a lower level of uncertainty.
- In this case, Uplift Tree has a slightly lower Qini Score (0.258296) compared to S-Learner (0.29603).
- The difference in Qini Score between the two models is also relatively small, but Uplift Tree shows a slightly lower level of uncertainty.

Based on the evaluation results, Uplift Tree performs slightly better in terms of AUUC Score and Qini Score, but the difference is relatively small.

## 📜 Conclusion
This project focused on building an uplift model to optimize Marketing Promotion Campaigns. By analyzing the effectiveness of different models like S-Learner and Uplift Tree, we determined that Uplift Tree slightly outperforms in distinguishing treatment benefits and exhibits lower uncertainty. These insights will guide future marketing strategies to maximize conversions and minimize costs.
