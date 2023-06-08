# 

# Prediction of prices of Used Cars (Machine Learning)

**The project involves a usage of supervised learning to build a Linear Regression model that predicts the prices of used cars. The idea behind this was to build a smart Machine Learning model that could help- 1. A buyer to know a reasonable price of a used car based on his desired features, and 2. A seller to get a reliable idea of the current value of their used car. For this, data of more than 1000 used cars, scraped from spinny.com using selenium, was used after doing intensive feature engineering, data manipulation & visualisation, using numpy, pandas, seaborn, finally giving way to creating a Linear Regression Model. The model shows accuracy of more than 80% and is able to reliably provide a meaningful prediction of prices of used cars in India.**

<br>
<br>
<p align="center"><a><img src="https://forthebadge.com/images/badges/built-with-love.svg"><img src="https://forthebadge.com/images/badges/made-with-python.svg"></a></p>

##  <img src="https://user-images.githubusercontent.com/106439762/181935629-b3c47bd3-77fb-4431-a11c-ff8ba0942b63.gif" width="42" height="42"> **User's Manual**

| Files/Folder | Description |
| ------------- | ------------- |
| **Web Scraping** | Contains ipynb code of web scraping spinny.com, a company that provides services to buy & sell pre-owned cars |
| **Raw Data Files** | Provides the raw data generated through web scraping, in csv format |
| **Feature Engineering** | Contains python codes written to clean, prepare and modify data to make it model ready |
| **Final CSV File** | This folder provides the final csv file after feature engineering, ready for model building and drawing insights |
| **Project PPT File** | This file provides the powerpoint presentation which contains all the major steps, insights, challenges and conclusions |
<br>

# Installation Instructions
    o  Provide step-by-step instructions on how to install and set up your project. Include any necessary dependencies, libraries,
       or packages required for running your code
    o  Operating System: Windows, macOS, or Linux
    o  Processor: Intel Core i5 or i7
    o  RAM: At least 6GB, although 8GB or more is recommended for smoother performance
    o  Storage: Sufficient free disk space to install Python, Jupyter Notebook, and other necessary libraries
    o  Python: Install the latest version of Python (3.7 or later) from the official Python website (https://www.python.org/downloads/).
       Make sure to select the appropriate version for your operating system
    o  Jupyter Notebook: Install Jupyter Notebook using pip, which is usually included with Python by default. Open a terminal or
       command prompt and run the command: pip install jupyter
    o  Selenium: Install Selenium library using pip. Run the following command in your terminal or command prompt: pip install selenium
    o  Web Driver: Selenium requires a web driver to interact with web browsers. The appropriate web driver depends on the browser
       you intend to use. The most popular web drivers are:
        1. Chrome: ChromeDriver (https://sites.google.com/a/chromium.org/chromedriver/)
        2. Firefox: GeckoDriver (https://github.com/mozilla/geckodriver/)
        3. Safari: SafariDriver (comes bundled with Safari)
    o  Download the appropriate web driver for the browser you'll be using and make sure to place it in a directory included in your
       system's PATH environment variable. I have used ChromeDriver
    o  Once you have the above configuration, you should be able to run Python code for web scraping using Selenium in Jupyter Notebook.
    o  Install scikit-learn for Machine Learning: Open a terminal or command prompt and run the command to install scikit-learn using
       pip: pip install scikit-learn
    o  That's it, now you can start using the project on your own pc

# Usage Guide
Explain how to use your project. Provide clear instructions on how to preprocess the data, train the machine learning model, and make predictions using the trained model. Include code snippets or examples to illustrate the process.
1. To start using the project, let's start by opening Jupyter Notebook and runing the web scraping codes available in the User's Manual. Just 
2. The code will automatically store data in



4. Dataset Description: Briefly describe the dataset you used for training and evaluating your model. Mention the source of the dataset, the number of samples, and the features available. If possible, provide a link to the dataset or include it in your repository.

5. Model Architecture: Describe the architecture of your machine learning model. Explain the algorithms, techniques, or frameworks you used to build the model. Provide information about the input and output of the model.

6. Evaluation Metrics: Specify the evaluation metrics you used to assess the performance of your model. Common metrics for regression tasks like predicting car prices include mean absolute error (MAE), mean squared error (MSE), and R-squared (R²) score. Explain how to interpret these metrics and what values indicate better performance.

7. Pretrained Model: If you have a pretrained model available, provide instructions on how to download or load the model for making predictions without retraining. Include any necessary files or weights associated with the pretrained model.

8. Examples and Results: Share some examples or case studies demonstrating the usage of your model. Provide code snippets or scripts to showcase how to use the model for making predictions on new data. Include some sample outputs or visualizations to illustrate the results.

9. Limitations and Future Work: Acknowledge any limitations or assumptions in your model or dataset. Discuss potential improvements or additional features that could be explored in the future to enhance the predictive accuracy or performance of the model.

10. Contributions and License: Specify whether you welcome contributions to your project and explain how users can contribute. Also, include the license under which you're releasing your code, ensuring that it aligns with your intended usage and distribution.

11. Contact Information: Provide your contact details, such as your email address or GitHub profile, so that users can reach out to you with any questions, suggestions, or issues they encounter.


