# AV : HEALTHCARE ANALYTICS II PROJECT

Welcome to my first project, this is my work for Janatahack: Healthcare Analytics II hackathon on [Analytics Vidhya](https://datahack.analyticsvidhya.com/contest/janatahack-healthcare-analytics-ii/)

## Overview

Recent Covid-19 Pandemic has raised alarms over one of the most overlooked area to focus: Healthcare Management. While healthcare management has various use cases for using data science, patient length of stay is one critical parameter to observe and predict if one wants to improve the efficiency of the healthcare management in a hospital. 

This parameter helps hospitals to identify patients of high LOS risk (patients who will stay longer) at the time of admission. Once identified, patients with high LOS risk can have their treatment plan optimized to miminize LOS and lower the chance of staff/visitor infection. Also, prior knowledge of LOS can aid in logistics such as room and bed allocation planning.

## Approach

By creating Machine Learning model to predict patient LOS, we could :

1. Predict currently treated patient LOS, and..
2. Predict recently admitted patient would be LOS

to get an overview for better room management

## EDA

**Here's how the patient's LOS is distributed, notice that we are dealing with imbalanced data with 11 classes**<br>
![alt text](https://github.com/kimichiaveli/AV-Healthcare-Analytics-II-Project/blob/main/dis2.png?raw=true)<p>

**This is how the patient's cases are distributed based on the hospital code and region**<br>
![alt text](https://github.com/kimichiaveli/AV-Healthcare-Analytics-II-Project/blob/main/fig2.png?raw=true)<p>

**Here is the distribution of "Available Extra Rooms" when a patient is admitted**<br>
![alt text](https://github.com/kimichiaveli/AV-Healthcare-Analytics-II-Project/blob/main/fig3.png?raw=true)<p>
![alt text](https://github.com/kimichiaveli/AV-Healthcare-Analytics-II-Project/blob/main/fig4.png?raw=true)<p>
  
**This chart shows that majority of patient were admitted to the hospital outside their city. The inner chart shows the composition based on the severity of their case**<br>
![alt text](https://github.com/kimichiaveli/AV-Healthcare-Analytics-II-Project/blob/main/fig10.png?raw=true)<p>

 ## Model Evaluation
 
 **Using CatBoost algorithm with the class weight parameter set to be true, we built a model that does not over-predict a class**<br>
 ![alt text](https://github.com/kimichiaveli/AV-Healthcare-Analytics-II-Project/blob/main/cm.png?raw=true)<p>
