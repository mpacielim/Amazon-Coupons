# Amazon-Coupons

This repository contains an analysis of a survey dataset that recorded information on drivers who were sent coupons for different businesses (such as bars, coffee shops and restaurants) while driving. 

The goal of the analysis was to determine whether or not the driver would accept and use the coupon.

This was completed as part of the Berkeley Professional Certificate in Machine Learning and Artificial Intelligence course, with the data coming from the UCI Machine Learning repository, collected via Amazon Mechanical Turk.

## Findings Summary
The full analysis can be found in this jupyter notebook: [prompt_coupon_mpaciepnik.ipynb](https://github.com/mpacielim/Amazon-Coupons/blob/main/prompt_coupon_mpaciepnik.ipynb)

The analysis focused on customers who were sent coupons for either bars or coffee shops, with the following hypotheses formed:

### Bars
Bar coupons had an overall acceptance rate of 41.2%

Drivers were **MORE** likely to accept the coupon if:
1. They go to a bar more than 3 times a month
2. They are <30 years old and go to bars atleast once a month
3. They have no kid passengers

Observations which filtered for drivers in these categories showed acceptance rates of atleast 75%, ranging up to 80%, compared to the overall bar coupon acceptance rate of 41%. 

Drivers were **LESS** likely to accept the coupon in opposite categories, meaning:
1. Those who went to bars less than once a month (29% acceptance)
2. Those who went less than 3 times a month at 37%.

### Coffee Shops
Coffee shop coupons had an overall acceptance rate of 49.6%.

Drivers were **MORE** likely to accept a coffee coupons if:
1. Their occupation status is either student, unemployed, healthcare or transport/material movement.
2. They are driving in hot weather conditions (80°F)
3. Their education status is "some college - no degree"
4. They are 26 years old or less
5. They are driving in the same direction as the coffee house
6. They got to a coffee house more than once a month
The coffee coupon acceptance rate when taking into account all the 6 conditions above is 100.0%.

Drivers were **LESS** likely to accept a coffee coupon if:
1. Their occupation status is in sales, education, legal, office/admin, social services, food preparation, or they are retired
2. They are driving in temperatures below 60°F
3. They have a bachelor's degree
4. They are 31 or older, specifically if they are 50+ years old
5. They are driving in the opposite direction as the coffee house
6. They go to a coffee house less than once a month
The coffee coupon acceptance rate when taking into account all the 6 conditions above is 19.4%.

### Next Steps & Recommendations
The hypothesis and results above are based on categories with vastly different sample sizes (for example, 60% of the coffee coupon data was for temperature conditions in the 80°F category, and 27% of respondents were students/unemployed, while the other 23 categories were 3% or less of the data each).

The hypothesis provide a good indication of which categories were more likely to influence coupon acceptance, but further samples are recommended to ensure all categories are captured.
