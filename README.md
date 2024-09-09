# Customer-Churn-Prediction-Analysis
This project focuses on predicting customer churn using the Telco Customer Churn dataset. The objective is to analyze key factors influencing customer churn and build a predictive model to classify whether customers are likely to churn or not.
# Creating a markdown file summarizing the findings for display on GitHub
markdown_content = """
# Customer Churn Prediction Analysis

### Dataset
- The dataset includes customer information such as tenure, contract type, monthly charges, and other factors.
- The target variable is `Churn`, indicating whether the customer has churned (Yes) or not (No).

## Key Findings

### 1. Tenure and Churn
Customers with shorter tenure are more likely to churn. This suggests that new customers, or those who have been with the service for a shorter period, may not be satisfied, possibly due to unmet expectations or onboarding challenges.

### 2. Monthly Charges and Churn
Customers with higher monthly charges are more likely to churn. High costs might lead to dissatisfaction, prompting customers to leave.

### 3. Contract Type and Churn
Customers on month-to-month contracts are significantly more likely to churn than those on one- or two-year contracts. Longer contracts seem to provide stability and reduce churn risk.

## Model Performance

- **Model Used**: Logistic Regression
- **Accuracy**: 81.8%
- **Precision**: 
  - Class 0 (non-churn): 86%
  - Class 1 (churn): 68%
- **Recall**: 
  - Class 0 (non-churn): 90%
  - Class 1 (churn): 58%
- **F1-Score**: 
  - Class 0 (non-churn): 88%
  - Class 1 (churn): 63%

While the model performs well overall, predicting churn (class 1) is more challenging than predicting non-churn (class 0).

## Recommendations

1. **Focus on New Customers**:
   - Since customers with shorter tenures are more likely to churn, prioritize customer engagement and satisfaction in the early months of service.
   
2. **Review Pricing Strategy**:
   - Consider optimizing the pricing structure, especially for customers with higher monthly charges. Offering discounts or additional benefits could reduce churn.
   
3. **Promote Long-Term Contracts**:
   - Encourage customers on month-to-month contracts to switch to longer-term contracts by offering incentives such as discounts, loyalty rewards, or free upgrades.

## Next Steps

- Explore more advanced machine learning models such as Random Forest or Gradient Boosting to improve churn prediction.
- Perform hyperparameter tuning to optimize model performance.
- Investigate further factors that might influence churn, such as customer service interactions or geographic location.

### Conclusion

The analysis provides valuable insights into customer churn at a telecom company. By focusing on tenure, monthly charges, and contract types, businesses can take proactive steps to reduce churn and improve customer retention.

---

**Project by:** Aya El-Dassouki


# Write the markdown content to a file
markdown_file_path = "/mnt/data/Customer_Churn_Analysis.md"
with open(markdown_file_path, "w") as file:
    file.write(markdown_content)

# Return the file path for download
markdown_file_path
