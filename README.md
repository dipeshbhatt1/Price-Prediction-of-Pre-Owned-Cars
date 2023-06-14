
# <img src="Media Files/icon.png" width="50" height="30"> Price-Prediction of pre-owned Cars <img src="Media Files/icon2.png" width="50" height="32">

<img src="Media Files/1.jpg" width="400" height="250"> <img src="Media Files/2.jpg" width="400" height="250">
<img src="Media Files/3.jpg" width="500" height="300"> <img src="Media Files/4.jpg" width="500" height="300">
<img src="Media Files/5.jpg" width="500" height="300"> <img src="Media Files/TATA NEXON GIF.gif" width="500" height="300">

## 📝 Description
* This repository represents **"Price-Prediction using a Multiple Linear Regression Model"**
* With the help of this project we can meaningfully and reliably predict prices of pre-owned cars based on their features.

## ⏳ Dataset 
* Data of over 6000 pre-owned cars was extracted from spinny.com
* After applying feature engineering and data preparation we are left with data of over 1000 pre-owned cars
* Download the dataset for custom training: LINK
----------------------
## 🏽‍ Download Object Detection Model
- Download the object detection model manually : **yolov3-spp.weights** file from following Drive Link
- https://drive.google.com/file/d/1h2g_wQ270_pckpRCHJb9K78uDf-2PsPd/view?usp=sharing
- Download the weight file and Place it into **" detector/yolo/data/ "** folder.

##  🏽‍ For Pose Tracking, Download the object tracking model
- For pose tracking, download the object tracking model manually: **" JDE-1088x608-uncertainty "** from following Drive Link 
- https://drive.google.com/file/d/1oeK1aj9t7pTi1u70nSIwx0qNVWvEvRrf/view?usp=sharing
- Download the file and Place it into **" detector/tracker/data/ ".** folder.

## 🏽‍ Download Fast.res50.pt file
- Download the **" fast.res50.pth "** file from following Drive Link 
- https://drive.google.com/file/d/1WrvycZnVWwltSa6cjeTznEFOyNAwHEZu/view?usp=sharing
- Download the file and Place it into **" pretrained_models/ ".** folder.
-----------------------


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
5. Once you have these all, launch the Jupyter Notebook using command prompt:
```bash
    jupyter notebook
```
6. Now you can start working on the project using the given dataset and python codes

_______________________________
## 🎯 Inference demo
1. Testing with **Images** ( Put test images in **AlphaPose/examples/demo/** )  :-
```bash
$ python scripts/demo_inference.py --cfg configs/coco/resnet/256x192_res50_lr1e-3_1x.yaml --checkpoint pretrained_models/fast_res50_256x192.pth --indir examples/demo/ --save_img
```
______________________

## Steps Involved (End to End)

1. **Objective:** To build a Machine Learning model (Linear Regression) that can predict prices (label) of used cars based on various features
2. **Data Collection:** For this, a reasonable and large enough dataset was required. Now, instead of looking for some old data or sample data available on internet, I decided to scrape website of a service provider already working in this field. So, I came across spinny.com which has a simple yet cool UI. Finally, the data was scrapped from this website.
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

