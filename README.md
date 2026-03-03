# 📊 bank-marketing-eda
## 1. Project overview
This project consists of an Exploratory Data Analysis (EDA) of a Portuguese bank’s direct marketing campaigns. The objective is to analyze customer characteristics and campaign-related variables to identify patterns associated with subscription to a term deposit product.

The analysis was performed using Python and Pandas in Visual Studio Code.
## 2. Objectives
The main objective of this project is:

To clean and transform the datasets.

To perform descriptive statistical analysis.

To explore relationships between customer attributes, campaign variables, and subscription outcome.

To extract actionable insights from the data.
## 3. Datasets Description
Two datasets were used:

3.1 bank-additional.csv

Contains information related to:

Customer demographics (age, job, marital status, education)

Financial attributes (default, housing loan, personal loan)

Campaign information (duration, campaign, pdays, previous, poutcome)

Macroeconomic indicators

Target variable (y – subscription)

3.2 customer-details.xlsx

Contains additional customer information:

Income

Household composition (Kidhome, Teenhome)

Date of becoming a customer

Website activity (NumWebVisitsMonth)

Both datasets were merged using the customer ID.
## 4. Data Cleaning and Transformation
The following steps were performed:

Checked for missing values and inconsistencies.

Converted date columns to datetime format.

Created new features such as:

tenure_years

contacted_before

Verified data types.

Ensured correct merging between datasets.

Removed unnecessary or duplicated columns where applicable.
## 5. Exploratory Data Analysis
The analysis included:

Descriptive statistics (mean, median, standard deviation).

Distribution analysis of numerical variables.

Conversion rate comparison across different categories.

Visualization using matplotlib and seaborn.

Grouped analysis using Pandas (groupby, aggregations).

Conversion rate was used as the main metric to evaluate differences between groups.
## 6. Key Findings
### 6.1 Demographic Variables

Income, tenure, and number of website visits showed no significant differences in conversion rate.

Single clients showed higher subscription rates.

Clients with higher levels of education showed higher subscription rates.

This suggests that financial literacy and personal circumstances may influence the decision more than income level alone.
### 6.2 Campaign Variables

The strongest relationships with subscription were observed in:

Call duration (longer calls were associated with higher conversion rates).

Previous campaign success (poutcome = success).

Clients who had been previously contacted.

This indicates that prior relationship and engagement level play a key role in subscription likelihood.

Note: Call duration is a post-contact variable and may not be available before the call takes place.
## 7. Business Recommendations
Based on the analysis:

The bank could prioritize clients with previous successful subscriptions.

Maintaining client relationships across campaigns may increase efficiency.

Targeting highly educated and single clients may improve conversion rates.

Income alone should not be considered a primary segmentation criterion.
## 8. Tools Used
- Python

- Pandas

- Matplotlib

- Seaborn

- Visual Studio Code

## 9. Repository Structure
--/ data/ raw → Original datasets

--/ data/ processed → Cleaned and transformed datasets

--/ notebooks → Analysis notebooks

README.md → Project documentation