# Shared_Bikes
I Build a model to predict the shared bikes demand with the available independent variables (features).
It will be used by the company or management to understand how exactly the demands vary with different features.
They can accordingly manipulate the business strategy to meet the demand levels and reach the customer's expectations.

**Prilimanary details:**

Data : from client

Python: Googlecolab

EDA : Manuuvally, AutoEDA(Pandas_Profiling)

Model: Multi linear Regression and AutoML(TPOT)

**I follow the CRISP(MLQ) Procedure:**

*1. Business and Data Understanding.

*2. Data Preparation.

*3. Model Engineering.

*4. Model Evaluation.

*5. Model Deployment.

6. Monitoring and Maintenance.

We construct the Multi Linear Regression model:

Final equation of MLR:

Count =  0.1832 + (temp * 0.2544) - (Humidity * 0.1361) - (windspeed * 0.1160) - (Season_spring * 0.0954) + (Season_summer * 0.0055) +  (Season_winter * 0.0855) + (Year_2019 * 0.2324) - (Month_Dec * 0.0650) - (Month_Feb * 0.0382) - (Month_Jan * 0.0562) - (Month_July * 0.0469) +
(Month_May * 0.0324) - (Month_Nov * 0.0665) + (Month_Sept * 0.0629) -
(holiday_Yes * 0.1065) - (weekday_Thurs * 0.0177) - (weekday_Tues * 0.0301) - (weekday_Wed * 0.0329)+ (Weather_Good_Clear * 0.2213) +
(Weather_Moderate_Misty * 0.1694)

# **Final Reuslt(MLR):**

* R2 score(test):  0.8437

* R2 score(train):  0.8445

* adjusted R2 score(test): 0.8278

* adjusted R2 score(train): 0.8288

Its right fit model.

# **Final Reuslt(AUTOML):**

R2 score(test): 0.8974

R2 score(train): 0.9538

Its  a slighly over fit model.

# **Conclusion:**

As per our final Model, the **top 3 predictor variables** that influences the bike booking are:

**Temperature (temp)** - A coefficient value of ‘0.2544’ indicated that a unit increase in temp variable increases the bike hire numbers by 0.2544 units.

**Year** - A coefficient value of ‘0.2324’ indicated that a unit increase in year variable increases the bike hire numbers by 0.2324 units.
So, it's suggested to consider these variables utmost importance while planning, to achive maximum Booking.

**Weather Situation (Good_Clear)** - A coefficient value of ‘0.2213’ indicated that, w.r.t Weather, a unit increase in Weather variable increases the bike hire numbers by 0.2213 units.

