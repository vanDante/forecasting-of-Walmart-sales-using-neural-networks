INTRODUCTION

The two notebooks show how to use (i) a neural network with categorical embeddings or (ii) light gradient boosting with day-to-day prediction to forecast the sales of Walmart stores in the United States for a period of 28 days. 

The work is part of the M5 Competition, a cooperation of the Makridakis Open Forecasting Center (MOFC) at the University of Nicosia and Walmart (https://mofc.unic.ac.cy/m5-competition/). The aim of the M5 Competition is to identify the most appropriate method(s) for different types of situations requiring predictions and making uncertainty estimates. Its ultimate purpose is to advance the theory of forecasting and improve its utilization by business and non-profit organizations. Its other goal is to compare the accuracy/uncertainty of ML and DL methods vis-à-vis those of standard statistical ones, and assess possible improvements versus the extra complexity and higher costs of using the various methods.

In both notebooks, to optimize the model (neural network/light gradient boosting) I implemented a 3-fold cross-validation taking into account the previous two month and the same month of the previous year as validation periods. I implemented a store-WRMSSE as validation metric, which is simply the error which the respective store contributes to the overall WRMSSE (regarding all data).
More information on the evaluation metric (WRMSSE) can be found here (https://mofc.unic.ac.cy/wp-content/uploads/2020/03/M5-Competitors-Guide-Final-10-March-2020.docx).

The notebooks are also published on kaggle:
(i) https://www.kaggle.com/dantefilu/nn-on-store-level-with-3-fold-cv-store-wrmsse
(ii) https://www.kaggle.com/dantefilu/lgbm-on-store-level-with-3-fold-cv-store-wrmsse

Unfortunatelly the input data is not fully public but easily accessible via kaggle:
https://www.kaggle.com/c/m5-forecasting-accuracy/data

    
