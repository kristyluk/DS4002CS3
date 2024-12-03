# DS4002 CS3 Predicting Gender Wage Ratios Case Study 
### Fall 2024 - Kristy Luk

This repository contains information, data, and scripts based on Project 2 of this course, which focused on time-series data. You are tasked to use ARIMA forcasting model to predict gender wage ratios. 

### This repository is organized as follows:
1. DATA
    - full_data.csv --> orginial dataset before cleaning
    - cleaned_data.csv --> cleaned dataset 
    - 20th_century_data.csv --> data from the cleaned dataset, but only from 1960-2001 for the ARIMA modeling 
    - Data Appendix.pdf --> Data Appendix for all variables in the dataset used in the project
      
2. SCRIPT
    - final_script.ipynb --> a full script containing all of the code needed to reproduce results

3. Reference Materials
    - ARIMA for Time Series Forecasting_A Complete Guide.pdf --> additional information about ARIMA forcasting 
    - Gender pay gap remained stable over past 20 years in US.pdf --> more in depth article about gender wage disparities in the US
      
4. CS3 Case Study Hook Document.pdf
   
5. CS3 Case Study Rubric.pdf
   
6. README.md
   
### Instructions for reproducing results
#### Please follow these steps in order to replicate this project's experimental design:

1. Download all three .csv files from the DATA folder. This step is not particulary necessary since the script extracts the data files straight from this DATA folder. 
2. Open up "final_scipt.ipynb" located in the SCRIPT folder using Google Colab. Load the datset using the code in the file, and then follow the code to perform inital EDA. Then, you can begin the ARIMA modeling process after downloading the necessary Python libraries. The first section details steps on how to select appropriate values for p, d, and q values using the data visualizations created in the code. The code under the "Choosing best ARIMA parameters" consists of some tests and plots used to determine appropriate parameters. Feel free to change the parameters if you feel there are more fitting values. The second part of the ARIMA modeling process is the code located under the "Now actually using the ARIMA model" section. This is where ARIMA will use the historical wage ratio data from 1960-2000 to predict the wage ratios for 2001-2019. A model fit summary and dataframe of the predicted and actual wage ratios will be generated to easily compare the values. Then, the MSE, RMSE, and residuals are calculated. The code will plot the residuals on a plot, display summary statistics of the residuals, and display a graphic of the actual and predicted wage ratios.
3. Lastly, the section "OPTIONAL: Attempting To Model Using Holt's Dampened Trend" is a little extra code we deployed that tried to forcast the wage ratio using exponential smoothing techniques. 
   
## References
[1] B. Etienne, “Time Series in Python — Exponential Smoothing and ARIMA processes,” TowardsDataScience.com, https://towardsdatascience.com/time-series-in-python-exponential-smoothing-and-arima-processes-2c67f2a52788.  
[2] D. Abugaber, “Chapter 23: Using ARIMA for Time Series Analysis,” University of Illinois Chicago, https://ademos.people.uic.edu/Chapter23.html/.  
[3] J. Brownlee, “How to create an Arima model for time series forecasting in Python,” MachineLearningMastery.com, https://machinelearningmastery.com/arima-for-time-series-forecasting-with-python/.  
[4]	Fuqua School of Business, "Introduction to ARIMA: nonseasonal models," https://people.duke.edu/~rnau/411arim.htm.  
[5] C. Aragão, "Gender pay gap in U.S. hasn’t changed much in two decades," Pew Research Center, https://www.pewresearch.org/short-reads/2023/03/01/gender-pay-gap-facts/.  
[6] Z. Saadeddin, "ARIMA for Time Series Forecasting: A Complete Guide," DataCamp, https://www.datacamp.com/tutorial/arima.
