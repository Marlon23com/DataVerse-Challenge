# Jumia Jitters Challenge

A retail risk analytics project focused on seller reliability, review fraud detection, and logistics performance for the Jumia marketplace dataset.

## Project Overview
This project explores how seller behavior, product complaints, delivery delays, and review patterns can be used to flag operational and trust risks. The analysis combines data cleaning, feature engineering, exploratory analytics, and predictive modeling to support actionable business decisions.

## Objectives
- Clean and prepare the dataset for analysis
- Detect suspicious seller and review patterns
- Analyze product/category complaint trends
- Measure delivery and logistics inefficiencies
- Build a risk-focused predictive model
- Recommend operational policies and seller interventions

## Key Findings
- Certain sellers consistently underperform on delivery reliability and complaint resolution.
- Some product categories show recurring customer dissatisfaction and return spikes.
- Repetitive review text and unusually positive ratings alongside high complaints are strong fraud indicators.
- Logistics delay hotspots significantly affect customer trust and order experience.
- Data imbalance limits the effectiveness of pure return-prediction models, but feature engineering improves risk detection.

## Workflow
### 1. Data Cleaning and Feature Engineering
- Standardized inconsistent identifiers and category values
- Converted dates and calculated delivery delay metrics
- Engineered seller risk, return, review, and delivery-efficiency features
- Imputed missing values using appropriate business-aware strategies

### 2. Analytics and Visualization
- Ranked top and bottom sellers by fulfillment performance
- Identified the most complaint-prone categories
- Mapped delay-heavy regions and logistics bottlenecks
- Flagged suspicious review behavior using textual and behavioral patterns

### 3. Risk Modeling
- Applied class balancing techniques for predictive modeling
- Built classification models using both structured features and review text features
- Evaluated performance through accuracy, confusion metrics, and classification reports

### 4. Business Recommendations
- Prioritize high-delay regions and logistics partners
- Apply customer trust policies and seller monitoring controls
- Regulate high-risk categories and suspend suspicious sellers
- Introduce review-fraud detection automation for ongoing monitoring

## Repository Files
- [Jumia_Jitters_Report.md](Jumia_Jitters_Report.md) — business-focused report and executive summary
- [Tinotenda Makwara Dataverse Africa July Challenge.ipynb](Tinotenda%20Makarwa%20Dataverse%20Africa%20July%20Challenge.ipynb) — full analysis, code, and visualizations
- [jumia_jitters_dataset.csv](jumia_jitters_dataset.csv) — raw dataset
- [jumia_jitters_cleaned.csv](jumia_jitters_cleaned.csv) — cleaned dataset used for analytics

## Project Status
This project was completed as part of the DataVerse Africa challenge and focuses on seller risk profiling and trust optimization for an e-commerce environment.

## Notes
The report and notebook document the complete process, including model decisions, assumptions, and stakeholder-friendly recommendations.

## License
This project is shared for educational and portfolio use.
