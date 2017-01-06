+++
# Date this page was created.
date = "2016-04-27"

# Project title.
title = "2. (GIS) Predicting Development Pressure: Case in Korea "

# Project summary to display on homepage.
summary = "Developed a model to measure the development pressure and are currently considering applying it in practice at LH Corp., which is , a Public enterprise."

# Optional image to display on homepage (relative to `static/img/` folder).
image_preview = "main_pic_budget.png"

# Optional image to display on project detail page (relative to `static/img/` folder).
image = ""

# Tags: can be used for filtering projects.
# Example: `tags = ["statistical-learning", "econometrics"]`
tags = ["Statistical-Learning","Econometrics","GIS"]

# Optional external URL for project (replaces project detail page).
external_link = ""

# Does the project detail page use math formatting?
math = false

+++

# Abstract
Developed a model to measure the development pressure and are currently considering applying it in practice at LH Corp., which is , a Public enterprise.

```
#Keywords: GIS, econometrics, development pressure, dynamic programming, generalized linear model, L2 penalty
```
# Introduction/Background
![Intro](https://drive.google.com/uc?export=&confirm=no_antivirus&id=0B2x5sIkwVHb7QU9PaHJORnMzM2s)
Which area should be developed? The National Assembly is still debating today. One of the most important tasks for LH Corporation, a Public enterprise, is to measure and predict development pressures. The company focuses especially on the development pressure according to the needs of the market, because if the company cannot figure it out, there will be cases where it is necessary to build an apartment or build a road. For this reason, it is very important to measure the development pressure.


# Problem
Currently, there are few scientific tools used to accurately predict development pressure from National Agency in Korea. The first reason is lack of quality data. The data was computerized and archived for a long time, but it was so big and complicated that it was not kept neatly. Lastly, In Korea, we have never studied scientific development pressure by applying time and space at the same time.

# Solution
![Solution1](https://drive.google.com/uc?export=&confirm=no_antivirus&id=0B2x5sIkwVHb7QVpndGlfbkNjMVk)
![Solution2](https://drive.google.com/uc?export=&confirm=no_antivirus&id=0B2x5sIkwVHb7LWZoeW1KcDN5b3c)
![Solution3](https://drive.google.com/uc?export=&confirm=no_antivirus&id=0B2x5sIkwVHb7MFdpY1MtTzNJVG8)
We have developed a development pressure prediction model that has the concept of time and space by normalizing massive amounts of data. The model identifies the impacts between the layers through the hierarchical structure that the land has, and grasps the influence relations between the adjacent regions according to spatial conditions. Next, the model identifies how the above characteristics have changed over time.
![Solution4](https://drive.google.com/uc?export=&confirm=no_antivirus&id=0B2x5sIkwVHb7b1BlcDU4amdwczg)
The definition of development pressure was defined as "the number of land movements", "the number of transactions in land transactions", and "the number of building permits" after consultation with practitioner at LH corporation. However, since each number is too large a concept is defined more precisely as seven in above. The independent variables used in the model were about 200 such as area and landmark.


# Result
![result1](https://drive.google.com/uc?export=&confirm=no_antivirus&id=0B2x5sIkwVHb7YlJpcEFibzN3eEU)
![result2](https://drive.google.com/uc?export=&confirm=no_antivirus&id=0B2x5sIkwVHb7Wkc3SElRZTZ4eUE)
![result3](https://drive.google.com/uc?export=&confirm=no_antivirus&id=0B2x5sIkwVHb7Nk4yUGFCTDlrdlE)

Of the approximately 200 variables, 168 are statistically significant. Predictability is also excellent. Currently, LH Corporation is considering to use it in practice.
