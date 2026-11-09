# DataVerse Challenge: Jumia Jitters

## Executive Summary
This report documents the analysis, modeling, and business recommendations for the Jumia Jitters dataset, focusing on seller risk profiling, review fraud detection, and logistics optimization. All findings are based on the accompanying notebook, which details the code, analytics, and visualizations for each task.

---

## Task 1: Data Cleaning & Feature Engineering
- **Actions:**
    - Cleaned inconsistent entries in Seller ID, Product Category, and Warehouse Zone.
    - Converted date columns and calculated delivery delays.
    - Engineered features: Return Rate, Average Rating, Complaint Rate, Seller Risk Score, Delivery Efficiency, Total Price.
    - Addressed missing values using forward fill, mean imputation, and category-based strategies.
    - Documented all cleaning steps in the notebook for reproducibility.

- **Key Insights:**
    - Data quality is critical for reliable analytics. All missing and inconsistent values were handled before analysis.
    - Seller Risk Score was calculated using a weighted formula combining delivery delay, return rate, and complaint rate.

---

## Task 2: Analytics & Visualization
- **Actions:**
    - Identified top and bottom sellers by fulfillment reliability.
    - Analyzed product categories with the highest complaint counts.
    - Mapped regions with the longest average delivery delays.
    - Detected repetitive review texts to flag potential review fraud.
    - Created complaint heatmaps and visual summaries.

- **Key Insights:**
    - Certain sellers and product categories are consistently associated with high complaints and delays.
    - Repetitive review texts are a strong signal of review manipulation.
    - Lagos warehouse delay data was excluded from analytics due to overcapacity and unreliability, with all affected metrics recalculated and flagged.

---

## Task 3: Prediction & Risk Modeling
- **Actions:**
    - Addressed class imbalance using SMOTE for return prediction modeling.
    - Built RandomForest classification models with and without NLP features (TF-IDF on review text).
    - Evaluated model performance using accuracy, confusion matrix, and classification report.
    - Identified sellers likely to trigger high returns using recent trends and model predictions.
    - Created a Seller Risk Framework radar chart for board presentation.

- **Key Insights:**
    - The test set remains highly imbalanced, limiting recall for return prediction.
    - Feature engineering and NLP can improve model sensitivity, but further work is needed for minority class detection.
    - Sellers with only 5-star ratings and high return/complaint rates are flagged as suspicious.

---

## Task 4: Strategy & Resolution
- **Actions:**
    - Recommended actionable strategies to reduce delivery delays, including prioritizing high-delay regions, optimizing seller dispatch, and improving logistics partnerships.
    - Provided a Customer Trust Policy to guide transparent communication and fair resolution.
    - Recommended top sellers to suspend and product categories to regulate based on complaint and return metrics.
    - Documented all business curveballs and adjustments (e.g., exclusion of Lagos data).

- **Key Insights:**
    - Excluding unreliable data (Lagos zone) is essential for accurate insights.
    - Early warning signals for review fraud include mismatches between high ratings and negative outcomes, repetitive review texts, and abrupt changes in review volume.
    - Automated detection logic is recommended for ongoing monitoring.

---

## Answers to Key Questions

**1. How was the data cleaned and engineered?**
- All columns were standardized, missing values imputed, and new features engineered for risk and efficiency analysis. See notebook cells for code and logic.

**2. What patterns were found in seller reliability, complaints, and delays?**
- Top/bottom sellers, complaint-prone categories, and delay-prone regions were identified. Lagos zone was excluded from delay analytics due to unreliable data.

**3. How was review fraud detected?**
- Sellers with only 5-star ratings and high return/complaint rates, and those with repetitive review texts, were flagged as suspicious. Automated logic is provided in the notebook.

**4. How was the impact of delivery method on ratings validated?**
- ANOVA was used to test for significant differences in customer ratings by delivery method. Results are documented in the notebook.

**5. How was data imbalance handled in modeling?**
- SMOTE was used to balance the training set for return prediction models. Model performance was evaluated and documented.

**6. What strategies and policies are recommended?**
- Actionable strategies for reducing delays and improving trust are provided, along with a Customer Trust Policy and recommendations for seller suspension and category regulation.

**7. What signals should be monitored for review fraud?**
- Mismatches between high ratings and negative outcomes, repetitive review texts, and abrupt changes in review volume should be flagged. Automated detection logic is recommended.

---

## Documentation & Transparency
- All code, logic, and business decisions i got are documented in the notebook and this report.
- Adjustments (e.g., exclusion of Lagos data) are clearly flagged for stakeholders.
- Recommendations are based on reproducible analytics and model results.

---

## Appendix
- See notebook for all code, visualizations, and step-by-step analysis.
- For further questions or custom analyses, refer to the notebook or contact the data science team (pun intended lol...).
- Had fun with project, hope to have feedback on what can be improved and what can be done better.

