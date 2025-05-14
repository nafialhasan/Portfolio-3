# Portfolio 3: Analysis of Mobile Price Data

This repository contains my solutions for the Portfolio 3 assignment for the course COMP6200 – Data Science. The assignment involves analyzing a mobile price dataset to predict mobile phone price ranges using classification models, and evaluating the strengths and weaknesses of these models.

## Contents

- `Portfolio 3_Analysing Mobile Price Data.ipynb`: The Jupyter notebook containing the questions, solutions, code, and analysis for Portfolio 3.

## Assignment Details

### Analysis of Mobile Price Data

The goal of this analysis task is to train classification models to predict mobile phone prices ('price range' in the dataset) and evaluate the strengths and weaknesses of these models. The dataset contains details about mobile phone hardware, specifications, and prices.

#### Dataset Description

The dataset includes the following fields:

- **battery_power**: Total energy a battery can store in one time measured in mAh
- **blue**: Has Bluetooth or not (0: No, 1: Yes)
- **clock_speed**: Speed at which microprocessor executes instructions
- **dual_sim**: Has dual SIM support or not (0: No, 1: Yes)
- **fc**: Front Camera mega pixels
- **four_g**: Has 4G or not (0: No, 1: Yes)
- **int_memory**: Internal Memory in Gigabytes
- **m_dep**: Mobile Depth in cm
- **mobile_wt**: Weight of mobile phone
- **n_cores**: Number of cores of processor
- **pc**: Primary Camera mega pixels
- **px_height**: Pixel Resolution Height
- **px_width**: Pixel Resolution Width
- **ram**: Random Access Memory in Mega Bytes
- **sc_h**: Screen Height of mobile in cm
- **sc_w**: Screen Width of mobile in cm
- **talk_time**: Longest time that a single battery charge will last when you are
- **three_g**: Has 3G or not (0: No, 1: Yes)
- **touch_screen**: Has touch screen or not (0: No, 1: Yes)
- **wifi**: Has Wi-Fi or not (0: No, 1: Yes)
- **price_range**: Target variable with value of 0 (low cost), 1 (medium cost), 2 (high cost), and 3 (very high cost)

### Tasks and Solutions

#### Explore the Data and Clean the Data
**Task:** Remove abnormal instances and replace missing values.
- **Actions:**
  - Checked for missing values and replaced them with respective feature means.
  - Verified the dataset to ensure no missing values remain.

#### Study the Correlation between Features and Price Range
**Task:** Calculate the correlations and select variables helpful for predicting the price range.
- **Actions:**
  - Calculated the correlation coefficients between 'price_range' and other features.
  - Selected the four most correlated features: `ram`, `battery_power`, `px_width`, `px_height`.

#### Split the Dataset
**Task:** Split the dataset into training (80%) and testing (20%) sets.
- **Actions:**
  - Used `train_test_split` to split the data.

#### Train a Logistic Regression Model
**Task:** Train a logistic regression model using the selected features.
- **Actions:**
  - Trained the model and calculated accuracy on both training and testing sets.
  - Evaluated the model's performance.

#### Train a KNN Model
**Task:** Train a K-Nearest Neighbors (KNN) model using the selected features.
- **Actions:**
  - Trained the KNN model with an initial value of K (ad-hoc selection of K=22).
  - Calculated accuracy on both training and testing sets.
  - Evaluated the model's performance.

#### Tune the Hyper-parameter K in KNN
**Task:** Tune K using GridSearchCV and visualize the results.
- **Actions:**
  - Used `GridSearchCV` to find the optimal value of K.
  - Plotted K against mean accuracy scores on the test set.
  - Analyzed how K influences prediction performance.

## Repository Structure

- `README.md`: This file, providing an overview of the repository contents and assignment details.
- `Portfolio 3_Analysing Mobile Price Data.ipynb`: The main assignment file containing questions, solutions, code, and analysis.

## Contact Information

For any queries or further information, feel free to contact me at [nafialhasan@gmail.com](mailto:nafialhasan@gmail.com).  
You can also connect with me on [LinkedIn](https://www.linkedin.com/in/nafialhasan/).

