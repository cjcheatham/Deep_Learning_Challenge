# Deep Learning Challenge

# Table of Contents
1. [Overview of the Repository](#overview)
2. [Model Report](#report)

## Overview <a name="overview"></a>

The nonprofit foundation Alphabet Soup wants a tool that can help it select the applicants for funding with the best chance of success in their ventures. With your knowledge of machine learning and neural networks, you’ll use the features in the provided dataset to create a binary classifier that can predict whether applicants will be successful if funded by Alphabet Soup.

From Alphabet Soup’s business team, you have received a CSV containing more than 34,000 organizations that have received funding from Alphabet Soup over the years. Within this dataset are a number of columns that capture metadata about each organization, such as:

* EIN and NAME—Identification columns
* APPLICATION_TYPE—Alphabet Soup application type
* AFFILIATION—Affiliated sector of industry
* CLASSIFICATION—Government organization classification
* USE_CASE—Use case for funding
* ORGANIZATION—Organization type
* STATUS—Active status
* INCOME_AMT—Income classification
* SPECIAL_CONSIDERATIONS—Special considerations for 
* application
* ASK_AMT—Funding amount requested
* IS_SUCCESSFUL—Was the money used effectively

The preprocessing and compilation of the initial model can be found in the Deep_Learning.ipynb file. 

This initial model was then optimized in the AlphabetSoupCharity_Optimization.ipynb file (See report for more details).

All nn models created were saved in h5 format, and can be found in the H5_Models folder.

## Report <a name="report"></a>

### Overview

The purpose of this analysis was to create a tool for the nonprofit foundation Alphabet Soup that can help select the applicants for funding with the best chance of success in their ventures. To do this, we use our knowledge of machine learning and nueral networks, we will use the features of the provided charity.csv data set to create a binary classifier that can predict whether applicants will be successful if funded by Alphabet Soup.

### Results

* Data Preprocessing:

    #### Variables
    
    * Our y variable = "IS_SUCCESSFUL" column

    #### Features

    * Our features variable X includes every column but "IS_SUCCESSFUL". These columns include: "APPLICATION_TYPE", "AFFILIATION", "CLASSIFICATION", "USE_CASE", "ORGANIZATION", "STATUS", "INCOME_AMT", "SPECIAL_CONSIDERATIONS",
    "ASK_AMT".  

    #### Features Removed

    * Features removed incuded the "EIN" and "NAME" columns since they are neither targets nor features.

* Compiling, Training, and Evaluating the Model: 

    There were 3 attempts to get the model to 75% accuracy.

    * First Attempt: Consisted of two hidden layers, layer 1 = 10 nuerons relu activation and layer 2 = 6 nuerons relu activation. Outer layer = 1 unit sigmoid activation.

    * Second Attempt: Consisted of 3 hidden layers, layer 1 = 1o nuerons relu activation, layer 2 = 8 nuerons sigmoid activation, and layer 3 = 6 nuerons sigmoid activation. Outer layer = 1 unit sigmoid activation.

    * Third Attempt: Consisted of 3 hidden layers, layer 1 = 7 nuerons relu activation, layer 2 = 14 nuerons relu activation, and layer 3 = 21 nuerons

