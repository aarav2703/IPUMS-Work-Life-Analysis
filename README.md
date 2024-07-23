# Work-Life Balance and Health Outcomes Analysis

## Project Overview
This project aims to analyze the relationship between work-life balance and health outcomes using survey data. The analysis focuses on exploring various health-related variables and their association with work-related factors. Using a comprehensive dataset, the project seeks to uncover patterns and insights that can inform policies to improve work-life balance and overall health.

**Note:** This project includes static visualizations created in Google Colab, without an interactive dashboard.

### Links:
- **Code Notebook**: [Work_Life_Balance_Health_Analysis.ipynb](https://colab.research.google.com/drive/your-notebook-link)

## Objectives
- **Correlation Analysis**: Examine relationships between various health and work-related variables.
- **Health and Work Analysis**: Visualize the distribution of health statuses, depression frequencies, and hours worked per week.
- **Regression Analysis**: Explore the impact of hours worked on health status through linear regression.
- **Predictive Modeling**: Use logistic regression to predict depression frequency based on employment status.

## Data Sources
- **National Health Interview Survey (NHIS)**: Comprehensive survey data on health and work-related factors from the IPUMS NHIS website.

## Tools and Technologies
- **Python**: The primary programming language used for data processing and analysis.
- **Pandas**: For data manipulation and cleaning.
- **Matplotlib and Seaborn**: Used for creating visualizations.
- **Google Colab**: Environment for developing and testing the code.

## Data Acquisition
The data for this project was sourced from the IPUMS NHIS website, where I selected the necessary variables and sample years. The IPUMS NHIS website allows researchers to customize their datasets by choosing specific variables and sample years relevant to their study. For this analysis, I focused on variables related to health status, work hours, depression, and employment status, covering multiple years to ensure a comprehensive analysis.

## Key Steps and Methodologies
1. **Data Acquisition**: Loading and inspecting the NHIS dataset.
2. **Data Cleaning and Preprocessing**: Handling missing values, converting data types, and preparing the data for analysis.
3. **Exploratory Data Analysis (EDA)**: Initial exploration to understand the dataset structure and key statistics.
4. **Visualizations**:
   - **Correlation Matrix**: Heatmap to visualize correlations between variables.
   - **Distribution of Depression Frequency**: Bar chart to show the frequency of depression occurrences.
   - **Distribution of Health Status**: Bar chart to visualize health status distribution.
   - **Distribution of Hours Worked Per Week**: Histogram and KDE plot to show hours worked.
   - **Average Health Status by Employment Status**: Bar chart to compare health status across different employment statuses.
   - **Linear Regression: Health Status vs. Hours Worked**: Scatter plot with regression line.
   - **Confusion Matrix: Depression Frequency vs. Employment Status**: Heatmap to evaluate logistic regression performance.

## Data Visualization and Insights

### Correlation Matrix
![Correlation Matrix](file-TYxxMs3Ija6bcQXeUrkn5ebP)

The correlation matrix provides a comprehensive overview of the relationships between different variables in the dataset. Some key observations include:
- **Health Status (HEALTH)** has a negative correlation with **Work Loss Days (WLDAYR)**, suggesting that poorer health is associated with more work loss days.
- **Depression Frequency (DEPFREQ)** is positively correlated with **Depression Medication (DEPRX)**, indicating that those who frequently feel depressed are more likely to be on medication.
- **Hours Worked (HOURSWRK)** has a slight negative correlation with **Health Status (HEALTH)**, implying that longer working hours might be associated with poorer health outcomes.

### Distribution of Depression Frequency
![Distribution of Depression Frequency](file-oTqFrSoWXS87nreHuT9g6jsg)

The distribution shows that the majority of respondents never feel depressed (DEPFREQ = 5), followed by those who feel depressed a few times a year (DEPFREQ = 4). This indicates that while depression is a significant issue for some, the majority of the population reports infrequent feelings of depression.

### Distribution of Health Status
![Distribution of Health Status](file-SbCnG6f0atQkajNYe9M3vG0V)

The health status distribution reveals that most respondents rate their health as **Excellent (HEALTH = 1)** or **Very Good (HEALTH = 2)**. This suggests a generally healthy population, although there is still a notable portion reporting lower health statuses.

### Distribution of Hours Worked Per Week
![Distribution of Hours Worked Per Week](file-7f9HZsUUDYbvDaIjODx2Jkuo)

The distribution shows a bimodal pattern, with peaks at **0 hours** and around **40 hours**. This indicates a mix of individuals who are either not working or working full-time. There is also a smaller peak around **20 hours**, which might represent part-time workers.

### Average Health Status by Employment Status
![Average Health Status by Employment Status](file-tEYnkLCNdh4BoK0UOw0XrkTH)

The analysis reveals that individuals who are **Not Employed (EMPSTAT = 200)** or **Not in the Labor Force (EMPSTAT = 220)** tend to report better health statuses compared to those who are employed. This could suggest that employment, especially under certain conditions, might have a negative impact on health.

### Linear Regression: Health Status vs. Hours Worked
![Linear Regression: Health Status vs. Hours Worked](file-WgsN6c3TX8yrpaV36ygbbZpe)

The linear regression plot shows a slight negative slope, indicating that as hours worked per week increase, health status tends to decrease slightly. However, the variation in health status is quite large, suggesting that factors other than work hours also play a significant role in determining health.

### Confusion Matrix: Depression Frequency vs. Employment Status
![Confusion Matrix: Depression Frequency vs. Employment Status](file-LV8ECQsxZfWo79aWTrGTR0Qz)

The confusion matrix for logistic regression reveals that the model has a high rate of correctly predicting individuals who do not experience daily depression. However, it struggles with accurately predicting daily depression occurrences, suggesting that more factors need to be considered to improve the model's predictive power.

### Conclusion and Next Steps:
- **Geographic Disparities**: Address disparities in patient ratings across different states by analyzing state-specific factors.
- **Targeted Improvements**: Focus on lower-rated hospitals in high-performing states to identify and replicate best practices.
- **Response Rates**: Investigate methods to improve survey response rates, particularly in states and hospitals with low engagement.
- **Systemic Issues**: Further analyze socio-economic and policy-related factors contributing to lower ratings in certain states.

## How to Use
1. **Clone the Repository**: Clone this repository to your local machine.
2. **Install Dependencies**: pandas, matplotlib, seaborn.
3. **Run the Notebook**: Execute the Jupyter notebook in Google Colab or any local Jupyter environment to generate the visualizations.

## Acknowledgements
- **IPUMS NHIS**: For providing access to comprehensive survey data.
- **Google Colab**
- **Pandas, Matplotlib, Seaborn**: For data manipulation and visualization

## Citation
- IPUMS NHIS. National Health Interview Survey Data.
