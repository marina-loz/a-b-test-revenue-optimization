# A/B Testing for an Online Store

##  Project Overview
This project analyzes an A/B test conducted for an online store to evaluate different marketing hypotheses and measure the impact on revenue and conversion rates. The goal is to prioritize hypotheses using ICE and RICE frameworks and assess statistical significance in conversion rates and average order sizes between two groups.

## Dataset Description
The project uses three datasets:
- **hypotheses_us.csv**: Contains marketing hypotheses with Reach, Impact, Confidence, and Effort scores.
- **orders_us.csv**: Includes transaction details such as order ID, user ID, date, revenue, and A/B test group.
- **visits_us.csv**: Tracks the number of visitors per group per day.

## Key Steps in Analysis
1. **Hypothesis Prioritization**  
   - Used **ICE** and **RICE** frameworks to rank hypotheses.
   - Compared how rankings changed between ICE and RICE.

2. **A/B Test Analysis**  
   - **Exploratory Data Analysis (EDA)**: Examined cumulative revenue, average order size, and conversion rates.
   - **Outlier Detection**: Identified and filtered users with extreme order values.
   - **Statistical Testing**:
     - Used **Z-test** for comparing conversion rates.
     - Used **T-test / Mann-Whitney U test** for comparing average order sizes.
   - **Decision Making**: Determined whether to stop or continue the test based on statistical results.

## Key Findings
- The RICE framework prioritized hypotheses with higher **Reach**, which led to different rankings than ICE.
- The A/B test results showed that **conversion rates** were significantly different, while **average order sizes** were not.

## 🛠 Technologies Used
- **Python**: `pandas`, `numpy`, `scipy`, `matplotlib`, `math`
