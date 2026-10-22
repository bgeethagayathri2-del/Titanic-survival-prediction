# Titanic Survival Prediction

Predicts whether a passenger survived the Titanic using passenger details such as sex, class, age and fare.

- **Dataset:** Titanic (891 passengers, from seaborn)
- **Steps:** exploration, cleaning missing values, encoding text columns, training two models
- **Data cleaning:** 177 missing ages were filled with the median age, and 2 missing embarkation ports were filled with the most common port.
- **Results:**

| Model | Accuracy |
|---|---|
| Logistic Regression | 0.810 |
| Random Forest | 0.799 |

- **Random Forest detail:** precision 0.82 and recall 0.84 for passengers who died, precision 0.76 and recall 0.74 for passengers who survived.
- **Conclusion:** Both models performed about the same (around 80%). Logistic Regression was slightly ahead, but the gap is only about 2 passengers out of 179 in the test set, so neither is clearly better. The models predict deaths a little better than survivals.

## Key Finding
The most important features were fare (27.4%), sex (26.8%) and age (25.3%). The bar charts also showed
