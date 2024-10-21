# Gym-Exercise-Data-Analysis
## Overview
This project analyzes a dataset containing gym members' exercise routines, physical attributes, and fitness metrics. The dataset includes 973 samples with features such as age, gender, heart rate, workout duration, calories burned, and body measurements like BMI and body fat percentage. The goal of the analysis is to uncover fitness patterns and predict key health metrics, such as BMI, using various machine learning models.

## Dataset Features
- Age: The age of gym members.
- Gender: The gender of gym members (Male/Female).
- Weight (kg) & Height (m): Physical measurements of gym members.
- Heart Rate Data: Maximum, average, and resting heart rates.
- Session Duration: The length of workout sessions in hours.
- Calories Burned: Total calories burned per workout session.
- Workout Type: Type of workout (e.g., Cardio, Strength, Yoga, HIIT).
- Fat Percentage: Body fat percentage of the members.
- Water Intake: Water consumed during workouts (liters).
- Workout Frequency: Number of workout sessions per week.
- Experience Level: Member’s experience level, from beginner to advanced.
- BMI: Body Mass Index, calculated from height and weight.

## Exploratory Data Analysis (EDA)
The exploratory analysis revealed several important insights:
- Popular Workout Types: Strength and Cardio were the most common workout types, followed by HIIT and Yoga.
- Calories Burned: A strong positive correlation was found between session duration and calories burned.
- Gender Distribution: The dataset had an almost equal number of male and female members.
- Experience vs. Body Fat: More experienced gym members tended to have a lower body fat percentage.

## Machine Learning Models
To predict BMI, several regression models were trained, including:
- Linear Regression: A baseline linear model.
- Ridge Regression: A regularized linear model with L2 regularization.
- Lasso Regression: A regularized model with L1 regularization for feature selection.
- Decision Tree Regressor: A non-linear, tree-based model.

## Model Results

| Model                  | MSE  | R²    |
|------------------------|------|-------|
| Linear Regression       | 1.28 | 0.72  |
| Ridge Regression        | 1.25 | 0.73  |
| Lasso Regression        | 1.35 | 0.70  |
| Decision Tree Regressor | 1.45 | 0.68  |

## Best Model
- Ridge Regression was the best performing model, minimizing error and achieving the highest R² value (0.73). This model effectively captured the linear relationship between features like calories burned, session duration, and BMI.
##  Key Insights
- Session Duration and Calories Burned were strong predictors of BMI.
- Experience Level and Workout Type also played important roles in determining members' physical health metrics.
- Ridge Regression proved to be the most suitable model for this dataset, offering better generalization due to its regularization of the model's complexity.

# Conclusion
This analysis provides valuable insights into the relationship between workout routines and physical health metrics. With further fine-tuning and experimentation, these models can help predict fitness outcomes more accurately and guide health-related decision-making.
