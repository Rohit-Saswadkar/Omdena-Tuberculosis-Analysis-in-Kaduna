# Omdena-Tuberculosis-Analysis-in-Kaduna

![Omdena](https://github.com/user-attachments/assets/0bec0fee-b39c-430e-8a05-1e729c5906fd)

## Data Transformation and Model Evaluation

### Data Transformation

The dataset underwent several transformations before model evaluation:

- **Square Root Transformation**: Applied square root transformation to numerical columns to mitigate skewness. 
  ```python
  for col in num_cols:
      df[col] = np.sqrt(df[col]) - 0.01
  ```
- **One-Hot Encoding**: Encoded the LGA (Local Government Area) feature to convert categorical data into numerical format.
- **Principal Component Analysis (PCA)**: Utilized PCA to reduce dimensionality and extract 30 best components.
  
### Model Evaluation

The performance of a Ridge Regression model was evaluated using the following key metrics:

- **Hyperparameter**: Ridge Regression with alpha = 0.1 was chosen.
  
#### RMSE (Root Mean Squared Error)
- **Training Set**: 1.45
- **Test Set**: 1.44

#### R-squared (R2) Score
- **Training Set**: 0.9447
- **Test Set**: 0.9408

### Interpretation

- The low RMSE values indicate a close alignment between the model's predictions and actual values for both training and test sets.
- High R-squared values suggest that a significant portion of the target variable's variance is captured by the model.

### Conclusion

The Ridge Regression model, with alpha = 10, demonstrates robust predictive performance on both training and test datasets. Its ability to generalize well is evident from the comparable performance on both sets, minimizing the risk of overfitting.

---


# Tuberculosis (TB) Analysis and Recommendations

## Overview

This section provides a comprehensive analysis of presumptive TB cases, diagnosed cases, HIV status, and healthcare worker involvement. Key observations and recommendations are outlined based on the analyzed data.

### Presumptive Cases and Examinations

- An upward trend in presumptive cases and examinations suggests increased vigilance or targeted testing initiatives.
- The surge in 2020 Q3 may be related to a specific public health campaign.

### Diagnosed Cases

- The rise in total diagnosed cases indicates potential improvements in diagnostic technologies or expanded testing infrastructure.
- Consistent growth might signify advancements in testing capabilities leading to more accurate diagnoses.

### HIV Positive Cases

- Fluctuations highlight potential disparities in education and limited public awareness.
- Persistent challenges in HIV education may contribute to higher HIV positive cases.

### Healthcare Workers (HCWs)

- The presence of HCWs among presumptives may reflect proactive health monitoring or targeted workplace testing.

### Geographic Observations

- Higher TB prevalence in specific LGAs (Kaduna North, Zaria, Kaduna South).
- Higher frequency of HIV-positive cases in Kaduna South, Kaduna North, and Chikun, suggesting integrated TB and HIV control strategies are needed.

### Rifampicin Resistance

- Present in Kaduna South, Zaria, and Kaduna North, indicating the emergence of drug-resistant TB.
- Urgent measures are needed to curb the spread of drug-resistant TB.

### Recommendations

1. Prioritize TB screening, diagnosis, and treatment programs in high-burden LGAs (Kaduna North, Zaria, Kaduna South).
2. Implement interventions to reduce drug-resistant TB, focusing on areas with identified Rifampicin resistance cases.
3. Integrate TB control with HIV testing and treatment services, particularly in LGAs with high HIV prevalence.
4. Strengthen public health education campaigns to raise awareness about TB symptoms and encourage early testing.

### Data Considerations

- This analysis is based on potentially limited data.
- Access to more comprehensive data, including specific timeframes and missing details on other LGAs, could provide a more complete picture.

### Further Analysis

1. Obtain data covering a specific timeframe to analyze trends in TB cases, diagnosis rates, and drug resistance.
2. Explore potential risk factors associated with TB in different LGAs (e.g., socioeconomic factors, access to healthcare).

### Additional Notes

- The conclusion acknowledges the limitations of the data and emphasizes the need for more comprehensive information.
- It suggests further analysis to explore potential risk factors and trends.
- The recommendations prioritize public health interventions targeting high-burden areas and address the need for integrated TB and HIV control strategies.

---

# Appreciation

I am thrilled to contribute to this project, and I believe that our collective efforts will significantly impact public health in the community. Thank you for the opportunity, and I look forward to further collaboration.

Best regards,
Rohit R Saswadkar
