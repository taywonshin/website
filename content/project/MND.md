+++
# Date this page was created.
date = "2016-04-27"

# Project title.
title = "1. Predicting Dynamic Models of Quit Behavior, Ministry of National Defence, Korea "

# Project summary to display on homepage.
summary = "Created an econometrics model of the labor department of the Ministry of National Defence to achieve a quantitative effect of 120 billion won per year. Being in use since 2016."

# Optional image to display on homepage (relative to `static/img/` folder).
image_preview = "main_pic_budget.png"

# Optional image to display on project detail page (relative to `static/img/` folder).
image = ""

# Tags: can be used for filtering projects.
# Example: `tags = ["Statistical-Learning", "Econometrics"]`
tags = ["Statistical-Learning","Econometrics"]

# Optional external URL for project (replaces project detail page).
external_link = ""

# Does the project detail page use math formatting?
math = false

+++

# Abstract
Created an econometrics model of the labor department of the Ministry of National Defence to achieve a quantitative effect of 0.2 billion dollars per year. Being in use since 2016. 

Keywords: military, econometrics, budget projection, dynamic programming, generalized linear model, L2 penalty

# Introduction/Background
![Intro](https://drive.google.com/uc?export=&confirm=no_antivirus&id=0B2x5sIkwVHb7dS1sV0VsVUNyYXM)
In management of military manpower, military retention is a major subject. Policy makers are regulating its size by controlling the rate of retention and re-enlistment and those are closely related to personnel budget since military is a labor-intensive government organization. Most of the countries spent approximately 35% of budget of the total national defense for directly paying it to soldiers.


# Problem
![Problem](https://drive.google.com/uc?export=&confirm=no_antivirus&id=0B2x5sIkwVHb7UXBXMlA2TkQ0ekE)
One of the main reasons for shorts/overs was the formula for computing total national defence labor expense budget wasn't best formula. The formula uses average salary grade at F year in order to compute F+2 year budget. It also does not adequately reflect existing personnel when organizing F+2 year military personnel.

# Solution 
![Sol](https://drive.google.com/uc?export=&confirm=no_antivirus&id=0B2x5sIkwVHb7Z3FIV2s2WU1Tb2c)
![Sol2](https://drive.google.com/uc?export=&confirm=no_antivirus&id=0B2x5sIkwVHb7dGdXUnFYMVRyeTA)
![Sol3](https://drive.google.com/uc?export=&confirm=no_antivirus&id=0B2x5sIkwVHb7OFNuRFF2OGIwTkE)
We build an econometrics model for predicting retention rate. The model was inspired by the basic context of decision process of whether the person will stay or leave the military. Past studies on related subject have showed that risk aversion is the basic behavior of public servant thus we build the model based on that assumption. The model first compares how much the person will earn if he stays in military and leaves military until retire point ‘T’. Then reflects personal characteristics of personal information such as grades, year of services, promotion candidate, commission background, number of childerns education level, and other 124 factors.

![Sol3](https://drive.google.com/uc?export=&confirm=no_antivirus&id=0B2x5sIkwVHb7VEhGX1FNLVc3dGs)
![Sol4](https://drive.google.com/uc?export=&confirm=no_antivirus&id=0B2x5sIkwVHb7a1RzZmU1b2tLems)
The proper data manipulation was made based on the Military personnel Law and data from Ministry of Labor. Past 50 years of the Military personnel Law was applied since some of the personal characteristics are closed related such as retirement policy, salary grade policy, promotion policy and etc. Moreover, it is natural to think that soldier will be hired the field where they have devoted in military. We have thus matched 50 occupation speciality to 11 different sectors and applied average salary based on sex and proper salary grades. 


Finally, we added random effect term to induce unbiased estimate of coefficient of the model. Each of the soldier has more than one chance to leave the military. In order to reflect those natural context, we have successfully added random effect in the formula. 


# Result
![Sol5](https://drive.google.com/uc?export=&confirm=no_antivirus&id=0B2x5sIkwVHb7eDVsc3EwM1dtXzA)
The result of model is out-standing. The classification accuracy of train set is 98.43% which was evaluated by performing 10 rolling origin cross validation and accuracy of ‘out-of-sample’ test set is 97.73%. Decision boundary was chosen at convention level of 0.5. 

# Effect
![Sol6](https://drive.google.com/uc?export=&confirm=no_antivirus&id=0B2x5sIkwVHb7R0lTd3lLSTVma1U)
The forecasting model was completed in 2016 and used from 2016 to measure the 2017 budget. Practitioners are expecting to achieve a quantitative effect of about 0.2 billion dollars per year. This labor cost prediction model project is the first in the Korean government ministries and can be extended to the civil servant area. Especially, the Ministry of Education will be able to see a great effect. It is also a project where three divisions have succeeded in cooperating with each other to break down each closed department.

# Details
+ Error Metrics: MAPE (mean absolute percentage error), MAE (mean absolute error)
+ Estimation Technique: IWLS algorithm, EM algorithm, Adaptive Gauss-Hermit Approximation, BLUP, BFGS

