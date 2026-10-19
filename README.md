# Project Title: Signature Assignment 8: Comparing GAM vs SARIMAX and Direct GAM vs Recursive GAM to forecast PIC deaths

## Author
Dawud Ujamaa

## Project Overview
The ability to accurately forecast deaths due to respiratory viruses such as Pneumonia, Influenza, and COVID-19 (PIC) helps healthcare professionals prepare timely responses to mitigate the adverse impacts. Previous studies have used forecasting models such as Autoregressive Integrated Moving Average (ARIMA) and Generalized Additive Model (GAM) to forecast Pneumonia, Influenza, and/or COVID-19 incidence and hospitalizations. However, there have been no previous studies published forecasting PIC deaths. Additionally, the ability to forecast multiple steps into the future for a given time horizon is an important component of time-series forecasting. Direct and Recursive are two strategies for multi-step forecasting which have investigated in previous studies using ARIMA models. However, there have been no published studies investigating Direct and Recursive multi-step forecasting strategies using GAM models. This study compares and evaluates the performance of ARIMA and GAM models used to forecast PIC deaths, and also compares and evaluated the performance of GAM models using Direct and Recursive multi-step forecasting strategies to forecast PIC deaths. 

## Dataset Information
The dataset used in this analysis is the “US COVID-19 Pneumonia & Flu Deaths Data: Weekly state-level mortality counts for time-series forecasting” by Ihab (n.d.) available from https://www.kaggle.com/datasets/razanihababdellatif/us-covid-19-pneumonia-and-flu-deaths-data

## CRISP-DM Process
The methodology used in this study is organized around the six steps of the CRISP-DM (Cross-Industry Standard Process for Data Mining) theoretical framework: (a) business understanding (provided in the problem statement and purpose statement), data understanding (Exploratory Data Analysis), Data preparation (Data Cleaning, Preprocessing, Feature Engineering, and Feature selection), modeling, evaluation, and deployment (this report). There are 3 modular jupyter notebooks for this analysis separated based on CRISP-DM:
1. UjamaaDDDS7255-8-1.Business_and_Data_Understanding.ipynb
2. UjamaaDDDS7255-8-2.Data_Preparation.ipynb
3. UjamaaDDDS7255-8-3.Modeling_Evaluation_Deployment.ipynb 

## Repository Structure
The repository structure is as follows:
-data/	 # Raw dataset
-output/ # model outputs, evaluation metrics, and visualizations
All modular jupyter notebooks are in the main folder

## How to Run the Project
1. Open Jupyter Notebook.
2. Navigate to the project folder.
3. Execute the modular notebooks in the appropriate order, or
4. Execute this notebook to run the whole analytic pipeline: UjamaaDDDS7255-8-3.Modeling_Evaluation_Deployment.ipynb

## Dependencies 
This project uses Python version 3.12.7 and the following Python packages should be installed using pip.
numpy==1.26.4
pandas==1.5.3
matplotlib==3.9.2
seaborn==0.13.2
sklearn==1.5.2
statsmodels==0.14.4
pmdarima==2.0.4
pygam==0.9.1
scipy==1.11.4
dieboldmariano==1.1.0

## Results and Insights  
This study has compared and evaluated the accuracy of SARIMAX and GAM models at forecasting PIC deaths and compared and evaluated the accuracy of GAM models using Direct and Recursive multi-step forecasting strategies to forecast PIC deaths. The key insights and findings from this study were: (a) the SARIMAX model slightly outperformed the GAM model at one-week ahead forecasting of PIC deaths, however the difference in performance was not statistically significant; and (b) the GAM model using the Direct 4-week ahead forecasting strategy performed better than the GAM model using the Recursive 4-week ahead forecasting strategy, however the difference in performance was not statistically significant. Future areas of research include comparing the multi-step performance of GAM models and SARIMAX models and evaluating the multi-step forecasting performance of GAM models using different strategies at longer and shorter forecasting horizons. These finding can help inform Data Scientists working in the fields of healthcare and Public Health to improve modeling of deaths related to Pneumonia, Influenza, and COVID-19.
