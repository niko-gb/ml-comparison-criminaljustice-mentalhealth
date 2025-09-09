# Comparative Study of Machine Learning Methods: Predicting Criminal Justice Involvement and Mental Health Treatment Intensity

This machine learning study compares five algorithms to predict mental health treatment needs and criminal justice involvement using real-world patient data from New York State's Office of Mental Health.

## Project Overview
This project addresses two critical healthcare challenges:
- Treatment Intensity Prediction: Identifying patients who will require intensive mental health treatment (inpatient, residential, emergency) vs. non-intensive care
- Criminal Justice Risk Assessment: Predicting which mental health patients may have criminal justice involvement

## Methodology
- **Data**: 2019 Patient Characteristics Survey (PCS), 2022 Patient Characteristics Survey (PCS)
- **Tech**: Jupyter Notebook (pandas, scikit-learn, matplotlib)
- **Models**: Logistic Regression, Naive Bayes, Decision Tree, K-Nearest Neighbors (KNN), Random Forest
- **Evaluation Metrics**: Accuracy, Precision, Recall, F1-score, ROC-AUC, confusion matrices
- **Validation**: Cross-validation performed on KNN with hyperparameter tuning

## Key Findings

- **Tree-based models** (Decision Tree, Random Forest) consistently outperformed other algorithms
- **Naive Bayes** showed the highest recall, crucial for healthcare safety (minimizing missed cases)
- **Housing stability** emerged as the strongest predictor across both tasks
- **Substance use disorders** strongly correlated with both intensive treatment needs and criminal involvement

Treatment Intensity Prediction (2019 PCS Data)

- **Best Performers**: Decision Tree & Random Forest (70% accuracy, 0.76 ROC-AUC)
- **Highest Recall**: Naive Bayes (77% - best for patient safety)
- **Key Predictors**: Age group (40% importance), housing situation (25-30%)

Criminal Justice Involvement Prediction (2022 PCS Data)

- **Best Performers**: Decision Tree & Random Forest (73% accuracy, 0.80 ROC-AUC)
- **Highest Recall**: Naive Bayes (69% - best for risk identification)
- **Key Predictors**: Housing situation (32-44% importance), gender (21%), substance disorders (16-19%)

## Performance Summary
| Model          | Treatment Intensity         | Criminal Justice            |
|----------------|-----------------------------|-----------------------------|
| Accuracy Range | 64-70%                      | 71-73%                      |
| Best ROC-AUC   | 0.76                        | 0.80                        |
| Top Performer  | Decision Tree/Random Forest | Decision Tree/Random Forest |
| Best Recall    | Naive Bayes (77%)           | Naive Bayes (69%)           |

## Limitations & Considerations

- Binary Classification: May oversimplify complex treatment needs
- Sampling Bias: Aggressive filtering may have removed valuable minority cases
- Ethical Considerations: Risk of discrimination in criminal justice predictions

## Future Enhancements

- Advanced Algorithms: Gradient boosting, ensemble methods
- Feature Engineering: Include medication history, treatment duration
- Multi-class Classification: More granular treatment intensity levels
- Fairness Metrics: Bias detection and mitigation techniques

## Author

**Nikolaos Gkmpenompa**  
Higher Diploma in Science in Data Analytics  
National College of Ireland  
