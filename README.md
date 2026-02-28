**📉 Telco Customer Churn & Retention Analysis**
Internship: Future Interns Data Analytics (Task 2)

Tool Stack: Power BI, Power Query, DAX, GitHub

**📑 Project Overview**
This project focuses on Customer Attrition Analysis for a Telecommunications company. By analyzing a dataset of 7,043 customers, I identified key factors that drive churn and developed an interactive dashboard to help stakeholders visualize retention trends and customer lifetime patterns.

**🛠️ Data Cleaning & Engineering (Power Query)**
To ensure the accuracy of the analysis, the following data cleaning steps were performed:

Data Type Correction: Converted TotalCharges from text to decimal after handling invisible empty strings (replaced with 0).

Logical Transformation: Updated SeniorCitizen from binary (0/1) to descriptive text ("Yes/No") for better report readability.

Tenure Grouping (Cohort Analysis): Created a conditional column Tenure Segment to group customers into 0-6 months, 6-12 months, 1-2 years, and 2+ years.

Data Consolidation: Simplified service columns by merging "No internet service" into "No" to clean up visualization legends.

**📈 DAX Measures Created**
The following measures were developed to track KPIs:

Total Customers: COUNTROWS('Table')

Churn Rate %: DIVIDE(CALCULATE([Total Customers], [Churn] = "Yes"), [Total Customers], 0) (Target: ~26.5%)

**📊 Key Insights & Findings**
Contract Risk: Customers on Month-to-Month contracts have the highest churn rate.

Service Drivers: Fiber Optic users are leaving at a higher rate than DSL users, suggesting a need for price-to-value review.

Critical Period: Churn is highest in the first 6 months of the customer journey.

Payment Method: Customers using Electronic Checks show a higher tendency to churn compared to those on automated credit card payments.

**💡 Strategic Recommendations**
Incentivize Long-term Contracts: Offer a small discount or loyalty bonus for customers who switch from monthly to annual plans.

Early Intervention: Implement an automated "Customer Success" check-in for all new users during their 3rd month.

Fiber Optic Retention: Investigate the stability of Fiber Optic services in high-churn regions to ensure service quality matches the premium price.
