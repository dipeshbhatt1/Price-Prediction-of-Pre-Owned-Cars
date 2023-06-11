
# Price-Prediction of pre-owned Cars

<img src="[nexon-ev-exterior-front.jpeg](https://github.com/dipeshbhatt1/images/blob/808e5ec220a6179369ca5d6fd9ae9284411c7de9/nexon-ev-exterior-front.jpeg)" width="250" height="175">
## Description

* The project involves usage of labeled dataset, extracted from spinny.com using web scraping, to build a Linear Regression model that predicts the prices of used cars.
* The idea behind this was to build a smart model that could help buyers to know a reasonable price of used cars based on his desired features, and a seller to get a reliable idea of the current value of their used car.
## Dataset
* Data of over 2000 pre-owned cars was extracted from spinny.com
* After applying feature engineering and data preparation we are left with data of over 1k pre-owned cars
* Download the dataset for custom training: LINK


## Installation
**Requirements**

```bash
  * Python 3.7+
  * IDE (Jupyter Notebook, VS Code, Spyder, etc)
  * selenium
  * Web Driver (Chrome, Firefox, Edge, Safari, etc)
  * scikit-learn
  * Other python libraries like numpy and pandas
```
    
## Setup
1. Install latest version of python:
```bash
    https://www.python.org/downloads/
```
2. If pip is not installed, you can follow the instructions:
```bash
    https://pip.pypa.io/en/stable/installing/
```
3. Install jupyter using command prompt:
```bash
    pip install jupyter
```
4. Install python libraries viz. numpy, pandas, seaborn, matplotlib, selenium, sklearn and time, one-by-one using command prompt:
```bash
    pip install numpy
```
5. Once you have these all, launch the Jupyter Notebook using command prompt:
```bash
    jupyter notebook
```
6. Now you can start working on the project using the given dataset and python codes
## Steps Involved (End to End)

1. **Objective:** To build a Machine Learning model (Linear Regression) that can predict prices (label) of used cars based on various features
2. **Availability of Dataset:** For this, a reasonable and large enough dataset was required. Now, instead of looking for some old data or sample data available on internet, I decided to scrape website of a service provider already working in this field. So, I came across spinny.com which has a simple yet cool UI. Finally, the data was scrapped from this website.
3. **Feature Engineering:** Initially the dataset had all the data in just 7 columns, the data had null values, duplicates and noise too. After applying techniques like Data Cleaning (imputation, outlier detection, and removing duplicate records), EDA, and Feature Generation, total 14 meaningful features were generated, which can be used for drawing insites through aggregations and visualistion. Then, I applied some final techniques, to prepare final data for training the model, like Feature Selection, Feature Encoding, Feature Scaling. The final dataset has the following features:
```bash
    model (year)
    km driven (in thousands)
    mileage (in kmpl)
    seating capacity (units)
    fuel_type_ Petrol
    fuel_type_ Diesel
    fuel_type_ Petrol+cng
    transmission_ Automatic
    transmission_ Manual
    ground clearance (in mm)
    boot space (in litres)
    fuel tank capacity (in litres)
    max power (in bhp)
```
4. **Training:** The final dataset was then split into training and testing datasets and trained through Linear Regression.
5. **Testing:** The predicted values for the label (price) were then generated. The accuracy came out to be 85% using R2 score metric and 84% using Adjusted R2 score method.
6. **Predicting (Applying the Model):** As a test case, predicting the price of a used car using hypothetical features seems to be quite reasonable and meaningful. The model now can be used by a user who may be buyer/seller to predict prices of pre-owned cars.
## Screenshots

![App Screenshot](https://via.placeholder.com/468x300?text=App+Screenshot+Here)

