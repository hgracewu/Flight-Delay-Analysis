# Flight Delay Prediction and Analysis

### Project Overview

This project is aimed at predicting flight delays using historical data from the U.S. Department of Transportation. The analysis is performed using Apache Spark, enabling the processing of large-scale data to model and predict delays based on various features such as airlines, flight dates, times, and routes.

### Environment Setup
To run this project, ensure that you have the following tools and libraries installed:

Python 3.10+

Apache Spark 3.5.1

PySpark

Java JDK 11

Kaggle API (for data acquisition)

### Installation Steps

1. Install PySpark and Java JDK:

!pip install pyspark

!apt-get install openjdk-11-jdk-headless -qq > /dev/null

2. Download and set up Spark:
   
!wget -q https://bitbucket.org/habedi/datasets/raw/spark/spark-3.0.2-bin-hadoop2.7.tgz

!tar xf spark-3.0.2-bin-hadoop2.7.tgz

!rm -rf spark-3.0.2-bin-hadoop2.7.tgz*

3. Install additional Python libraries:

!pip install findspark kaggle

4. Set up Kaggle API credentials:

import os

os.environ['KAGGLE_USERNAME'] = "your_kaggle_username"

os.environ['KAGGLE_KEY'] = "your_kaggle_key"

### Data Acquisition

Data is acquired from the Kaggle dataset "US DOT Flight Delays":

!kaggle datasets download -d usdot/flight-delays

### Data Processing

Data processing involves cleaning, transforming, and preparing the flight data for predictive modeling. Steps include handling missing values, encoding categorical variables, and normalizing dates and times.

### Predictive Modeling

We use Spark MLlib to train predictive models to forecast flight delays. Models include:

Random Forest Classifier
Logistic Regression
Decision Tree Classifier

###Evaluation

Model performance is evaluated using accuracy metrics to determine the effectiveness of each predictive model in forecasting delays.

### Running the Project

To run the analysis and modeling steps, execute the Jupyter notebook included in the repository:

jupyter notebook flight_delay_prediction.ipynb

### Contributions

Contributions to this project are welcome! You can contribute in the following ways:

Enhancing the predictive models

Adding more features to the models

Improving the data preprocessing steps

Documenting and writing more tests

### License

This project is licensed under the MIT License - see the LICENSE file for details.
