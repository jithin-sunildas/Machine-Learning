# Employee Salary Analysis🍀

This project analyzes the relationship between employee age, weight, and salary. The goal is to explore the distribution of salaries across different age and weight groups. Various visualizations and statistical insights are presented to help understand the patterns and trends in employee compensation.

## Dataset💻

The dataset contains the following columns:

- **Age**: The age of the employee.
- **Weight**: The weight of the employee.
- **Salary**: The annual salary of the employee.

The data is used to categorize employees into different age and weight groups and analyze the average salary for each group.

## Key Analysis📝

- **Age Group Analysis**: Categorizes employees into predefined age groups, and calculates the number of employees in each group.
- **Weight Group Analysis**: Categorizes employees into predefined weight groups, and calculates the average salary for each weight group.

## Key Visualizations🤖

1. **Age vs. Salary Distribution**: A bar plot showing the number of employees in each age group and their corresponding average salary.
2. **Weight vs. Salary Distribution**: A bar plot showing the average salary for each weight group.

## Requirements👾

To run this analysis, you will need the following libraries:

- pandas
- numpy
- matplotlib
- seaborn

You can install the required libraries using:

```bash
pip install pandas numpy matplotlib seaborn
```

Anaconda framework is recommended to use jupyter notebook. It's an amazing framework to develop python scripts for AI/ML/Data Science, etc.
https://www.anaconda.com/download

An example code🚀:
```
import pandas as pd
import matplotlib.pyplot as plt
import seaborn as sns

# Load dataset
df = pd.read_csv('employee_data.csv')

# Categorize Age
bins = [18, 23, 25, 31, 36, 40, 46]
labels = ["18-22", "23-24", "25-30", "31-35", "36-40", "40-45"]
df["Age_group"] = pd.cut(df["Age"], bins=bins, labels=labels)

# Categorize Weight
weight_bins = [40, 50, 60, 70, 80, 90, 100]
weight_labels = ["40-49", "50-59", "60-69", "70-79", "80-89", "90-100"]
df["Weight_group"] = pd.cut(df["Weight"], bins=weight_bins, labels=weight_labels, right=False)

# Plot Age vs Salary
age_group_salary = df.groupby("Age_group")["Salary"].mean()
sns.barplot(x=age_group_salary.index, y=age_group_salary.values, palette="Set2")
plt.title("Average Salary by Age Group")
plt.ylabel("Average Salary")
plt.xlabel("Age Group")
plt.show()

# Plot Weight vs Salary
weight_group_salary = df.groupby("Weight_group")["Salary"].mean()
sns.barplot(x=weight_group_salary.index, y=weight_group_salary.values, palette="Set2")
plt.title("Average Salary by Weight Group")
plt.ylabel("Average Salary")
plt.xlabel("Weight Group")
plt.show()
