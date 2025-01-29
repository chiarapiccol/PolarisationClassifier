# Polarisation Classifier
This repository contains the RMarkdown analysis for University Project. The project focuses on classifying and analyzing parliamentary speeches from the German Bundestag from 1991 to 2018.

## 1. Data Preparation
Install necessary packages.
Clear the workspace and set the working directory.
Load the main dataset using the foreign package.
## 2. Data Exploration
Analyze the dataset to understand its structure and content.
Perform analysis on the temporal and structural aspects of the data.
## 3. Data Processing
Clean the dataset by removing rows with missing values in the party column.
Create dummy variables for party affiliation.
Split the dataset into different legislative periods for focused analysis.
Transform the text data into a machine-readable format by removing punctuation, numbers, and stopwords.
## 4. Data Splitting
Split the data into training and testing sets using stratification.
Further split the testing data into pairs of parties for detailed analysis.
## 5. Creating Document-Term Matrix (DTM)
Build DTMs for both training and testing datasets using the Keras package.
## 6. Model Training
Train six different models using the XGBoost algorithm to classify speeches based on party affiliation.
## 7. Model Evaluation
Evaluate the models using the test dataset.
Calculate probabilities for each speech to determine its party affiliation.
## 8. Transforming Probabilities
Transform the calculated probabilities into binary classifications.
## 9. Model Accuracy and Polarization
Calculate accuracy, precision, and recall for each model.
Compare the performance of different models and assess the polarization degree between parties.

# Additional Information
The project involves analyzing speeches to understand their length, most frequent words, and distribution of the target variable.
The models aim to classify speeches based on party affiliation and assess the polarization degree by comparing interparty and intraparty heterogeneity.
# Requirements
R packages: haven, foreign, tidyverse, stringr, plyr, tm, ggplot2, splitstackshape, dplyr, textstem, stargazer, gridExtra, keras, tensorflow
Clone the repository: git clone https://github.com/chiarapiccol/PolarisationClassifier.git
Install the required packages listed in the Data Preparation section.
Load the dataset and follow the steps outlined in the RMarkdown file to reproduce the analysis.
