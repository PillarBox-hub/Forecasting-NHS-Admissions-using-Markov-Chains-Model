# Forecasting-NHS-Admissions-using-Markov-Chains-Model
For an organisation to plan effectively, it is essential that it can in some way anticipate the future. This project uses ten years of historical NHS A&amp;E admission data to predict the next ten years of A&amp;E admissions flow, using the Markov chain model. This can enable hospitals to make the necessary decisions in effective hospital management.

# Objectives
The overall goal of this project is to contribute to the research on predicting patience admissions in the NHS.
This project specifically aims to use ten years of historical NHS A&E admission data to predict the next five years of A&E admissions, using the Markov chain model. 
This can enable hospitals to make the necessary decisions in effective hospital management. 

# Methodology
This paper is structured into 6 main parts, using the cross-industry standard process for data mining (CRISP-DM), a 1996 methodology created to shape Data Mining projects.
Firstly, Project Understanding: The initial phase of this project focuses on understanding the requirements of the project and setting goals to meet the requirements. Secondly, the Data Understanding phase: After understanding the requirements of this project, we then convert that knowledge into data sourcing.
The data preparation phase covers cleaning, formatting, combining, analysing, and visualising the data set. 
In the modelling phase, various modelling techniques are explored, including traditional forecasting techniques like ARIMA, and SARIMA, Monte Carlo simulation and  the Markov Chain technique. 
During the evaluation phase, the Markov chains model is reviewed to ensure it properly achieves the objective. We then measured predictive performance using the Monte Carlo uniform distribution and considered how this changed in different scenarios of admissions data. 
Finally, during the deployment phase, the knowledge gained from this project will be presented in a way that is useful to the NHS.

# Key Findings
This project attempts to accurately forecast the next ten years of NHS admissions, using historical data. The predicted results were compared to the actual results of the ten years of historic data, and we observed an average of 6.27% in-accuracy. This reveals that admissions are not so unpredictable, except for a fluke in the year of the COVID-19 pandemic.



# Code Scripts and their Description

1. **Admissions.zip** 

This folder contains 8 Python scripts for quarterly forecasts across 10 years. 

**1.Q1Type1Final represents the first Quarter for type 1 A&E admissions predictions from 2022 to 2031** 

**2. Q1Type2Final represents the first Quarter for type 2 single speciality admissions predictions from 2022 to 2031** 

**3. Q2Type1Final represents the second Quarter for type 1 A&E admissions predictions from 2022 to 2031** 

**4. Q2Type2Final represents the second Quarter for type 2 single speciality admissions predictions from 2022 to 2031** 

**5. Q3Type1Final represents the third Quarter for type 1 A&E admissions admissions predictions from 2022 to 2031** 

**6. Q3Type2Final represents the third Quarter for type 2 single speciality admissions predictions from 2022 to 2031**

**7. Q4Type1Final represents the fourth Quarter for type 1 A&E admissions predictions from 2022 to 2031**

**8. Q4Type2Final represents the fourth Quarter for type 2 single speciality admissions predictions from 2022 to 2031**


2. **Forecast1.zip**


This file contains 2 Python scripts for Quarterly forecasts across 10 years mainly using numpy and pandas. Transition matrix are applied to the actuals to derive the forecasts for the said durations. 

**A. Type1 represents the Quarterly predictions for A&E admissions based on the transition matrix{probability})**

**B. Type2 represents the Quarterly predictions for single speciality admissions based on the transition matrix{probability})** 





3. **TestModels**



This file contains 4 python jupyter notebook files:


**A. DataInTen mostly  involves the use pandas and time series machine learning tecniques like arima etc to carry out forecast for both A&E admissions and single speciality admissions and compared to Markov Chains. These models are evaluated and their performances compared as well with ARIMA performing quite poor as compared to Markov Chain** 

**B. P represents to use of numpy to define functions that carries out forecast using transition matrices for quarter 1 admissions** 

**C. Q1Type1Second represents further functions defined to carry out predictions on type 2 admissions using markov chain**

**D. Upgrad represents further addition of code to predict for subsequent quarters i.e. Q2,Q3,Q4** 





