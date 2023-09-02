# <img src="Media Files/icon.png" width="50" height="30"> Price-Prediction of pre-owned Cars <img src="Media Files/icon2.png" width="50" height="32">

<img src="Media Files/1.jpg" width="400" height="200"> <img src="Media Files/2.jpg" width="400" height="200">
<p align="center"><img src="Media Files/3.jpg" width="400" height="250">
 <br>
<p align="center"><img src="Media Files/4.jpg" width="310" height="180"> <img src="Media Files/5.jpg" width="420" height="200">
<p align="center"><img src="Media Files/TATA NEXON GIF.gif" width="400" height=250">
 
<br>
<p align="center"><img src="https://forthebadge.com/images/badges/made-with-python.svg"></a></p>

## 📝 Description
* This repository represents **"Price-Prediction using a Multiple Linear Regression Model"**
* With the help of this project we can meaningfully and reliably predict prices of pre-owned cars based on some relevant characteristics.

## ⏳ Dataset 
* Data of over 6000 pre-owned cars was extracted from spinny.com
* After applying data cleaning, organization, and feature engineering we are left with data from over 1300 pre-owned cars
* Download the dataset for custom training:
  https://github.com/dipeshbhatt1/Price-Prediction-of-Pre-Owned-Cars/tree/main/Datasets

## 🏽‍ Download Model File
- Download the model file: https://github.com/dipeshbhatt1/Price-Prediction-of-Pre-Owned-Cars/blob/main/Python%20Codes%20(in%20ipynb)/C-analysis-and-model.ipynb

## :desktop_computer:	Installation

### :hammer_and_wrench: Requirements
```bash
  * Python 3.7+
  * IDE (Jupyter Notebook, VS Code, Spyder, etc)
  * selenium
  * Web Driver (Chrome, Firefox, Edge, Safari, etc)
  * scikit-learn
  * Other python libraries like numpy and pandas
```
    
## :gear: Setup
1. Install latest version of python:
    https://www.python.org/downloads/
2. If pip is not installed, you can follow the instructions:
    https://pip.pypa.io/en/stable/installing/
3. Install jupyter using command prompt:
```bash
    pip install jupyter
```
4. Install python libraries viz. numpy, pandas, seaborn, matplotlib, selenium, sklearn and time, one-by-one using command prompt:
```bash
    pip install numpy
```
5. Once you have these all, launch the Jupyter Notebook using the command prompt:
```bash
    jupyter notebook
```
6. Now you can start working on the project using the given dataset and Python codes

## <img src="Media Files/steps3.png" width="45" height="40"> Steps Involved

1. **Objective:** To build a Machine Learning model (Linear Regression) that can predict prices (label) of used cars based on various features
2. **Data Collection:** For this, a reasonable and large enough dataset was required. Now, instead of looking for some old data or sample data available on the internet, I decided to scrape the website of a service provider already working in this field. So, I came across spinny.com which has a simple yet cool UI. Finally, the data was scrapped from this website.
3. **Data Cleaning & Feature Engineering:** Initially the dataset had all the data in just 7 columns, the data had null values, duplicates, and noise too. After applying techniques like Data Cleaning (imputation, outlier detection, and removing duplicate records), EDA, and Feature Generation, a total of 14 meaningful features were generated, which can be used for drawing insights through aggregations and visualization. Then, I applied some final techniques, to prepare the final data for training the model, like Feature Selection, Feature Encoding, and Feature Scaling. The final dataset has the following independent features:
```bash
    brand
    body type
    fuel type
    transmission
    model (year)
    km driven (in thousands)
    mileage (in kmpl)
    seating capacity (units)
    ground clearance (in mm)
    boot space (inliterss)
    fuel tank capacity (inliterss)
    max power (in bhp)
```
4. **Data Analysis and Visualisation:** Meanwhile data analysis through groupby, pivot table, and aggregate functions was also done and the data was visualized (screenshots may be referred to).
5. **Training:** The final dataset was then split into training and testing datasets and trained through Linear Regression.
6. **Testing:** The predicted values for the label (price) were then generated. The accuracy came out to be 85% using the R2 score metric and 84% using the Adjusted R2 score method.
7. **Predicting (Applying the Model):** As a test case, predicting the price of a used car using hypothetical features seems to be quite reasonable and meaningful. The model now can be used by a user who may be a buyer/seller to predict the prices of pre-owned cars.

 ## Data Visualisation and Insights

<img src="Screenshots/Average Price of cars graph.jpg" width="350" height="300"> <img src="Screenshots/Correlation between mileage and price.jpg" width="350" height="300">
<br>
**• The average price of MG cars is the highest among all brands.**
<br>
**• On average, Prices are falling with increasing Mileage.**
<br>
****
<img src="Screenshots/Pie chart showing percentage of cars of different fuel types.jpg" width="350" height="260"> <img src="Screenshots/Pie chart showing percentage of cars of different body-types.jpg" width="350" height="260">
<br>
**• The most commonly available fuel-type is Petrol followed by Diesel.**
<br>
**• The most commonly available body type is Hatchback followed by SUV.**
<br>
****
<img src="Screenshots/Number of cars of different brands.jpg" width="350" height="300"> <img src="Screenshots/Car body-type vs average Price (in lakh Rs.).jpg" width="400" height="300">
<br>
**• The most commonly available car Brand is the Maruti Suzuki.**
<br>
**• The average price of SUV cars is the highest among all available body types.**
<br>
****
<img src="Screenshots/Outlier Analysis of Mileage (in kmpl).jpg" width="350" height="300"> <img src="Screenshots/Correlation among continuous features.jpg" width="450" height="300">
<br>
**• Some outliers are present in the Mileage column roughly below 15 kmpl and above 25 kmpl.**
<br>
**• The Pearson correlation among the numerical features shows that there's no multicollinearity among the features at this stage.**
<br>
**• Some obvious patterns are also visible such as model year and km driven, mileage and price, km driven and price, all are negatively correlated with each other.**
<br>
****
<be>

## Model Performance:
<img src="Screenshots/Accuracy score.jpg" width="300" height="285"> <img src="Screenshots/Predicting the price.jpg" width="400" height="285">
<br>
<br>
**• Model accuracy is over 83%**
<br>
**• For this 2016 Tata SUV Manual (Petrol), the model predicts the price as 7.14 lakhs**
<be>

## <img src="https://user-images.githubusercontent.com/108053296/185756908-fbb62168-d923-48f2-992f-b8e2fde848fe.gif" width="48" height="48" > Conclusions:
   
   1. Maruti Suzuki remains the brand of the masses
   2. Hatchback and SUV are the most preferred car body types
   3. Possibly due to low maintenance and longer life cap (15 years), Petrol cars are the most common ones
   4. The model shows a good accuracy rate on the test dataset
   5. The model provides a meaningful price prediction for a pre-owned car, aligning with common expectations regarding its resale value.

## Future Scope of the Model for the Masses:
1. **Empowering Buyers**: The model can assist potential buyers in estimating the fair market value of a used car they are interested in. By inputting the car's relevant characteristics, such as make, model, year, mileage, condition, and additional features, the model can provide a predicted price range. This helps buyers make informed decisions and negotiate better deals.
2. **Transparent Pricing**: The model can increase transparency in the used car market by providing a standardized and objective pricing mechanism. It reduces information asymmetry between sellers and buyers, ensuring that individuals are less likely to be taken advantage of due to a lack of market knowledge. The model's predictions can serve as a reference point for evaluating a seller's asking price.
3. **Saving Time and Effort**: Instead of manually researching and comparing prices for similar used cars, individuals can rely on the machine learning model to quickly estimate a fair price range. This saves time and effort for potential buyers, allowing them to focus on other aspects of the purchasing process.
4. **Selling Assistance**: The model can also benefit sellers by guiding them in setting reasonable prices for their used cars. By considering the characteristics of their vehicle and examining the predicted price range, sellers can ensure they are not undervaluing or overpricing their cars. This helps sellers attract potential buyers more effectively.
5. **Financial Planning**: The availability of accurate price predictions can aid individuals in their financial planning. For example, if someone intends to sell their car in the future, they can estimate its potential value using the machine learning model. This information allows them to make informed decisions about when to sell and how it may impact their overall financial situation.

## Contributing
Contributions are always welcome! Especially if you can help me with creating a UI for this model to make it useful for masses.
