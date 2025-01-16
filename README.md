Project 1: Layoffs Data Cleaning
This project focuses on cleaning a messy dataset to ensure accuracy and reliability for analysis. Key steps included:

Key Steps:
Removing Duplicates:

Identified duplicates using ROW_NUMBER with PARTITION BY on key columns.
Deleted duplicate rows after assigning row numbers, ensuring unique records.
Standardizing Data:

Trimmed whitespaces and normalized inconsistent entries (e.g., country names like "United States." to "United States").
Standardized industry names (e.g., variations of "Crypto" unified under a single label).
Converted date columns to a uniform DATE format using STR_TO_DATE.
Handling Missing Values:

Imputed missing industries based on non-null values from duplicate company records.
Flagged and reviewed records with null values for total_laid_off and percentage_laid_off.
Final Preparation:

Dropped temporary columns used during cleaning (e.g., row_num).
Verified the cleaned dataset for consistency and readiness for analysis.
Outcome:
This process ensures the dataset is deduplicated, standardized, and enriched, enabling accurate and meaningful insights in subsequent analysis stages.

Project 2: Layoffs Exploratory Data Analysis
Objective:
Analyze global layoffs data to identify trends, key contributors, and industry-wide impacts.

Key Tasks:
Data Exploration:

Queried layoffs_staging2 for metrics like total_laid_off and percentage_laid_off.
Identified companies with 100% layoffs, often signaling closures.
Trend Analysis:

Examined layoffs over time, calculating monthly, yearly, and rolling totals.
Identified peak layoff periods and recovery trends.
Aggregated Insights:

Summarized layoffs by company, industry, country, and funding stage.
Ranked top companies by layoffs per year using dense ranking.
Key Findings:

Highlighted industries, regions, and companies most affected.
Revealed relationships between funding stage and layoff scale.
Value:
Provides actionable insights into global layoffs, supporting informed decisions in workforce planning and policy-making.

SQL scripts ensure clarity and reproducibility for future analyses.
