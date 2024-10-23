# Perfect-Time-for-Meal-in-Mess

## Overview

The **Perfect-Time-for-Meal-in-Mess** project aims to predict the optimal time to visit the mess based on historical crowd data, weather conditions, and special events. By using machine learning techniques, the project helps users minimize their waiting time for meals, enhancing their dining experience.

## Table of Contents

- [Motivation](#motivation)
- [Problem Definition](#problem-definition)
- [Data Generation](#data-generation)
- [Data Preprocessing](#data-preprocessing)
- [Model Training](#model-training)
- [Usage](#usage)
- [Future Work](#future-work)
- [License](#license)
- [Acknowledgments](#acknowledgments)

## Motivation

Long wait times at messes during peak hours can be frustrating for students and staff. This project seeks to analyze patterns in meal timings and predict when the mess is likely to be crowded, allowing users to plan their meals accordingly.

## Problem Definition

The objective is to predict the **waiting time** (in minutes) at any given hour based on:
- Time of day
- Day of the week
- Type of meal (Breakfast, Lunch, Dinner)
- Weather conditions
- Special events

## Data Generation

Since real-world data was not readily available, we generated synthetic data that includes:
- `hour`: Hour of the day (0-23)
- `minute`: Minute of the hour (0-59)
- `day_of_week`: Day of the week (0-6)
- `meal_type`: Type of meal (1: Breakfast, 2: Lunch, 3: Dinner)
- `weather`: Weather conditions (0: Sunny, 1: Cloudy, 2: Rainy, 3: Snowy)
- `event`: Type of event (0: Normal, 1: Sports Day, 2: Cultural Fest, 3: Holiday)
- `waiting_time`: Predicted waiting time in minutes

The generated data is stored in a CSV file for further processing.
Datasets Link : https://www.kaggle.com/datasets/ankitrajsh/mess-waiting-time-datsets

## Data Preprocessing

The preprocessing steps include:
1. Handling missing values
2. One-hot encoding of categorical variables
3. Feature scaling using standardization
4. Splitting the data into training and testing sets

## Model Training

We utilized the **Random Forest Regressor** for this project. The model was trained on the preprocessed dataset, and its performance was evaluated using Mean Absolute Error (MAE) and Root Mean Squared Error (RMSE).

## Usage

To use this project, follow these steps:

1. **Clone the repository:**
   ```bash
   git clone https://github.com/ankitrajsh/Perfect-Time-for-Meal-In-Mess.git



## Usage Instructions

### Install the required dependencies:
```bash
pip install -r requirements.txt
```
## Future Work
- Integrate real-time data from mess counters and weather APIs.
- Deploy the model as a web application for easy access.
- Enhance the model with more advanced algorithms for better accuracy.

## License
This project is licensed under the MIT License. See the LICENSE file for details.

## Acknowledgments
- Inspired by the need for efficient meal planning in institutions.
- Special thanks to machine learning libraries like Scikit-learn for providing easy-to-use tools for model training.

