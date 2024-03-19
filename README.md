# Project 4: Spaceship Titanic

## Overview
This project aims to predict the transportation status of passengers based on various features such as demographics, travel destination, and onboard facilities. The project consists of several Jupyter notebooks and an HTML for visualization, each focusing on different aspects of the data analysis, preprocessing, and model building.


### A Kaggle competition

A Kaggle competition is a data science challenge hosted on the Kaggle platform. Participants engage in competitive data analysis to develop the most accurate predictive models or solutions for specific real-world problems. These competitions provide datasets, evaluation metrics, and problem descriptions to guide participants in their analyses.

Participants leverage machine learning techniques to build predictive models using the provided data. Submissions are evaluated against a holdout dataset, and participants are ranked on a leaderboard based on the performance of their models.

Kaggle competitions serve as a platform for data scientists, machine learning practitioners, and enthusiasts to showcase their skills, learn from others, and address challenging problems across various domains.

## Situation

The Spaceship Titanic embarked on its maiden voyage a month ago, carrying nearly 13,000 passengers from our solar system to three newly habitable exoplanets. Unfortunately, tragedy struck when the spaceship collided with a spacetime anomaly near Alpha Centauri, transporting almost half of the passengers to an alternate dimension.

To aid in the rescue efforts and recover the lost passengers, the challenge is to predict which passengers were transported by the anomaly using records retrieved from the spaceship's damaged computer system.

## Dataset Description | Variables

- `train.csv`: Personal records for approximately two-thirds (~8,700) of the passengers, provided as training data.
  - `PassengerId`: Unique identifier for each passenger, following the format "gggg_pp" where "gggg" indicates a group and "pp" is the passenger's number within the group.
  - `HomePlanet`: The planet the passenger departed from, typically their permanent residence.
  - `CryoSleep`: Indicates if the passenger elected suspended animation for the voyage, confining them to their cabins.
  - `Cabin`: Passenger's cabin number in the format "deck/num/side" (e.g., "A/23/S" for Starboard side).
  - `Destination`: The planet the passenger is destined for.
  - `Age`: Passenger's age.
  - `VIP`: Whether the passenger paid for VIP service.
  - `RoomService`, `FoodCourt`, `ShoppingMall`, `Spa`, `VRDeck`: Expenses at various amenities aboard the Spaceship Titanic.
  - `Name`: Passenger's full name.
- `test.csv`: Personal records for the remaining one-third (~4,300) of the passengers, to be used for prediction.
  - `PassengerId`: Identifier for each passenger in the test set.
- `sample_submission.csv`: Submission file format.
  - `PassengerId`: Identifier for each passenger in the test set.
  - `Transported`: Target variable to predict, indicating if the passenger was transported by the anomaly (True/False).

This competition presents an opportunity to apply data science skills to a unique scenario, contributing to the rescue mission of the Spaceship Titanic's lost passengers.




## Setup and Dependencies

To run the code in the Jupyter notebook, the following dependencies need to be installed:

- Python 3.x
- Jupyter Notebook
- Pandas
- PySpark
- Scikit-learn
- TensorFlow
- Graphviz
- Matplotlib
- Seaborn

## Notebooks Description
1. **EDA.ipynb (Exploratory Data Analysis)**
   - This notebook focuses on exploratory data analysis (EDA) to gain insights into the dataset.
   - It includes loading the data, understanding the data schema, and basic statistical summaries.
   - Visualizations such as histograms, box plots, and correlation matrices are used to analyze the distribution and relationships between variables.
   - The goal is to understand the characteristics of the dataset and identify patterns that may be useful for modeling.

2. **Base_predictions.ipynb (Baseline Predictions)**
   - This notebook establishes a baseline for prediction by implementing simple models without any preprocessing.
   - It typically includes building and evaluating basic models like logistic regression or decision trees directly on raw data.
   - The purpose is to set a benchmark for model performance, which subsequent models can aim to improve upon.

3. **NaN_treatment.ipynb (Missing Values Treatment)**
   - This notebook focuses on handling missing values in the dataset.
   - Techniques such as imputation, deletion, or interpolation may be applied to deal with missing data effectively.
   - The goal is to ensure that the dataset is clean and ready for further analysis and modeling.

4. **Final_model_predictions.ipynb (Final Model Building and Predictions)**
   - This notebook represents the final stage of the project, where the best-performing model is built and used for predictions on unseen test data.
   - It includes advanced preprocessing steps, such as feature engineering, encoding categorical variables, and scaling numerical features.
   - The best model (often determined through hyperparameter tuning) is trained on the preprocessed data and evaluated using appropriate metrics.
   - Predictions are made on the test dataset, and the results are saved for further analysis or submission.

## Conclusion
Each notebook in this project serves a specific purpose in the data analysis and modeling pipeline. By following this structured approach, we aim to develop accurate predictive models while ensuring the integrity and quality of the data throughout the process.
