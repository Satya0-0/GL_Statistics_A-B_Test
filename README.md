# Statistics - A/B-Test

# E-news Express - A/B Testing Analysis

## Project Overview
This project analyzes A/B testing data from E-news Express, an online news portal that aims to expand its business by acquiring new subscribers. The company conducted an experiment to test the effectiveness of a new landing page design in gathering new subscribers, comparing it against the existing design.

## Business Context
E-news Express has observed a decline in new monthly subscribers. The executives believe this decline is due to the current webpage not being designed well enough to keep potential customers engaged. The design team created a new landing page with an improved outline and more relevant content, and the data science team conducted an A/B test to evaluate its effectiveness.

## Experimental Design
- **Sample**: 100 users randomly selected and divided equally into two groups:
  - **Control Group**: Shown the existing landing page
  - **Treatment Group**: Shown the new landing page
- **Data Collected**: User interactions with both versions of the landing page
- **Significance Level**: 5%

## Research Questions
1. Do users spend more time on the new landing page than on the existing landing page?
2. Is the conversion rate for the new page greater than the conversion rate for the old page?
3. Does the converted status depend on the preferred language?
4. Is the time spent on the new page the same for different language users?

## Data Dictionary
- **user_id**: Unique identifier for each user visiting the website
- **group**: Whether the user belongs to the control or treatment group
- **landing_page**: Whether the landing page is new or old
- **time_spent_on_the_page**: Time (in minutes) spent by the user on the landing page
- **converted**: Whether the user was converted to a subscriber or not
- **language_preferred**: Language chosen by the user to view the landing page (Spanish, English, or French)

## Tools & Libraries Used
- Python 3
- NumPy
- Pandas
- Matplotlib
- Seaborn
- SciPy.stats
- Statsmodels
- Scikit-learn

## Statistical Tests Applied
- **Two Sample Independent T-Test**: To compare time spent on landing pages
- **Two Proportions Z-Test**: To compare conversion rates
- **Chi-Square Test**: To test independence between conversion and language preference
- **One-Way ANOVA**: To compare time spent across different language users

## Key Findings
1. **Time Spent**: Users spend significantly more time on the new landing page (6.22 mins) compared to the old landing page (4.53 mins).
2. **Conversion Rate**: The new page has a significantly higher conversion rate (66%) than the old page (42%).
3. **Language Independence**: The conversion status is independent of the user's preferred language.
4. **Language-based Engagement**: The mean time spent on the new page differs among users of different language preferences.

